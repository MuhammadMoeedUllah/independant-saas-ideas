# DROP Fulfillment Engine for Small Registered Data Brokers: Product/Technical Feasibility and Go-to-Market (as of 2026-10-09)

> **How these notes were gathered (read first).** In this session the fetch tool could not resolve any domain, and the proxy blocked direct downloads from `privacy.ca.gov`, `cppa.ca.gov` and `dropresources.blob.core.windows.net`. Facts from CalPrivacy (CPPA) pages therefore come from three places: (a) search-engine extracts of those pages; (b) a third-party **verbatim copy of CalPrivacy's published OpenAPI 3.1.0 (v1.2.0)** and of the doc pages, kept by API Evangelist on GitHub and generated 2026-09-17; (c) California Legislature bill text (the PUBINFO dump mirrored on GitHub). **All 11 published single-field hashing test vectors and the NDZ composite vector were re-computed locally, and every one matched exactly.** That makes the hashing spec in these notes high-confidence. The web-search budget ran out before events, DropClerk pricing and the question of third-party vendor access to DROP could be researched. Those items are listed under Gaps.

## 1. DROP mechanics for brokers: access, identifiers, hashing, files, cadence, status reporting, docs, sandbox, onboarding

### Takeaway
DROP is a small, well-documented **batch file exchange**. The REST API has three operations (download a ZIP of CSVs, upload status CSVs, amend), and a manual portal download/upload path does the same thing. Brokers only ever get **SHA-256/Base64 hashes** of six identifier "list types," never raw PII. They must hash their own records under exact standardization rules, match them, and return one status code per work item, accessing DROP at least every 45 days from Aug 1, 2026. The hard part is not the API but the matching, deletion and evidence across the broker's own systems.

### Cited Findings
**Access and onboarding**
- Brokers can integrate "using the DROP Data Broker API or by using the manual download/upload option." The workflow is a repeating cycle: set up the account, generate a key, download the ZIP, extract the CSVs, match against your records, act on each match, upload status CSVs, then repeat steps 3–7. — [privacy.ca.gov Integration workflow](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/integration-workflow/); [privacy.ca.gov Getting started](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/)
- Base URLs: production `https://api.drop.privacy.ca.gov`, sandbox `https://api.drop.privacy.ca.gov/sandbox`. Auth is an `X-API-KEY` header. "Your API key is scoped to the consumer deletion list(s) you select. Only the selected list(s) will appear in your downloads." — [Getting started](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/); [verbatim OpenAPI copy (API Evangelist mirror)](https://github.com/api-evangelist/california-privacy-protection-agency)
- Production key path: Data Broker Portal (`databroker.drop.privacy.ca.gov`) → Consumer Deletion Lists → select lists → API Key tab → "Get a new API key." Sandbox key path: SANDBOX ENVIRONMENT → ISSUE SANDBOX API KEY. Keys are issued only after account approval, fee payment and selection of at least one list. There is no OAuth, and no anonymous or self-serve sandbox (it is reached from inside an approved broker account). — [Getting started](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/); [API Evangelist sandbox profile](https://github.com/api-evangelist/california-privacy-protection-agency)
- The OpenAPI description states that keys are generated in the Data Broker Portal "after registration and fee payment are complete." — [OpenAPI v1.2.0, verbatim copy](https://github.com/api-evangelist/california-privacy-protection-agency) (official YAML location listed as `dropresources.blob.core.windows.net/apidocs/databroker_api.yaml`; a CalPrivacy PDF version is at [cppa.ca.gov/orph/drop_tech_api_ref.pdf](https://cppa.ca.gov/orph/drop_tech_api_ref.pdf))
- Brokers "must select all lists that contain consumer identifiers that match to personal information about the consumer within their records." — [Processing DROP requests (search extract)](https://privacy.ca.gov/drop-for-data-brokers/process-drop-requests/)
- SB 361 (Ch. 466, Stats. 2025, approved 2025-10-08) requires registrants to disclose whether they collect names, dates of birth, ZIP codes, emails, phone numbers, mobile advertising IDs, connected-TV IDs and VINs, among other things. These map directly onto the DROP list types. — [SB 361 chaptered text via PUBINFO mirror](https://github.com/aaronjuar-ez/PUBINFO-2025) (bill page: [leginfo SB 361](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB361))

**Documentation versions and sandbox timing**
- Tech-doc and API versions: **1.0.0 (2026-04-02)**, an "initial release in DROP, accompanying the DROP Sandbox"; **1.1.0 (2026-06-03)**, general release on privacy.ca.gov, adding cancellations and the Removed CSV; **1.2.0 (2026-07-02)**, which clarifies ZIP+4 handling, documents work-item IDs and adds webhooks. — [Reference page version history, via API Evangelist changelog](https://github.com/api-evangelist/california-privacy-protection-agency); [Reference](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/reference/)
- Conflict: a vendor explainer says the full technical spec came out on **April 7, 2026**, and the mirror cites the DROP timeline for sandbox availability from **March 2026**. The 2026-04-02 version date comes from the agency's own version history. — [Superset](https://www.trustsuperset.com/post/what-is-the-california-drop-system)
- In an agency briefing (secondary summary), the sandbox was said to return direct comparison results, while production only validates status codes. Brokers were told to verify the contact emails on their account so validation results reach them. — [CitizenPortal summary of CalPrivacy briefing](https://citizenportal.ai/articles/8372638/California/Executive/Other-State-Agencies/California-Privacy-Protection-Agency/Cal-Privacy-walks-data-brokers-through-Droplevel-technical-steps-hashing-lists-API-and-sandbox-testing) (unverified secondary)
- The portal sandbox includes a "Standardization and Hashing Tool" for checking an implementation against fake data. CalPrivacy publishes no test fixtures or magic identifiers beyond the worked examples. — [Working with the data](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/working-with-data/); [API Evangelist sandbox profile](https://github.com/api-evangelist/california-privacy-protection-agency)

**API operations (three in total)**
- `GET /data/download` behaves as follows:
  - **202** plus `Retry-After` (example 60 s) while the ZIP is being built.
  - **200 application/zip** when ready, with a `Content-Disposition` file name such as `20260312_4821_DROP.zip`.
  - **200 application/json** when there is "No new consumer request data or removed identifiers… since your last completed download."
  - **409**: "Previous download is not complete. Complete the current batch or contact DROP support if a re-download is needed."
  - **403** when the account is ineligible ("Resolve any account, registration, payment, or access issue") or no lists are selected.
  - **429** plus `Retry-After` (30 s example). No numeric rate limit is published.
  
  — [OpenAPI v1.2.0 verbatim copy](https://github.com/api-evangelist/california-privacy-protection-agency)
- `POST /data/upload`: `multipart/form-data`, field name `files`, one or more CSVs (not ZIP). The header must be exactly `Id,Status`, and status codes may only be `2`, `3`, `4` or `5`. The response is **202** with `acceptedCount`, `rejectedCount`, `accepted[]` and `rejected[]`. "Full row-level validation may continue after the response is returned." **409** means "No active download is waiting for responses." — [OpenAPI v1.2.0](https://github.com/api-evangelist/california-privacy-protection-agency)
- `POST /data/amend` takes the same format and corrects statuses already submitted. **409** means "The amend request cannot be processed in the current state." No amendment time window is published. — [OpenAPI v1.2.0](https://github.com/api-evangelist/california-privacy-protection-agency)
- Idempotency: there is no Idempotency-Key header. Re-uploading a file name already accepted for the current download is rejected ("A file with this name was already uploaded for the current download. Use a unique suffix…"). — [API Evangelist conventions profile, quoting API operations page](https://github.com/api-evangelist/california-privacy-protection-agency)
- Optional webhooks (Portal → Notification settings): `download.ready`, `upload.received`, `upload.processed`, `amendment.received`, `amendment.processed`. They are signed with HMAC-SHA256 over `"<X-Webhook-Timestamp>.<raw body>"` in `X-Webhook-Signature: sha256=<hex>`. The docs recommend rejecting timestamps older than 5 minutes. Email notifications to the primary and secondary contacts are always on. — [OpenAPI info block / Reference page, via mirror](https://github.com/api-evangelist/california-privacy-protection-agency)

**Identifier lists, file format, hashing**
- There are six list types: `NDZ` (first name + last name + DOB + ZIP), `Email`, `Phone`, `MAID`, `NameVIN` (first + last name + VIN) and `CTVID`. "Removed is a file type, not a consumer deletion list type." — [OpenAPI v1.2.0](https://github.com/api-evangelist/california-privacy-protection-agency); [Superset](https://www.trustsuperset.com/post/what-is-the-california-drop-system)
- File naming is `<YYYYMMDD>_<DataBrokerId(4 digits)>_<DataType>[_<suffix ≤10 alnum>].csv`, for example `20260312_4821_Email.csv` and `20260312_4821_Email_part01.csv`. Download CSV header: `ID,Hash`. A list with no new records still ships with a header-only CSV. The `..._Removed.csv` file adds `ListType`. Upload: `Id,Status`, using the same file name as the download (plus an optional suffix to split a list). — [OpenAPI v1.2.0 / Working with the data via mirror](https://github.com/api-evangelist/california-privacy-protection-agency); [search extract of API reference](https://cppa.ca.gov/orph/drop_tech_api_ref.pdf)
- Work-item IDs are 12-character case-sensitive Base62 strings (`^[A-Za-z0-9]{12}$`), unique across lists and permanently tied to one work item. Hashes are 44 Base64 characters. — [OpenAPI v1.2.0](https://github.com/api-evangelist/california-privacy-protection-agency)
- "There is no option to download raw consumer identifiers from DROP." — [search extract, privacy.ca.gov reference/API PDF](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/reference/)
- After the first completed cycle, each download contains only identifiers new or removed since the previous batch. — [API Evangelist conventions profile](https://github.com/api-evangelist/california-privacy-protection-agency)
- Hashing is **SHA-256 over UTF-8, output Base64**. The standardization rules, verbatim from the OpenAPI description:
  - **Email:** "remove all whitespace, then lowercase. Do not remove dots, plus signs, or other characters."
  - **DOB:** `YYYYMMDD`.
  - **Phone:** "keep digits only, then retain the last 10 digits, or all digits if fewer than 10 remain."
  - **ZIP:** "Keep alphanumeric characters only, For ZIP+4, drop the +4. Convert to lowercase, remove leading zeros, and use the first five characters present."
  - **Names:** "normalize Unicode, lowercase, transliterate supported Greek and Cyrillic characters, fold supported Latin characters to plain ASCII where possible, then keep only letters and digits."
  - **MAID:** hex only, lowercase, must be 32 characters.
  - **VIN:** alphanumeric, lowercase, 17 characters.
  - **CTVID:** alphanumeric, lowercase, 8–32 characters.
  
  — [OpenAPI v1.2.0 verbatim](https://github.com/api-evangelist/california-privacy-protection-agency); [Working with the data](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/working-with-data/)
- Composite hashing for NDZ and NameVIN: "Each field is standardized and hashed first, then the resulting Base64 hashes are concatenated in the required order and hashed again." The order is NDZ = FirstName + LastName + DOB + ZIP and NameVIN = FirstName + LastName + VIN. — [OpenAPI v1.2.0](https://github.com/api-evangelist/california-privacy-protection-agency); [Final regulation text](https://cppa.ca.gov/regulations/pdf/drop_ftr.pdf)
- Published worked examples:

  | Input | Standardized | Hash |
  |---|---|---|
  | `Anna.Smith@Domain.com` | `anna.smith@domain.com` | `KA18MT/ph6IHYjzT9zwETySDQyvSh87YuoSBpOQtkhE=` |
  | `+1(415)555-9317` | `4155559317` | `vGM7y5n+hBXRSEAklhHDPCbysyNgYTmXdMcagGUOY8E=` |
  | `00712345` (ZIP) | `71234` | — |
  | `M1B 1A1` (ZIP) | `m1b1a` | — |
  | NDZ: Danielle Johnson / 1985-07-04 / 91790 | — | final hash `PQOfn1RffEKmqMmNAzDKKaoZCwxWbQZkQzPWmQo9REA=` |

  **All of these were reproduced exactly in this session** with Python `hashlib` + `base64`. — [Working with the data examples, reproduced in mirror](https://github.com/api-evangelist/california-privacy-protection-agency)

**Status codes and cadence**
- Status codes:
  - `2` Exempted: "match found and all personal information is exempt."
  - `3` Deleted: "match found and non-exempt personal information was deleted."
  - `4` Opted out: "multiple consumers are linked to the same identifier and all were opted out of sale or sharing."
  - `5` Not found: "no match found after completing the matching process."
  
  — [OpenAPI v1.2.0](https://github.com/api-evangelist/california-privacy-protection-agency)
- Consumers see a per-broker outcome of Deleted, Opted Out, Exempted or Record Not Found. — [Fenwick](https://www.fenwick.com/insights/publications/dont-drop-ball-upcoming-changes-california-delete-act-five-key-steps-companies)
- Statute (Civ. Code §1798.99.86(c)(1), as amended by SB 361): "Beginning August 1, 2026, a data broker shall access the accessible deletion mechanism … at least once every 45 days." Within 45 days it must also:
  - process all deletion requests and delete all related PI;
  - process unverifiable requests as opt-outs of sale or sharing;
  - "Direct all service providers or contractors associated with the data broker to delete all personal information … related to the consumers making the requests."
  
  — [SB 361 chaptered text (PUBINFO mirror)](https://github.com/aaronjuar-ez/PUBINFO-2025)
- If the automated connection fails, the broker must download manually. If the failure is not due to user error, it must notify CalPrivacy in writing through its DROP account within 45 days (Cal. Code Regs. tit. 11 §7612(b)(1)). — [API Evangelist conventions citing §7612(b)(1)](https://github.com/api-evangelist/california-privacy-protection-agency); [search extract, getting-started guidance](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/)

**Fees and penalties**
- 2026 annual registration fee: **$6,000**, payable by credit card in DROP, plus a processing fee of up to 2.99%. New brokers pay a monthly declining access fee ($6,000 in Jan 2026 down to $500 in Dec 2026). — [Fees and registration page via mirror](https://privacy.ca.gov/drop-for-data-brokers/account-creation-fees-and-annual-registration/)
- The fee rises to **$9,500 for the 2027 registration period** (+$3,500). — [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html) (the exact figure came from a search summary that did not attribute it clearly)
- Penalties: $200/day for failure to register; **$200/day per deletion request** for failure to delete; plus investigation and enforcement costs. — [DROP for data brokers](https://privacy.ca.gov/drop-for-data-brokers/)

**Adoption metrics (CalPrivacy)**
- Consumer sign-ups and broker counts over time:
  - January 2026: 18,000 requests in the first 48 hours ([SD13 press release, Jan 9 2026](https://sd13.senate.ca.gov/news/press-release/january-9-2026/californians-rush-to-take-advantage-nations-strongest-privacy)).
  - February 2026: more than 242,000 Californians had submitted requests ([IAPP](https://iapp.org/news/a/calprivacy-unpacks-drop-updates-on-consumer-participation-upcoming-enforcement)).
  - June 2026: more than 300,000 sign-ups, with registered brokers at "a record high" ([privacy.ca.gov, June 2026](https://privacy.ca.gov/2026/06/privacy-momentum-builds-300000-californians-sign-up-for-drop-as-registered-data-brokers-hit-a-record-high/)).
  - August 2026: more than 500,000 sign-ups and 654 brokers "part of the system." About 25% of brokers had reported processing in the first weeks after Aug 1 ([privacy.ca.gov, Aug 2026](https://privacy.ca.gov/2026/08/half-a-million-californians-have-signed-up-for-drop-to-delete-their-personal-information-from-data-brokers/)).
  - Early October 2026: more than 550,000 sign-ups and more than 650 registered brokers. 99% of consumers had been deleted by at least one broker, and 70% by 100 or more brokers ([privacy.ca.gov DROP FAQ, Oct 2026](http://privacy.ca.gov/2026/10/drop-faq-blog/)).
- An industry guide notes that many consumers submit several emails, so the identifier count is larger than the number of consumers. — [Transcend](https://transcend.io/blog/calprivacy-drop-compliance-guide) (secondary)

### Inferences
- The protocol is fully specified and deterministic, so the DROP-facing client is a small, commoditizable piece of work. The defensible value is on the broker side: connectors, in-warehouse hashing, deletion orchestration, a durable suppression store and audit evidence.
- The 409 rule (no new download until every work item in the open batch has a status) forces a product to **guarantee 100% status coverage** before the next pull. A pipeline that drops rows blocks the broker from DROP, and that can cascade into the 45-day violation clock.
- Production only validates format, not correctness. A broker that hashes wrongly gets silent "5 Not found" results that look compliant. That is a strong selling point for a conformance and testing module.
- The 2026-04 → 2026-07 doc churn (3 versions in 3 months, including a ZIP+4 rule change) means the hashing library must be versioned, and re-hash campaigns must be possible whenever rules change.
- Initial volume: a broker's first download probably holds every request accumulated since Jan 1, 2026 (about 550k consumers, several identifiers each). The first batch could therefore run to millions of rows across lists, and later deltas would be much smaller. This is an inference from the delta semantics and sign-up counts. The actual per-broker row counts were not found.

### Gaps
- It was not possible to read the privacy.ca.gov pages directly. Not confirmed: whether the 45-day clock runs from download or from the request date, and whether the portal enforces a maximum batch size or upload size.
- No CalPrivacy statement was found on **whether a third-party vendor may hold a broker's API key and call DROP on its behalf**. TrustArc says third-party platforms "are not permitted to access DROP directly on a broker's behalf" ([TrustArc](https://trustarc.com/resource/california-delete-act-drop-platform-data-brokers/)), while DataGrail and Ketch market automated DROP processing. This is a **critical architecture question**. Check the DROP Terms of Use and the Portal user/role model (for example, whether a vendor can be added as a user) before designing a hosted product.
- Status of **AB 883** (Lowenthal) and **SB 1106** (Cabaldon, introduced 2026-02-13), both of which would shorten the 45-day cadence to **30 days**, is unknown. AB 883 was last seen amended in the Senate on 2026-06-17 and also adds elected-official/judge deletion lists, operative 2027-07-01. Its enactment status after the Sept 30, 2026 signing deadline was not verified. — [AB 883 and SB 1106 text via PUBINFO mirror](https://github.com/aaronjuar-ez/PUBINFO-2025); bill pages: [leginfo AB 883](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260AB883), [leginfo SB 1106](https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB1106) (URLs built to the standard leginfo pattern, not fetched)

## 2. Matching standards, partial matches, suppression, service providers and contractors

### Takeaway
The final regulations dropped the proposed ">50% of identifiers" fuzzy match in favor of a **100% match**. Composite hashing makes this structural: NDZ and NameVIN match only if every component standardizes identically. Brokers must:
- keep non-matching DROP identifiers and screen future collection against them (de facto suppression);
- re-delete every 45 days and never sell new PI of deleted consumers;
- opt out every consumer sharing a matched identifier;
- direct service providers and contractors to delete, sharing only the minimum data needed.

### Cited Findings
- The proposed rules let a broker find a match if "more than 50% of the unique identifiers match with the same consumer record." The Agency later "removed the 50% match rate threshold … and set it to 100% to ensure a more precise match and reduce the likelihood of erroneous deletions." — [FSOR 15-day](https://cppa.ca.gov/regulations/pdf/drop_fsor_15day.pdf); [Final Statement of Reasons](https://cppa.ca.gov/regulations/pdf/drop_fosr.pdf); [Troutman analysis, Dec 2025](https://www.troutmanprivacy.com/2025/12/analyzing-the-california-delete-act-regulations/)
- "Multiple identifiers must be individually hashed, combined into one identifier, and then hashed once more." Later revisions convert non-English characters to the closest English characters and add instructions for DOB, ZIP and phone. — [FSOR 15-day](https://cppa.ca.gov/regulations/pdf/drop_fsor_15day.pdf); [proposed text, Sept 2025 board](https://www.cppa.ca.gov/meetings/materials/20250926_item6_prop_text.pdf)
- Brokers only need to standardize PI "for purposes of matching to consumer deletion lists and providing that information to service providers and contractors." They "may maintain the data in other formats for other purposes." — [FSOR 15-day](https://cppa.ca.gov/regulations/pdf/drop_fsor_15day.pdf)
- §7613(a)(2)(B) and §7614(b)(2)(B) "require data brokers to opt out consumers of the sale or sharing of their personal information if there are multiple matches with a given identifier." — [FSOR 15-day](https://cppa.ca.gov/regulations/pdf/drop_fsor_15day.pdf)
- **Retain non-matches and re-screen:**
  - "Data brokers must maintain the consumer identifier information provided by the Agency through the DROP when the information does not match with any of their existing consumer records."
  - If a later-collected record matches (§7613(c)), "the data broker must report the new status … in the next access session following the match."
  
  — [FSOR / Kelley Drye summary](https://www.kelleydrye.com/viewpoints/blogs/ad-law-access/getting-ready-to-use-the-drop); [Final Statement of Reasons](https://cppa.ca.gov/regulations/pdf/drop_fosr.pdf)
- **Statutory suppression (§1798.99.86(d)):** after deleting, "the data broker shall delete all personal information of the consumer at least once every 45 days … unless the consumer requests otherwise." It "shall not sell or share new personal information of the consumer unless the consumer requests otherwise or … permitted under Section 1798.145 or 1798.146." Exempt-retained PI "shall only be used for the purposes described … and shall not be used or disclosed for any other purpose, including … marketing." — [SB 361 chaptered text (PUBINFO mirror)](https://github.com/aaronjuar-ez/PUBINFO-2025)
- **Service providers and contractors:**
  - "The Delete Act does not contain a provision treating contractors and service providers as separate entities from the data broker for the purposes of the delete request."
  - "Data brokers must direct their service providers and contractors to delete records associated with a matched identifier … data brokers must also report the status of deletion requests."
  - A 2025 draft "allow[s] data brokers to forward suppression lists to service providers and contractors," and the final rule reportedly allows sharing "the minimum personal information necessary."
  
  — [FSOR 15-day](https://cppa.ca.gov/regulations/pdf/drop_fsor_15day.pdf); [Fox Rothschild](https://dataprivacy.foxrothschild.com/2025/09/articles/united-states/state-privacy-laws/what-the-cppa-has-to-say-about-the-delete-act-and-the-drop/); [NatLawReview](https://natlawreview.com/article/californias-new-delete-request-tool-impacts-data-brokers-and-residents)
- Consumer cancellations: since doc v1.1.0, identifiers that consumers withdraw arrive in a `Removed` CSV (`ID,Hash,ListType`). — [Reference changelog via mirror](https://github.com/api-evangelist/california-privacy-protection-agency)
- A rulemaking commenter argued that hashed identifiers can be reverse-engineered to link data. The agency responded in its FSOR appendix. Hashing here is data minimization, not anonymization. — [Draft FSOR Appendix A](https://www.cppa.ca.gov/meetings/materials/20250926_item6_fsor_draft_app_a.pdf)

### Inferences
- **Partial matches are invisible by design.** Take a consumer whose stored ZIP differs from the one they gave DROP. The NDZ composite will not match, and the broker correctly reports "5". A broker that keeps historical addresses could hash every (name, DOB, ZIP-variant) combination it holds to catch more matches. That is a plausible product differentiator ("variant expansion"), but whether regulators expect it is **an open legal question**.
- A suppression store is effectively mandatory. It needs three properties:
  1. Every DROP hash, matched and unmatched, kept persistently (minus Removed cancellations).
  2. Screening of new data at ingest (hash on arrival, compare, then block, delete and report a new status at the next session).
  3. A periodic re-delete every ≤45 days for previously deleted consumers.
  
  This is the "sticky" recurring workload that justifies SaaS pricing.
- Downstream notices to service providers and contractors need their own evidence trail: what was sent, when, which hashes or minimum PI, and the acknowledgement. Auditors will likely ask for it (see §3).
- Standardization traps a product should test against the official examples:
  - ZIP codes with leading zeros (`02139` becomes `2139`);
  - Canadian postal codes;
  - email "remove all whitespace" versus trimming only the ends;
  - Greek and Cyrillic transliteration in names;
  - dots kept in Gmail addresses;
  - phone numbers with fewer than 10 digits.
  
  The open-source Ozvel hasher, for example, trims email only at the ends and documents that it lacks Greek/Cyrillic transliteration. That small divergence would produce misses. — [Ozvel/california-DROP drop_hash.py](https://github.com/Ozvel/california-DROP)

### Gaps
- The final codified text of §§7610–7616 could not be retrieved. Section numbers come from the FSOR and secondary summaries. Not confirmed: whether the regulations set an explicit **record-retention period for DROP processing records**, or require logging of service-provider notices.
- Exactly how "exempt" (status 2) must be documented per item (which exemption applies) was not found.
- Whether brokers must re-screen **historical** data when hashing rules change (for example, the ZIP+4 clarification in v1.2.0) was not found.

## 3. The 2028 independent audit, record-keeping and metrics reporting

### Takeaway
The statute requires a third-party audit starting **Jan 1, 2028 and every 3 years**. Reports go to CalPrivacy within 5 business days of request and are kept for 6 years. Draft regulations (in formal rulemaking since Aug 2026) would:
- require a "qualified, objective, and independent" external auditor (no internal auditors, no size threshold);
- bar findings based mainly on attestations or policy review;
- require independent verification of nine components (list selection, hashing, matching, actioning and suppression among them) through system testing and interviews;
- reportedly make the first report due **Nov 1, 2028**, covering activity **from Aug 1, 2026**.

So evidence a broker generates today will be audited.

### Cited Findings
- Statute §1798.99.86(e):
  - "(1) Beginning January 1, 2028, and every three years thereafter, a data broker shall undergo an audit by an independent third party to determine compliance with this section."
  - "(2) … submit a report resulting from the audit and any related materials to the [CPPA] within five business days of a written request."
  - "(3) … maintain the report and materials … for at least six years."
  
  — [SB 361 chaptered text (PUBINFO mirror)](https://github.com/aaronjuar-ez/PUBINFO-2025)
- Preliminary comments on audits ran from Apr 7 to May 7, 2026. They covered:
  - how brokers "may properly demonstrate that they have processed deletion requests";
  - what makes an auditor qualified and independent;
  - what methods and tools to require;
  - what materials to submit.
  
  — [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/the-delete-act-calprivacy-seeks-input-on-data-broker-audit-requirements-102mqe8); [MoFo, May 2026](https://www.mofo.com/resources/insights/260504-data-broker-audits-are-coming); [CPPA preliminary audit document](https://www.cppa.ca.gov/regulations/pdf/drop_audits.pdf)
- In August 2026 the Board launched **formal rulemaking** with a 45-day comment period. The draft includes:
  - criteria for a "qualified, objective, and independent auditor";
  - audit components covering "processes and policies reviews; deletion system testing; and in-person interviews with relevant DROP compliance personnel";
  - a ban on auditors "basing their findings primarily on assertions, attestations, or a review of policies and procedures alone";
  - a requirement that auditors "consider and independently verify nine essential components," including deletion list selection, hashing, matching, actioning and suppression lists;
  - no internal auditors and no size threshold.
  
  — [Freshfields, "DROP is Live"](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/drop-is-live-what-data-brokers-need-to-know-as-calprivacy-ramps-up-oversight-102nqhf); [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html); [Alston & Bird, Aug 2026](https://www.alston.com/en/insights/publications/2026/08/california-privacy-opt-out-signals-data-brokers)
- Auditors are expected to examine "data deletion logs and status reports." The proposed scope reportedly covers "policies and procedures, system logs, matching methodologies, deletion records, suppression lists, and reporting activity." — [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [Captain Compliance](https://captaincompliance.com/education/calprivacy-seeks-stakeholder-feedback-on-drop-audits-for-data-brokers/) (secondary)
- **Conflict on the first deadline:**
  - First reports due **Nov 1, 2028**, covering a period beginning **Aug 1, 2026** (rulemaking summary). — [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html) / [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/drop-is-live-what-data-brokers-need-to-know-as-calprivacy-ramps-up-oversight-102nqhf)
  - First results due to CalPrivacy by **Jan 1, 2029**. — [Clark Hill](https://www.clarkhill.com/news-events/news/is-your-business-a-data-broker-californias-drop-goes-live-and-calprivacy-continues-to-enforce-delete-act/)
- Once a formal notice is published, the agency has one year to submit the regulation to the Office of Administrative Law (OAL). — [search summary of CPPA rulemaking materials](https://www.cppa.ca.gov/regulations)
- EPIC urged CalPrivacy to require independent testing and inspection, not paper reviews. — [EPIC](https://epic.org/epic-encourages-calprivacy-to-enact-independent-testing-and-inspection-requirements-for-data-broker-audits/)
- **Metrics:**
  - By July 1 each year, brokers must compile and disclose in their privacy policies metrics on CCPA requests, including DROP deletion requests, received and responded to in the prior calendar year. — [Fenwick](https://www.fenwick.com/insights/publications/dont-drop-ball-upcoming-changes-california-delete-act-five-key-steps-companies); [DWT](https://www.dwt.com/blogs/privacy--security-law-blog/2023/10/california-delete-act-consumer-data-privacy) (summaries differ on scope)
  - The public registry already carries each broker's prior-year metrics for five request types (delete, know collected, know sold/shared, opt-out, limit sensitive PI): received, complied in whole, complied in part, denied, and mean and median days to respond. — [delistmydata registry snapshot README](https://github.com/delistmydata/ca-data-broker-registry); [CPPA registry](https://cppa.ca.gov/data_broker_registry/)

### Inferences
- **The audit-evidence pack is the clearest MVP wedge for small brokers.** Its contents should map to the nine components:
  - list-selection rationale tied to the SB 361 registration answers;
  - versioned hashing code and conformance results against the official vectors;
  - match logs per batch;
  - per-system deletion evidence;
  - service-provider and contractor notices with acknowledgements;
  - suppression-store state and screening hits;
  - upload receipts and the async validation emails or webhooks;
  - 45-day access history;
  - an outage notice log for §7612(b)(1).
  
  All of it would be retained for at least 6 years, because the statute requires keeping audit materials for 6 years.
- The audit period reportedly starts Aug 1, 2026, so brokers that lack logs for Aug–Dec 2026 will already have evidence gaps. That supports "start logging now" urgency messaging in Q4 2026.
- Auditors (likely CPA firms and privacy-assurance consultancies) are a potential **channel**. An engine that exports auditor-ready evidence in a standard format could become the de facto tool auditors recommend.

### Gaps
- The formal draft audit regulation text and its nine components were not available verbatim. Auditor qualification criteria (for example, certifications such as CPA, CIPP or ISO) were not found.
- No CalPrivacy-specified retention period for **DROP processing records** themselves was found, separate from the 6-year audit report retention. The general CCPA rule on keeping consumer-request records (believed to be 24 months under Cal. Code Regs. tit. 11 §7101) was **not verified in this session**.
- Exact metric definitions under Civ. Code §1798.99.85, and how DROP statuses map to "complied/denied," were not verified in primary text.
- Whether the Oct 2026 Board meeting finalized or modified the audit draft is unknown.

## 4. Build feasibility: MVP components, open-source references, security, effort

### Takeaway
Technically, an MVP is very feasible for a small team. The DROP side is three endpoints with published test vectors, and hashing is about 100 lines of code. The real build is:
- warehouse and DB connectors that hash inside the customer environment;
- a durable suppression store with ingest screening;
- deletion and service-provider orchestration;
- an append-only audit log;
- a metrics reporter.

Open-source projects exist only as hashing kits and hobby tools. Commercial incumbents (DataGrail, Ketch, Transcend, OneTrust, TrustArc) target larger customers, and at least one niche entrant (DropClerk) already targets small brokers with a local-hashing model.

### Cited Findings
- **Open-source references (all small, zero stars as of Oct 2026):**
  - **Ozvel/california-DROP** (created 2026-06-05, updated 2026-07-03) has DROP hashing in Python, JavaScript, Java, Go, PHP and C#, plus per-list JSON test cases. Its README notes that Greek/Cyrillic transliteration is not implemented. — [Ozvel/california-DROP](https://github.com/Ozvel/california-DROP)
  - **ericthomson13/delete-me** is an "Open-source CCPA/state-DSAR/GDPR deletion-letter generator + sender with California DROP compliance auditing for data brokers" (Python, 20 open issues, updated 2026-10-06). — [GitHub](https://github.com/ericthomson13/delete-me)
  - **samsrose/drop-cockpit** is a consumer-side "DROP privacy exposure dashboard." — [GitHub](https://github.com/samsrose/drop-cockpit)
  - **API Evangelist** keeps a verbatim OpenAPI copy, a derived conventions, error, sandbox and webhook profile, and a process-deletion "agent skill." — [api-evangelist/california-privacy-protection-agency](https://github.com/api-evangelist/california-privacy-protection-agency)
- **Commercial landscape:**
  - **DataGrail:** a "Data Broker Compliance" product "purpose-built for the DROP batch process," whose API "supports bulk request processing." — [DataGrail DROP solution](https://www.datagrail.io/solutions/drop-compliance/)
  - **Ketch:** automates "matching against consumer records, executing deletion across hundreds of connected systems through a pre-built integration library, and generating the identity-linked audit trail." — [Ketch](https://www.ketch.com/blog/posts/california-drop-platform-data-broker-compliance)
  - **Engineering guides from other platforms:** [Transcend](https://transcend.io/blog/calprivacy-drop-compliance-guide), [OneTrust](https://www.onetrust.com/blog/californias-drop-what-the-delete-act-changes-for-consent-preferences-and-data-deletion/), [TrustArc](https://trustarc.com/resource/california-delete-act-drop-platform-data-brokers/), [Clym](https://www.clym.io/blog/california-drop-compliance-data-brokers), [Sentra](https://sentra.io/blog/automating-ccpa-drop-compliance).
  - **Optacy** sells a "California DROP Act" product. — [Optacy](https://optacy.com/product/the-california-drop-act/)
  - **DropClerk** ("DROP deletion cycles for California data brokers") uses a browser-based approach that "hashes your records, matches them against those lists, and sends back only the state's own work item ids, each with a status digit." — [DropClerk](https://dropclerk.com/) (pricing not retrieved)
- TrustArc states that third-party platforms "are not permitted to access DROP directly on a broker's behalf." This conflicts with vendor automation claims and remains unresolved (see §1 Gaps). — [TrustArc](https://trustarc.com/resource/california-delete-act-drop-platform-data-brokers/)
- The API has no SDKs, CLI, status page or deprecation policy. Azure Front Door and Cloudflare edge headers are observed. DROP support asks for the timestamp (Pacific Time), endpoint, HTTP status, file name and payload. — [API Evangelist conventions profile](https://github.com/api-evangelist/california-privacy-protection-agency)
- The docs advise keeping API keys in environment variables or a secret manager, and regenerating them if compromised or when the list selection changes. — [Getting started (search extract)](https://privacy.ca.gov/drop-for-data-brokers/technical-specifications/getting-started/)
- The rulemaking record flags reverse-engineering risk for hashed identifiers. — [Draft FSOR Appendix A](https://www.cppa.ca.gov/meetings/materials/20250926_item6_fsor_draft_app_a.pdf)

### Inferences
**Proposed MVP components, with rough engineering estimates for 1–2 senior engineers.** No source gave effort estimates, so these are the researcher's estimates.
1. **DROP client** (≈1–2 weeks):
   - download polling with 202/Retry-After;
   - 409 handling and ZIP/CSV parsing;
   - Removed-file handling;
   - upload with suffix-splitting, plus treating a "duplicate filename" rejection as already accepted;
   - amend;
   - HMAC webhook receiver;
   - a 45-day scheduler with escalating alerts;
   - support for both sandbox and production keys.
2. **Standardization and hashing library** (≈1–2 weeks):
   - all 8 field rules plus composites;
   - Unicode NFKD folding and Greek/Cyrillic transliteration;
   - a conformance suite seeded with the official vectors;
   - versioning per doc release (1.0 → 1.2).
3. **Connectors, hashing in place** (≈1 week each for Postgres, Snowflake, BigQuery, and CSV/S3 upload). Push SQL down so hashing runs where the data lives and raw PII never leaves the broker. For example, Snowflake `BASE64_ENCODE(SHA2_BINARY(x,256))`, BigQuery `TO_BASE64(SHA256(x))` and Postgres `encode(sha256(convert_to(x,'UTF8')),'base64')`. These function names come from general knowledge and were not verified in this session. Standardization logic (transliteration in particular) is hard to express in SQL, so a hybrid approach (UDFs, or an agent container running in the customer's VPC) is likely.
4. **Matching and decisioning** (≈1 week): exact hash join per list; multi-consumer detection leading to status 4; an exemption tagging workflow leading to status 2; guaranteed coverage so every work item gets a status.
5. **Deletion orchestration** (≈2–3 weeks): generate deletion jobs or SQL per system; produce service-provider and contractor notice packets (minimum PI or hashes) with acknowledgement tracking; schedule the 45-day re-delete.
6. **Suppression store** (≈1 week): persistent hash sets per list; an ingest-screening API or SQL view; Removed-list un-suppression; new-match detection that triggers a status update in the next session.
7. **Audit log and evidence pack** (≈2 weeks): append-only, hash-chained event log; per-batch reports; 6-year retention; export organized around the nine audit components.
8. **Metrics reporter** (≈0.5 week): yearly counts in the registry's format (received, complied whole or part, denied, mean and median days).

In total that is roughly **10–14 engineer-weeks to a credible MVP**, plus hardening and security.

**Architecture and security:**
- Prefer a **"broker-run agent / bring-your-own-key"** design. The broker's DROP key stays in the broker's environment, and the SaaS control plane sees only work-item IDs, statuses and hashes (or nothing). This sidesteps the unresolved vendor-access question and reduces PII exposure, which matters because hashed identifiers are reversible by dictionary attack.
- SOC 2 Type II will likely be expected by mid-size brokers and enterprise data buyers. No source on DROP-specific security expectations was found. Small brokers may accept a SOC 2 roadmap if no raw PII touches the vendor.

**Differentiation for small brokers:**
- a hashing conformance test, i.e. "are you silently reporting Not Found?";
- historical-variant expansion (with legal caveat);
- audit-ready evidence from day 1;
- low-touch CSV/warehouse onboarding;
- fixed pricing, compared with DataGrail- or Ketch-style platforms.

### Gaps
- No published build-effort benchmarks, case studies or customer counts for DROP vendors were found.
- No SOC 2 or security-questionnaire requirements specific to DROP were found.
- DropClerk's pricing, customer count and team were not retrieved.
- Superset's and Optacy's offerings were not verified in detail.

## 5. Go-to-market: reaching brokers, channels, pricing models, launch timeline

### Takeaway
The target list is public and downloadable. The CPPA registry CSV gives about 603–654 brokers with websites, contact emails and prior-year request metrics. About half of brokers handled fewer than 100 deletion requests in 2024, so they have no DSR tooling scaled for DROP's 550k+ consumer lists. That is the ideal small-broker segment.

Channels:
- the many law firms that have published DROP alerts;
- privacy consultancies;
- future auditors.

Comparable privacy-ops platforms cost **$30–60k/yr** (DataGrail, via Vendr), and the state fee alone is $9,500 in 2027. That leaves room for a $5–25k/yr small-broker tier. The timeline has natural triggers:
- now (processing is live and most brokers lagged);
- the January 2027 registration window;
- July 1, 2027 metrics;
- the 2028 audit.

### Cited Findings
**Registry as a lead list**
- The CPPA registry page offers a "Download CSV" (registry.csv). Archive files include registry2024.csv, registry2025.csv and complete-reg-data-brokers.csv. — [CPPA Data Broker Registry](https://cppa.ca.gov/data_broker_registry/); [dev.to: Parsing California's data broker registry CSV](https://dev.to/edwardfancher/parsing-californias-data-broker-registry-csv-28gc); [API Evangelist llms.txt](https://github.com/api-evangelist/california-privacy-protection-agency)
- Counts:
  - 545 registered brokers as of Jan 1, 2026 ([Wikipedia](https://en.wikipedia.org/wiki/Delete_Act)).
  - 603 in the Sept 1, 2026 CSV snapshot ([delistmydata snapshot](https://github.com/delistmydata/ca-data-broker-registry); [Medium analysis](https://medium.com/@delistmydata/what-603-data-brokers-told-california-about-deleting-your-data-1e1741b49766)).
  - 654 "part of the system" (Aug 2026) and more than 650 registered (Oct 2026), per CalPrivacy ([Aug release](https://privacy.ca.gov/2026/08/half-a-million-californians-have-signed-up-for-drop-to-delete-their-personal-information-from-data-brokers/); [Oct FAQ](http://privacy.ca.gov/2026/10/drop-faq-blog/)).
- **Researcher analysis of the Sept 1, 2026 snapshot CSV** (603 rows × 77 columns):
  - **Contacts:** all 603 rows list a website and a contact email. 354 (about 59%) are role-based privacy, legal or compliance inboxes (privacy@, legal@ and so on). In 134 rows the contact-email domain differs from the website domain. One domain (ignitevisibility.com) is the contact for 5 registrants, suggesting outsourced compliance contacts.
  - **2024 deletion requests received** (602 brokers reporting): 163 reported zero; **295 (49%) fewer than 100**; **414 (69%) fewer than 1,000**; 120 (20%) 10,000 or more; median 107.
  
  — [delistmydata/ca-data-broker-registry CSV](https://github.com/delistmydata/ca-data-broker-registry)
- Registry geography: CA 126, NY 84, FL 48, TX 32, IL 32, MA 29, VA 23, GA 21. By country, 564 US, 12 UK and 10 Canada. — [delistmydata README](https://github.com/delistmydata/ca-data-broker-registry)
- Registration runs Jan 1–31 each year. In 2026 it applies to "more businesses than ever." — [GT Data Privacy Dish, Jan 2026](https://www.gtlaw-dataprivacydish.com/2026/01/california-data-broker-registration-deadline-arrives-jan-31-applying-to-more-businesses-than-ever/); [CalPrivacy on X](https://x.com/CalPrivacy/status/2006780459661897788)
- **Enforcement pressure:**
  - Jan 2026 "New Round of Enforcement Actions Against Data Brokers." — [CPPA announcement 2026-01-08](https://cppa.ca.gov/announcements/2026/20260108.html)
  - A DROP enforcement advisory and FAQs carry "Another Clear Warning to Data Brokers." — [Nelson Mullins](https://www.nelsonmullins.com/insights/alerts/privacy_and_data_security_alert/all/calprivacy-drops-latest-drop-enforcement-advisory-faqs-and-another-clear-warning-to-data-brokers)
  - Regulations and enforcement suggest more companies qualify as brokers. — [MoFo, Jan 2026](https://www.mofo.com/resources/insights/260115-think-you-re-not-a-data-broker-calprivacy-regulations)
  - A Stanford study found brokers not following the law. — [Stanford HAI](https://hai.stanford.edu/news/companies-that-buy-and-sell-your-data-are-not-following-californias-strict-privacy-laws)

**Channels**
- **Law firms that published DROP and Delete Act guidance in 2025–26** (candidate referral partners): Kelley Drye, Troutman, Freshfields, MoFo, WSGR, Fenwick, Alston & Bird, Nelson Mullins, Clark Hill, Coblentz, Greenberg Traurig, Hunton, Benesch, Fox Rothschild, Wiley, Covington, Davis Wright Tremaine and Bryan Cave (Byte Back). — [Kelley Drye](https://www.kelleydrye.com/viewpoints/blogs/ad-law-access/getting-ready-to-use-the-drop); [Troutman](https://www.troutmanprivacy.com/2025/12/analyzing-the-california-delete-act-regulations/); [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/drop-is-live-what-data-brokers-need-to-know-as-calprivacy-ramps-up-oversight-102nqhf); [MoFo](https://www.mofo.com/resources/insights/260504-data-broker-audits-are-coming); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html); [Fenwick](https://www.fenwick.com/insights/publications/dont-drop-ball-upcoming-changes-california-delete-act-five-key-steps-companies); [Alston](https://www.alstonprivacy.com/drop-is-coming-due-what-californias-delete-act-means-for-data-brokers-in-august/); [Nelson Mullins](https://www.nelsonmullins.com/insights/alerts/privacy_and_data_security_alert/all/calprivacy-drops-latest-drop-enforcement-advisory-faqs-and-another-clear-warning-to-data-brokers); [Clark Hill](https://www.clarkhill.com/news-events/news/is-your-business-a-data-broker-californias-drop-goes-live-and-calprivacy-continues-to-enforce-delete-act/); [Coblentz](https://www.coblentzlaw.com/news/navigating-californias-data-broker-requirements-in-2026/); [GT](https://www.gtlaw-dataprivacydish.com/2026/01/california-data-broker-registration-deadline-arrives-jan-31-applying-to-more-businesses-than-ever/); [Hunton](https://www.hunton.com/insights/publications/signed-sealed-deleted-a-look-at-the-california-delete-act); [Benesch](https://www.beneschlaw.com/insight/the-era-of-centralized-deletion-is-here-understanding-calprivacys-drop-platform-before-2026/); [Fox Rothschild](https://dataprivacy.foxrothschild.com/2025/09/articles/united-states/state-privacy-laws/what-the-cppa-has-to-say-about-the-delete-act-and-the-drop/); [Wiley](https://www.wileyconnect.com/sb-361-defending-californians-act-expanding-requirements-for-data-brokers); [Covington](https://www.insideprivacy.com/privacy-data-security/california-amends-data-broker-law/); [DWT](https://www.dwt.com/blogs/privacy--security-law-blog/2023/10/california-delete-act-consumer-data-privacy); [Byte Back](https://www.bytebacklaw.com/2026/10/is-your-business-model-subject-to-data-broker-laws/)
- **Privacy consultancies and boutiques active on DROP** (candidate resellers): In-House Privacy (DROP FAQ; filed rulemaking comments), Captain Compliance and Optacy. — [In-House Privacy FAQ](https://www.inhouseprivacy.com/blog/california-drop-faq); [In-House Privacy comments](https://www.inhouseprivacy.com/blog/in-house-privacys-comments-to-the-cppa-re-sb-362-delete-act-rulemaking-on-the-subject-of-the-accessible-deletion-mechanism); [Captain Compliance](https://captaincompliance.com/education/calprivacy-seeks-stakeholder-feedback-on-drop-audits-for-data-brokers/); [Optacy](https://optacy.com/product/the-california-drop-act/)
- The California Lawyers Association privacy section is publishing "you may be a data broker" content. — [CLA](https://calawyers.org/privacy-law/wake-now-discover-that-you-are-a-data-broker/)

**Pricing comparables**
- DataGrail (per Vendr's purchase data): small and mid-market deployments (<1M data subjects, <500 DSARs/yr, 10–20 integrations) commonly cost **$30k–$60k/yr**. The median is **$50k/yr** across 71 purchases. Pricing is modular by data-subject volume, request needs and modules, and multi-year terms give 15–25% discounts. — [Vendr DataGrail](https://www.vendr.com/marketplace/datagrail)
- Transcend publishes no pricing. Osano's consent product has a free tier and a paid plan from $199/month, while DSAR and the broader platform go through sales. Both figures come from a search summary of comparison sites, not verified on vendor pages. — [Enzuzo Osano alternatives](https://www.enzuzo.com/blog/osano-competitors-alternatives); [Usercentrics](https://usercentrics.com/knowledge-hub/osano-competitors/)
- Consumer-side removal services such as Optery charge about $3.99–$24.99/month. They are not comparable on the buyer side but are relevant as DROP-adjacent consumer demand. — [Optery pricing](https://www.optery.com/pricing/)
- Value anchors: a $9,500 state fee for 2027 ([IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike)) and $200/day per unprocessed request ([DROP for data brokers](https://privacy.ca.gov/drop-for-data-brokers/)).

**Timeline anchors**
- 2026-01-01: DROP opened to consumers.
- 2026-01-31: registration deadline.
- 2026-04-02: sandbox and docs 1.0 released.
- 2026-07-02: docs 1.2.
- 2026-08-01: processing began.
- About 25% of brokers had reported processing by late Aug 2026.
- Audit period reportedly started 2026-08-01.
- 2028-01-01: statutory audits begin.
- First report proposed for 2028-11-01 (or 2029-01-01, per Clark Hill).

— Sources as cited in §§1 and 3 ([Aug release](https://privacy.ca.gov/2026/08/half-a-million-californians-have-signed-up-for-drop-to-delete-their-personal-information-from-data-brokers/); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html))

### Inferences
- **The ideal customer:** brokers with fewer than 1,000 deletion requests a year before DROP (about 69% of registrants, roughly 400–450 companies), no in-house privacy engineering, and data in Postgres, Snowflake, BigQuery or flat files. They now face hundreds of thousands of hashed identifiers per list and a 45-day clock. Large brokers (about 120 with 10k+ requests) are DataGrail, Ketch and OneTrust territory.
- **Rough addressable market (researcher estimate):** about 450 small brokers × $6–15k/yr ≈ $3–7M ARR in California alone. That is a niche, bootstrappable business unless it expands across states (see §6) or adjacent workflows (state registrations, DSARs, opt-out signals).
- **Pricing model suggestion:**
  - flat annual tiers keyed to selected list types and record volume (for example, Starter for CSV upload with 1–2 lists, Growth for warehouse connectors with all lists, Audit+ for the evidence pack, SP-notice tracking and auditor export);
  - an optional per-batch managed service for brokers that want a "done-for-you" cycle;
  - no per-request pricing, because DROP volume is driven by the state, not by the broker's activity, and buyers dislike unpredictable costs.
- **Outreach:** the role-based privacy inboxes on the registry are also where consumer requests land. Cold email may be filtered or ignored, so pair it with LinkedIn outreach to named privacy and GC contacts, plus law-firm referrals. CAN-SPAM-compliant B2B email to published business contacts is generally permissible, but confirm with counsel.
- **Plausible launch timeline:**
  - **Q4 2026:** sandbox-validated MVP (CSV + Postgres plus the conformance checker). Lead with a free "hash conformance check" tool and an "Are you 45-day compliant?" checklist, targeting the roughly 75% who were late.
  - **Jan 2027:** registration-window campaign, since brokers renewing at $9,500 are thinking about compliance.
  - **Q1–Q2 2027:** Snowflake and BigQuery connectors, service-provider notice tracking, SOC 2 Type I.
  - **By July 1, 2027:** metrics report feature.
  - **H2 2027:** audit-evidence module aligned to the final audit regulations (OAL deadline about 1 year after the Aug 2026 notice), plus auditor partnerships.
  - **2028:** audit season, and CT expansion ahead of its July 1, 2028 mechanism.

### Gaps
- **Events were not researched** because the search budget ran out: IAPP Global Privacy Summit / IAPP Privacy. Security. Risk., LeadsCon, Lead Generation World, Affiliate Summit East/West, ANA (successor to DMA) events, and any data-industry associations (the user's "ADDA" acronym could not be resolved). No 2026–2027 dates or locations have been verified. Trade associations representing brokers (for example, ANA/DMA, the Consumer Data Industry Association, IAB) were not verified as channels.
- No public reseller programs from privacy consultancies were found. DropClerk pricing, and any published DROP-specific SKU prices from DataGrail, Ketch, Transcend, TrustArc or OneTrust, were not found.
- Whether CalPrivacy publishes a list of brokers that have or have not accessed DROP, which would be a strong lead signal, is unknown.
- The terms of use for the registry CSV (commercial outreach use) were not checked. It is a public record, per the snapshot README's note.

## 6. Expansion: other state broker registries and centralized deletion mechanisms

### Takeaway
California's DROP is the only live one-stop deletion mechanism as of Oct 2026. The most concrete next market is **Connecticut** (SB 4 / Public Act 26-64), which creates a registry, requires registration from Jan 1, 2027, and requires a centralized deletion mechanism by **July 1, 2028**. Vermont reportedly directed its Secretary of State to build a universal deletion mechanism in a June 2026 amendment (this is disputed). New York S9088 (single deletion request) is pending. Texas and Oregon have registries without deletion platforms, and New Jersey's registry provision is effective around March 2027. A state-agnostic engine (pluggable list formats, hashing profiles and cadences) is a sound architectural bet.

### Cited Findings
- **Connecticut:** SB 4 / Public Act 26-64 creates a Department of Consumer Protection data broker registry and accessible deletion mechanism. Brokers may not sell or license brokered personal data on or after Jan 1, 2027 unless registered. The mechanism must launch by **July 1, 2028**, and fees are $2,500 (initial and renewal). — [Pandectes 2026 guide](https://pandectes.io/blog/data-broker-compliance-in-2026-a-guide-to-california-connecticut-new-jersey-and-beyond/) (attribution from a search summary; verify against the enacted Public Act)
- **Vermont:** amended its broker law on **June 16, 2026**, adding breach-notification and annual-registration changes effective Jan 1, 2027, and directing the Secretary of State to develop a universal deletion mechanism. — [Privacy & Data Security Insight, "Just DROPped," Aug 2026](https://www.privacyanddatasecurityinsight.com/2026/08/just-dropped-a-data-broker-law-update/); **contradicted by** a source listing Vermont's deletion tool as under study (H.211, not enacted): [TraceKill](https://tracekill.com/blog/data-broker-deletion-rights-by-state) / [PrivacyOn](https://www.privacyon.com/blog/us-state-privacy-laws-in-effect-2026-data-broker-rights)
- **Texas and Oregon:** public broker registries but no one-stop deletion tool. Texas requires a conspicuous website notice. Oregon's registration must state whether and how Oregon residents can opt out. — [PrivacyLawMap 2026 guide](https://privacylawmap.com/blog/data-broker-registration-requirements-2026); [SecurePrivacy](https://secureprivacy.ai/blog/data-broker-registration)
- **New Jersey:** the registry section stays inoperative for 270 days after enactment, through **March 27, 2027**. The law also restricts selling or licensing sensitive data. No deletion mechanism was found. — [Pandectes](https://pandectes.io/blog/data-broker-compliance-in-2026-a-guide-to-california-connecticut-new-jersey-and-beyond/)
- **New York:** Senate Bill 9088 (introduced Jan 30, 2026; referred to Consumer Protection) would allow a single request to delete PI from all registered brokers. — [DataGuidance](https://www.dataguidance.com/news/new-york-bill-data-brokers-registration-and-data)
- A state-by-state registration tracker exists. — [GSDSI tracker](https://www.gsdsi.com/data-broker-registration-tracker)
- **California itself is changing:** AB 883 (as amended 2026-06-17) and SB 1106 (introduced 2026-02-13) would cut the 45-day cadence to **30 days**. AB 883 would also feed elected-official and judge deletion lists into DROP (operative July 1, 2027). — [PUBINFO bill text mirror](https://github.com/aaronjuar-ez/PUBINFO-2025)

### Inferences
- Design for multi-jurisdiction from day 1: a jurisdiction-specific "list adapter" (formats, hashing profile, cadence, status vocabulary), a single suppression store keyed by jurisdiction, and per-state evidence packs. Connecticut's 2028 launch is the first realistic second integration. It may copy California's hashed-list design, but that is unconfirmed.
- Registration-only states (TX, OR, VT, NJ) offer an adjacent **multi-state registration-management** feature (deadlines, fees, disclosures). This low-tech upsell is useful to the same buyer.
- The cadence could tighten (45 → 30 days) and new list sources could be added (officials and judges), so the scheduler and list-type model should be configurable.

### Gaps
- Nebraska: nothing found. The enacted texts for CT PA 26-64, the Vermont June 2026 amendment and the NJ law were not verified in primary sources.
- Whether Connecticut or Vermont will reuse California's hashing and list spec, or interoperate with DROP, is unknown.
- The status of AB 883, SB 1106 and NY S9088 as of Oct 2026 is unknown.
- A federal centralized-deletion bill (for example, a federal "DELETE Act") was not researched.
