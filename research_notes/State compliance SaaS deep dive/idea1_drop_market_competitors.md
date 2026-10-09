# Idea 1: DROP Fulfillment Engine for Small Registered Data Brokers: Regulation, Market, Competitors, Feasibility (as of 2026-10-09)

> **How these notes were made (read first).** WebFetch failed with DNS errors on every domain tried (cppa.ca.gov, privacy.ca.gov, alston.com, wilmerhale.com, freshfields.com, bytebacklaw.com). The shared WebSearch budget ran out after about 25 queries. **No page could be read in full.** Every finding below comes from search-engine summaries and excerpts of the cited URLs. Search summaries can merge or misattribute details, so treat exact figures as "reported by" the cited page. Re-check the load-bearing ones (marked ⚠) against the primary page before using them in a go/no-go memo. Several planned topics could not be searched at all; they are listed under Gaps.

---

## 1. Regulation: what a registered data broker must do under the Delete Act (SB 362) and the DROP regulations, and when

### Takeaway
Since **Aug 1, 2026**, every registered California data broker must:
- log in to DROP (by UI or API) at least every 45 days and download hashed deletion lists;
- standardize and SHA-256-hash its own records using exact rules, then match;
- delete, opt out, or mark exempt / not found;
- report a status for every request within 45 days;
- push the same deletion to its service providers and contractors;
- keep a suppression list that screens newly acquired data.

From **2028**, independent third-party audits every 3 years will test exactly these steps, and the first audit period reaches back to **Aug 1, 2026**. That creates a durable need for evidence and logging, not just a one-time setup.

### Cited Findings
**Core timeline**
- SB 362 (the Delete Act) was signed in Oct 2023. It requires CPPA to build an "accessible deletion mechanism" so a consumer can send one verifiable request to all registered brokers — [DWT, Oct 2023](https://www.dwt.com/blogs/privacy--security-law-blog/2023/10/california-delete-act-consumer-data-privacy); [CalMatters Digital Democracy, SB 362](https://calmatters.digitaldemocracy.org/bills/ca_202320240sb362)
- The CPPA board approved the final Delete Act / DROP regulations in Nov 2025 — [CPPA announcement 2025-11-13](https://cppa.ca.gov/announcements/2025/20251113.html); DROP system presentation at the [CPPA board meeting of 2025-11-07, item 5](https://cppa.ca.gov/meetings/materials/20251107_item_5_drop_present.pdf)
- DROP opened to consumers on **Jan 1, 2026**. Brokers' processing duty began **Aug 1, 2026** — [CPPA DROP page](https://www.cppa.ca.gov/data_brokers/); [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/californias-new-delete-request-tool-impacts-data-brokers-and-residents); [Byte Back, Feb 2026](https://www.bytebacklaw.com/2026/02/californias-deletion-request-and-opt-out-platform-drop-is-live/)
- ⚠ The first 45-day access window after Aug 1 closed "on or around 15 September" 2026 — [Control D analysis](https://controld.com/blog/data-broker-report/)

**Processing mechanics** (from secondary summaries of the regulation text; the reg text itself was not readable)
- Brokers must access DROP at least once every 45 days, process the deletion requests, and direct all service providers and contractors to delete — [Troutman, Dec 2025](https://www.troutmanprivacy.com/2025/12/analyzing-the-california-delete-act-regulations/); [Troutman Delete Act fact sheet, Mar 2026](https://www.troutmanprivacy.com/wp-content/uploads/sites/941/2026/03/Troutman_PrivacyCyber_CADeleteAct_Final.pdf)
- Brokers must report the status of each request within 45 days of retrieving it — [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/californias-new-delete-request-tool-impacts-data-brokers-and-residents); [CalPrivacy, "Processing DROP requests"](https://privacy.ca.gov/drop-for-data-brokers/process-drop-requests/)
- Unverified requests are treated as opt-outs of sale/sharing. Brokers must keep deleting newly collected data about requesters on the same 45-day cycle — [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/californias-new-delete-request-tool-impacts-data-brokers-and-residents)
- **Hashing:** all consumer identifiers in DROP are SHA-256 hashed. Brokers must standardize each value before hashing, for example dates as 8-digit strings and phones as the last 10 digits with no dashes. Where a list has several identifiers, each one is hashed separately and the hashes are then concatenated into a single identifier. Brokers do not have to store data in this form day to day — [ppc.land](https://ppc.land/california-approves-regulations-for-data-broker-deletion-platform/); [DataGrail DROP page](https://www.datagrail.io/solutions/drop-compliance/); [CalPrivacy DROP Technical & API Reference](https://cppa.ca.gov/orph/drop_tech_api_ref.pdf)
- **Four status codes** per request: "record deleted"; "record opted out of sale" (multiple consumers matched the identifier); "record exempted" (all data falls under exemptions in Civ. Code §1798.99.86); "record not found" — [ppc.land](https://ppc.land/california-approves-regulations-for-data-broker-deletion-platform/)
- **Suppression list:** brokers keep a list of identifiers, for both matched and unmatched records, and compare it against newly collected records before any new data is sold or shared — [CalPrivacy guidance as quoted by UnsubCentral](https://www.unsubcentral.com/california-drop-and-the-delete-act-operational-guide-for-data-brokers/); [Privacy Rights Clearinghouse, Aug 2026](https://privacyrights.org/resources-tools/advocacy/deletion-obligations-under-drop-are-here-data-brokers-must-now-delete)
- **API keys** are generated in the Data Broker Portal and scoped to the deletion lists the broker selects. They should be kept in env vars or a secret manager and regenerated if compromised or if list selection changes. The docs reviewed do not say whether a key may be shared with a vendor — [CalPrivacy DROP Technical & API Reference](https://cppa.ca.gov/orph/drop_tech_api_ref.pdf)
- ⚠ DROP initially distributed lists by CSV/download. Transcend wrote that the "DROP API integration [was] coming in Spring 2026" — [Transcend guide](https://transcend.io/blog/calprivacy-drop-compliance-guide)
- Each legal entity needs its own registration and DROP account. A broker cannot rely on a parent's or affiliate's registration, and all websites and DBAs must be listed — [CPPA Enforcement Advisory 2025-01, Dec 17 2025](https://cppa.ca.gov/pdf/enfadvisory202501.pdf); [CPPA announcement 2025-12-17](https://cppa.ca.gov/announcements/2025/20251217.html)

**Proposed DROP amendments** (Aug 2026 board meeting; not final)
- Brokers would have to screen incoming data against everyone who previously submitted a DROP request, including people with no match at first. "Suppression list" would be defined, along with what may be kept on it — [Alston, Aug 2026](https://www.alston.com/en/insights/publications/2026/08/california-privacy-opt-out-signals-data-brokers); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html)
- Brokers would have to update DROP account contact details within 10 business days of a change. The board started the comment-period clock on these amendments — [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html); [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike)

**Audits** (the statute requires them from Jan 1, 2028; implementing rules are in formal rulemaking as of Aug 2026)
- CalPrivacy took preliminary comments in spring 2026 — [CPPA preliminary comments PDF](https://cppa.ca.gov/regulations/pdf/drop_audits_prelim_comments.pdf); [MoFo, May 2026](https://www.mofo.com/resources/insights/260504-data-broker-audits-are-coming); [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/the-delete-act-calprivacy-seeks-input-on-data-broker-audit-requirements-102mqe8). The NAI trade group filed comments on 2026-05-07 — [NAI comments](https://thenai.org/wp-content/uploads/2026/05/NAI-Preliminary-DROP-Audit-Comments-2026.05.07_FINAL.pdf)
- Proposed rules (formal rulemaking with a 45-day comment period, started after the Aug 6–7, 2026 board meeting):
  - auditors must be independent third parties; internal auditors are not allowed; there is no size threshold;
  - audits every 3 years;
  - ⚠ first audit reports due **Nov 1, 2028**, covering an audit period that starts **Aug 1, 2026**;
  - auditors cannot rely mainly on attestations or policy review;
  - auditors must independently verify **9 components**: deletion-list selection, DROP access, standardization, hashing, matching, actioning, status reporting, suppression list, and service providers/contractors;
  - expected evidence includes system logs, hashing evidence, deletion commands, status reports and personnel interviews.
  - Sources: [Freshfields, "DROP is Live"](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/drop-is-live-what-data-brokers-need-to-know-as-calprivacy-ramps-up-oversight-102nqhf); [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html)

**Registration, metrics and fees**
- Annual registration is due by **Jan 31** for the prior year's broker activity. LocateSmarter was a broker in 2025 and had to register by Jan 31, 2026 — [Paul Weiss, Aug 2026](https://www.paulweiss.com/insights/client-memos/california-privacy-protection-agency-s-first-enforcement-action-against-data-broker-signals-industry-scrutiny)
- 2026 fee: **$6,000**, plus an electronic-payment processing fee of up to 2.99% — [CalPrivacy fees page](https://privacy.ca.gov/drop-for-data-brokers/account-creation-fees-and-annual-registration/); [Henson Legal](https://www.henson-legal.com/newsroom//california-data-broker-registration-lead-generation)
- The board approved a **2027 fee of $9,500** for registration and DROP access (+58%) in Aug 2026, citing residency-verification, infrastructure and staffing costs — [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html)
- ⚠ One summary says the fee is prorated by "just under $792 per month" depending on when a broker's DROP obligations begin. Not verified.
- **Metrics:** each year brokers must compile prior-calendar-year CCPA request counts (received, complied with, denied, plus response-time statistics) and publish them in their privacy policy by **July 1**. The same figures feed the annual registration. Sources differ on mean vs. median days and on the first-year deadline — [DWT](https://www.dwt.com/blogs/privacy--security-law-blog/2023/10/california-delete-act-consumer-data-privacy); [Privacy World](https://www.privacyworld.blog/2023/12/california-delete-act-imposes-new-obligations-on-data-brokers/); [Securiti](https://securiti.ai/privacy-laws/us/california/california-delete-act)
- **Registration disclosures:** the Delete Act already required brokers to say whether they collect minors' data, precise geolocation and reproductive-health data. **SB 361** (signed Oct 8, 2025) adds many more questions:
  - identifier types collected: date of birth, ZIP code, email, phone, government ID numbers, mobile ad IDs, biometrics, citizenship;
  - whether data was sold or shared to foreign adversaries, the federal government, other states or law enforcement.
  - Sources: [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/california-expands-data-broker-registration-requirements); [Troutman, Oct 2025](https://www.troutmanprivacy.com/2025/10/california-amends-data-broker-law/); [Hintze](https://hintzelaw.com/blog/2025/10/13/california-further-amends-its-data-broker-registration-law)

**Penalties**
- **$200 per deletion request per day** of failure to delete, plus investigation and administrative costs — [Troutman fact sheet](https://www.troutmanprivacy.com/wp-content/uploads/sites/941/2026/03/Troutman_PrivacyCyber_CADeleteAct_Final.pdf); [TechTimes, 2026-07-08](https://www.techtimes.com/articles/319927/20260708/california-drop-enforcement-hits-aug-1-data-brokers-face-200-per-day-fines.htm)
- **$200 per day** of failure to register — [CPPA Enforcement Advisory 2025-01](https://cppa.ca.gov/pdf/enfadvisory202501.pdf)
- Under Advisory 2026-01 (Sept 3, 2026), **$200 per day** that *incorrect* registry information stays uncorrected, whether or not the error was intentional — [CalPrivacy advisory PDF](https://privacy.ca.gov/wp-content/uploads/sites/357/2026/09/Enforcement-Advisory-No.-2026-01-Accuracy-of-Data-Broker-Registration-Information.pdf); [CalPrivacy release](https://privacy.ca.gov/2026/09/enforcement-advisory-targets-incorrect-information-in-data-broker-registration/)
- Troutman notes that with more than 500,000 DROP registrants (CalPrivacy figure as of Aug 25, 2026), exposure "could raise … substantially" depending on how many registrants a broker holds data on — [Troutman (via search excerpt)](https://www.troutmanprivacy.com/2025/12/analyzing-the-california-delete-act-regulations/)

### Inferences
- Every registered broker receives **every** DROP requester for the lists it selects, so each cycle it must hash, match and file a status for roughly 500k+ records, even if it holds data on few of them. Doing that by hand in spreadsheets is impractical at this volume. That is the core automation wedge.
- The 9 audit components are effectively a product spec, and the audit period starts Aug 1, 2026. Small brokers who cannot show logs from 2026 onward may fail their first audit (reports due Nov 2028). **Evidence retention from day one** is a concrete selling point.
- Normalization errors fail silently: a mis-standardized value hashes differently and simply never matches. That gives a concrete "correctness" value proposition, and audits will test standardization and hashing specifically.
- The proposed amendments would make suppression-at-ingest mandatory for *all* prior requesters, including no-match records. This moves the obligation from batch cleanup into the broker's data-acquisition pipeline, which is a stickier integration point.

### Gaps
- The final regulation text (Cal. Code Regs. tit. 11, §7600 et seq.) could not be read. Section numbers, retention periods for status and suppression records, and the exact clock definitions (45 days from retrieval vs. from submission) need checking. A consumer-facing source claimed "90 days to delete", which conflicts with the 45-day status rule.
- It is unconfirmed whether CalPrivacy allows a third-party vendor to hold a broker's API key or operate its DROP account (see §5). This is load-bearing for the product architecture.
- The exact current status of the audit and amendment rulemakings (comment-close dates, Office of Administrative Law timing) is not known.

---

## 2. Verification of claims from the earlier draft

### Takeaway
All four claims trace to real sources, but each needs more precise wording:
- **30% / 450,000:** accurate as reported by IAPP from the **Aug 7, 2026** CalPrivacy board meeting. The request count has since risen to 475k–500k+ (Aug 13–25, 2026).
- **About 580 brokers:** correct for **June 2026**, but by Aug–Sept 2026 the registry is **600+** (one analysis counts 603 on the Sept 1, 2026 snapshot).
- **9.2%:** comes from a **Stanford FAccT 2026 paper** (n=522, 2025 registry data). It measures full compliance with *metrics-reporting* transparency requirements, not overall compliance.

### Cited Findings
**Claim: "only about 30% of registered data brokers had begun processing DROP requests during the first week"**
- **Verified, with context.** IAPP reports that at the Aug 7, 2026 board meeting the agency said about 30% of registered brokers had started handling DROP requests in the first week after the Aug 1 compliance deadline — [IAPP, "CalPrivacy discusses DROP enforcement, data broker fee hike"](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike). The figure is repeated by [Clym](https://www.clym.io/blog/california-drop-compliance-data-brokers) and others.
- Caveat: brokers had 45 days to make their first access (until about mid-Sept 2026), so the 30% is an early-adoption snapshot, not a non-compliance rate — [Control D](https://controld.com/blog/data-broker-report/)
- I did not find the board-meeting slide deck itself or any later CalPrivacy figure (e.g., the share of brokers that accessed DROP by the end of the first 45-day cycle).

**Claim: "consumers had already submitted roughly 450,000 deletion requests"**
- **Verified for Aug 7, 2026**, also from [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike). Alston (Aug 2026) also reports about 450,000 — [Alston](https://www.alston.com/en/insights/publications/2026/08/california-privacy-opt-out-signals-data-brokers)
- Conflicting figure: one law-firm update put it at "345,000+ … submitted to date" around the same Aug 7 meeting. This is probably stale or a typo — [search summary of an Aug 20 law-firm update; source page not identified]
- Growth series (count of consumers or requests; one consumer's DROP request goes to all brokers):
  - "tens of thousands" registered — Jan 7, 2026 — [Privacy Daily](https://privacy-daily.com/article/2026/01/07/tens-of-thousands-register-for-californias-drop-required-deletions-begin-aug-1-2601070020?BC=bc_695ee76080a27)
  - more than 255,000 — late Mar 2026 — [PMG, May 13 2026](https://www.pmg.com/insights-and-news/understanding-drop-californias-new-platform-for-consumer-data-deletion). PMG also *projected* 500k–1M by August.
  - more than 285,000 — May 2026 — ⚠ search summary, source unclear
  - more than 300,000 sign-ups — Jun 2, 2026 — [CalPrivacy release](https://privacy.ca.gov/2026/06/privacy-momentum-builds-300000-californians-sign-up-for-drop-as-registered-data-brokers-hit-a-record-high/)
  - more than 325,000 consumers — July 2026 update — ⚠ [CalPrivacy DROP page via search summary](https://privacy.ca.gov/data-brokers)
  - 450,000 — Aug 7, 2026 — [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike)
  - more than 475,000 — Aug 13, 2026 — [Governor's office](https://www.gov.ca.gov/2026/08/13/icymi-california-takes-historic-action-against-data-brokers/)
  - more than 500,000 — Aug 25, 2026 — [Troutman citing CalPrivacy](https://www.troutmanprivacy.com/2025/12/analyzing-the-california-delete-act-regulations/)
- Consumer outreach was funded by a **one-time $7.9M** allocation. More marketing money needs legislative approval — [Bloomberg Government](https://news.bgov.com/privacy-and-data-security/most-california-data-brokers-saw-few-privacy-opt-out-requests)

**Claim: "~580 registered brokers"**
- **Accurate as of June 2026, outdated by August.** CalPrivacy's Jun 2, 2026 release says residents can reach "more than 580 data brokers" through DROP and calls it a record registry high — [CalPrivacy](https://privacy.ca.gov/2026/06/privacy-momentum-builds-300000-californians-sign-up-for-drop-as-registered-data-brokers-hit-a-record-high/). BrokerBlitzer counts 581 registrations — [BrokerBlitzer](https://brokerblitzer.com/registry)
- Later counts: "more than 600" brokers registered on the platform (Aug 2026) — [Alston](https://www.alston.com/en/insights/publications/2026/08/california-privacy-opt-out-signals-data-brokers). 603 companies in the **2026-09-01** registry snapshot — [DEV Community registry CSV analysis](https://dev.to/edwardfancher/parsing-californias-data-broker-registry-csv-28gc)
- Earlier counts: 459 entities (June 2025) rising to more than 575 (Feb 2026) per IAPP's February coverage — [IAPP](https://iapp.org/news/a/calprivacy-unpacks-drop-updates-on-consumer-participation-upcoming-enforcement). 566 per PMG (May 2026) — [PMG](https://www.pmg.com/insights-and-news/understanding-drop-californias-new-platform-for-consumer-data-deletion). 480 in the first SB 362 disclosure cycle — [The Record](https://therecord.media/dozens-of-data-brokers-disclose-selling-info-on-kids-geolocation-data-reproductive-health)

**Claim: "an academic review found only 9.2% were fully compliant with transparency requirements"**
- **Verified, but narrower than stated.** The source is Gueorguieva, King, Panidapu & Ho (Stanford), "Privacy Without Remedy: An Assessment of Data Broker Compliance with California Privacy Law", arXiv 2605.21376, accepted to ACM FAccT 2026. It studied **522** registered brokers.
  - In 2025, **9.2%** were fully compliant with reporting information for all rights-request types (the metrics-disclosure rules). The paper rounds this to 9% in places.
  - **45%** reported no information at all about requests received.
  - Of **250** brokers whose request processes were audited, **43%** made it impossible to exercise all rights and **64%** added at least one substantial friction feature.
  - Sources: [arXiv 2605.21376](https://arxiv.org/pdf/2605.21376); [Stanford HAI policy brief](https://hai.stanford.edu/assets/files/hai-policy-brief-regulating-data-brokers-in-the-age-of-ai.pdf); [HAI news](https://hai.stanford.edu/news/companies-that-buy-and-sell-your-data-are-not-following-californias-strict-privacy-laws)
- A separate study is often confused with it: van Kempen et al. (UC Irvine), "Consumer Beware!" (arXiv 2506.21914). They sent access requests to all **543** registered brokers, and **more than 40% never responded** — [arXiv 2506.21914](https://arxiv.org/pdf/2506.21914); [UCI news, Jul 2025](https://properdata.eng.uci.edu/2025/07/28/properdata-researchers-uncover-data-brokers-ccpa-compliance-issues)
- A third paper, "Let My Data Go: Data Brokers' Compliance with Opt-Out and Deletion Requests" (arXiv 2607.04552, Jul 2026), exists, but its findings could not be retrieved — [arXiv](https://arxiv.org/pdf/2607.04552)

### Inferences
- Suggested corrected wording:
  - "At its Aug 7, 2026 meeting, CalPrivacy reported that ~30% of registered brokers had begun processing DROP requests in the first week after the Aug 1 deadline, with ~450,000 requests submitted. By Aug 25 CalPrivacy cited 500,000+ registrants."
  - "The registry had 580+ brokers in June 2026 and 600+ by Aug–Sept 2026."
  - "A Stanford FAccT 2026 study of 522 brokers found only 9.2% fully complied with the request-metrics transparency rules in 2025."

### Gaps
- No primary CalPrivacy document (board slides or transcript) for the 30% and 450k figures was retrievable. They rest on IAPP's reporting.
- No post-Sept 15 figure for first-cycle compliance or total DROP requests as of Oct 2026 was found.

---

## 3. Enforcement against data brokers (2024 to Oct 2026)

### Takeaway
CalPrivacy runs a steady program: an Oct 2024 sweep, a Data Broker Enforcement Strike Force since Nov 2025, and roughly 9–14 broker actions so far. Almost all are **failure-to-register** cases with fines of about **$36k–$117k**, plus injunctive terms that now routinely require DROP processing and published metrics.

**No public enforcement action for failing to process DROP deletions was found as of Oct 9, 2026.** The first 45-day window only closed in mid-Sept 2026.

### Cited Findings
**Earlier actions (2024–2025)**
- Settlements with Growbots and UpLead (2024) and Background Alert (Feb 2025) followed the Oct 2024 sweep — [Crowell](https://www.crowell.com/en/insights/client-alerts/california-privacy-agency-launches-data-broker-strike-force-amid-delete-act-crackdown)
- ROR Partners, a marketing agency, paid **$56,600** for failing to register. This shows how broadly the agency reads "data broker" — [Troutman, Dec 2025](https://www.troutmanprivacy.com/2025/12/calprivacy-fines-marketing-agency-for-failing-to-register-as-a-data-broker/)
- **Nov 2025:** CalPrivacy launched a Data Broker Enforcement Strike Force in its Enforcement Division — [Troutman, Nov 2025](https://www.troutmanprivacy.com/2025/11/calprivacy-announces-data-broker-enforcement-strike-force/); [Crowell](https://www.crowell.com/en/insights/client-alerts/california-privacy-agency-launches-data-broker-strike-force-amid-delete-act-crackdown)
- **Dec 17, 2025:** Enforcement Advisory 2025-01 on registration (each entity registers separately; list all sites and DBAs) — [CPPA](https://cppa.ca.gov/pdf/enfadvisory202501.pdf)

**2026 actions**
- **Jan 8, 2026:**
  - Rickenbacher Data LLC d/b/a **Datamasters** (Texas, reseller for targeted advertising): **$45,000** fine and reportedly ordered to stop selling Californians' data.
  - **S&P Global:** **$62,600**, plus registration and compliance-audit procedures.
  - Sources: [CPPA announcement 2026-01-08](https://cppa.ca.gov/announcements/2026/20260108.html); [Covington Inside Privacy](https://www.insideprivacy.com/state-privacy/calprivacy-announces-45000-fine-against-data-broker-for-delete-act-violations/); [Loeb, Jan 2026](https://www.loeb.com/en/insights/passle/2026/01/cppa-acts-to-enforce-against-data-brokers-failure-to-register)
- **Aug 11, 2026: LocateSmarter LLC** (Iowa people-search). First action combining CCPA and Delete Act violations.
  - Total **$116,490**: $79,890 CCPA fine + $30,600 Delete Act fine + $6,000 registration fee. Some outlets report $110,490, which excludes the registration fee.
  - Violations: did not register by Jan 31, 2026, and required the last 4 digits of the SSN to opt out.
  - Order: register, remove the SSN and address requirement, retrain staff.
  - Sources: [CalPrivacy](https://privacy.ca.gov/2026/08/calprivacy-brings-first-action-against-a-data-broker-under-both-the-ccpa-and-delete-act/); [Paul Weiss](https://www.paulweiss.com/insights/client-memos/california-privacy-protection-agency-s-first-enforcement-action-against-data-broker-signals-industry-scrutiny); [Stauss Firm](https://staussfirm.com/2026/08/12/calprivacy-fines-data-broker-for-ccpa-and-delete-act-violations/); [Finnegan](https://www.finnegan.com/en/insights/articles/california-brings-first-ccpa-and-delete-act-enforcement-action-against-data-broker.html)
- **Aug 13, 2026: Cybba, Inc.** (Boston martech). **$52,400** for registering late.
  - Order: maintain timely registration, **process deletion requests through DROP**, and publish request metrics in its privacy policy.
  - FKKS/Mondaq call it the **14th** broker penalized for failing to register.
  - Sources: [CalPrivacy](https://privacy.ca.gov/2026/08/calprivacy-announces-second-data-broker-enforcement-action-in-less-than-a-week/); [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/calprivacy-settles-with-two-data-brokers-over-registration-failures-and-privacy-violations); [FKKS](https://technologylaw.fkks.com/post/102nhw0/californias-drop-era-enforcement-begins-targets-data-broker-registration-and-op)
- **Aug 13, 2026:** the Governor's office framed these as "historic action" and cited 475,000+ DROP requests — [gov.ca.gov](https://www.gov.ca.gov/2026/08/13/icymi-california-takes-historic-action-against-data-brokers/)
- **Sept 1, 2026: SalesIntel Research** (Virginia, B2B contact data). **$36,400** for late registration.
  - Order: post privacy-rights metrics, connect to DROP, process all future deletion requests through it.
  - Gizmodo calls it the **8th** in the current "blitz" and says SalesIntel holds about 54M mobile numbers.
  - Sources: [CalPrivacy](https://privacy.ca.gov/2026/09/calprivacy-continues-enforcement-blitz-with-action-against-virginia-data-broker/); [DataGuidance](https://www.dataguidance.com/news/california-cppa-fines-data-broker-36400-failure); [Gizmodo](https://gizmodo.com/this-unregistered-data-broker-holds-54-million-mobile-numbers-californias-fine-wont-erase-yours-2000814844)
- **Sept 3, 2026:** Enforcement Advisory 2026-01 on accuracy of registration information. CalPrivacy says it has already brought "multiple enforcement actions" over reporting errors. Executive director Tom Kemp: "DROP works because the law requires data brokers to report correct information" — [CalPrivacy release](https://privacy.ca.gov/2026/09/enforcement-advisory-targets-incorrect-information-in-data-broker-registration/); [Advisory PDF](https://privacy.ca.gov/wp-content/uploads/sites/357/2026/09/Enforcement-Advisory-No.-2026-01-Accuracy-of-Data-Broker-Registration-Information.pdf); [Nelson Mullins](https://www.nelsonmullins.com/insights/alerts/privacy_and_data_security_alert/all/calprivacy-drops-latest-drop-enforcement-advisory-faqs-and-another-clear-warning-to-data-brokers)

**Tallies and other notes**
- Counts differ by source: Loeb says nine actions since the Oct 2024 sweep (as of Jan 2026); Gizmodo counts SalesIntel as the 8th in the blitz; FKKS counts Cybba as the 14th registration penalty. WilmerHale calls LocateSmarter the "first ever" Delete Act action, which conflicts with earlier Delete Act registration fines — [WilmerHale, 2026-08-19](https://www.wilmerhale.com/en/insights/blogs/wilmerhale-privacy-and-cybersecurity-law/20260819-california-data-broker-updates)
- Headlines seen but not readable: "California Privacy Agency Shuts Broker for Registry Failure" — [Bloomberg Gov](https://news.bgov.com/bloomberg-government-news/california-privacy-agency-shuts-data-broker-for-registry-failure); "California Fines, Bans Data Broker in Privacy Crackdown" — [GovInfoSecurity](https://www.govinfosecurity.com/california-fines-bans-data-broker-in-privacy-crackdown-a-30498). These probably refer to the Datamasters stop-selling order, but that is unconfirmed.
- ⚠ CalPrivacy is reportedly coordinating investigations with Colorado and Connecticut. This was attributed to the Aug 2026 [Alston advisory](https://www.alston.com/en/insights/publications/2026/08/california-privacy-opt-out-signals-data-brokers) via search summary; attribution unconfirmed.
- No October 2026 broker enforcement action surfaced in search — searched 2026-10-09.

### Inferences
- Realized fines so far (about $36k–$117k) are far below the theoretical $200/request/day ceiling. Even so, each is **4–20× the $6k registration fee** and comes with injunctive DROP obligations. The credible small-broker fear is "a $50k–$120k settlement plus a compliance order," not ruin.
- A broker that ignored DROP for 30 days with 500k requests would face a statutory ceiling of 500,000 × $200 × 30 = $3B. That number is theoretical and unenforceable, but it shows up in vendor marketing.
- Expect the first DROP-processing actions in late 2026 or 2027, once CalPrivacy can see which brokers never accessed DROP or filed no statuses. The agency has that telemetry directly. Those first cases would be a strong demand catalyst.

### Gaps
- No primary list of all CPPA broker actions, so the exact count is unresolved.
- No information on whether any broker has been cited for DROP non-access since mid-Sept 2026.
- Datamasters' "stop selling" term and the Bloomberg "shuts broker" story are unverified.

---

## 4. Market size and makeup (California registry, other states, DROP-like mechanisms elsewhere)

### Takeaway
The directly obligated market is **about 600 California-registered brokers (Aug–Sept 2026)**. Roughly two-thirds declare no sensitive data, which points to many B2B-contact, marketing and lead-gen firms.

Other state registries (Vermont about 280, Oregon and Texas some hundreds each) mostly overlap with California's and have **no centralized deletion mechanism yet**.

The only other enacted DROP-style mechanism found is **Connecticut** (⚠ portal by Jul 2028, broker polling from Oct 1, 2028). Vermont's version was stripped to a study, New Jersey's new law has no deletion mechanism, and New York's bill is stalled in committee.

### Cited Findings
**California registry size**
- See §2: 480 (first disclosure cycle) → 459 (Jun 2025) → more than 575 (Feb 2026) → 566 (May 2026) → more than 580 (Jun 2, 2026) → 600+ (Aug 2026) → 603 (Sept 1, 2026 snapshot) — [CalPrivacy](https://privacy.ca.gov/2026/06/privacy-momentum-builds-300000-californians-sign-up-for-drop-as-registered-data-brokers-hit-a-record-high/); [DEV analysis](https://dev.to/edwardfancher/parsing-californias-data-broker-registry-csv-28gc); [official registry](https://cppa.ca.gov/data_broker_registry/)

**Registry makeup**
- Each registration answers about 77 questions: identity, sensitive-data flags, recipients, FCRA/GLBA/HIPAA coverage, and request metrics — [DEV analysis](https://dev.to/edwardfancher/parsing-californias-data-broker-registry-csv-28gc)
- Of 581 registrations, **384 (66.1%) declare no sensitive data**, which is consistent with business-contact-only brokers. **110 (18.9%) flag precise geolocation**, the most common sensitive flag — [BrokerBlitzer](https://brokerblitzer.com/registry)
- First cycle: 24 of 480 said they sell minors' data, and 79 said they sell precise geolocation — [The Record](https://therecord.media/dozens-of-data-brokers-disclose-selling-info-on-kids-geolocation-data-reproductive-health)
- Request volumes reported by brokers are skewed. Brokers reported **58.0M deletion requests** in the prior year and refused about 900k, per California filings — ⚠ [Control D](https://controld.com/blog/data-broker-report/). Yet "most California data brokers saw few privacy opt-out requests" — [Bloomberg Government](https://news.bgov.com/privacy-and-data-security/most-california-data-brokers-saw-few-privacy-opt-out-requests). Many brokers reported zero requests — [arXiv 2605.21376](https://arxiv.org/pdf/2605.21376)
- Categories in scope include marketing data appending, lead generation, identity resolution and data validation. Agencies that license third-party data for clients can also be swept in. People-search and background-check firms are partly FCRA-exempt — [California Lawyers Assn.](https://calawyers.org/privacy-law/data-broker-regulation-framework-a-comparative-analysis-of-california-texas-vermont-and-oregon/); [CLA, "Wake Now, Discover That You Are a Data Broker"](https://calawyers.org/privacy-law/wake-now-discover-that-you-are-a-data-broker/); [Henson Legal (lead gen)](https://www.henson-legal.com/newsroom//california-data-broker-registration-lead-generation); [Byte Back, Oct 2026](https://www.bytebacklaw.com/2026/10/is-your-business-model-subject-to-data-broker-laws/)
- Under the 2025 regulations, merely collecting data directly does not create a "direct relationship"; the consumer must intend and expect to interact with the business. This widens the set of firms that must register — [MoFo, Jan 2026](https://www.mofo.com/resources/insights/260115-think-you-re-not-a-data-broker-calprivacy-regulations)
- Enforced brokers so far are small or mid-size: Datamasters, LocateSmarter, Cybba, SalesIntel, ROR Partners. S&P Global is the large exception (§3).

**Other state registries**
- **Multi-state (Apr 2025):** PRC/EFF found **750** brokers registered in at least one state. Of these, 291 were absent from California's registry, 524 from Texas's, 475 from Oregon's and 309 from Vermont's. That implies large cross-state gaps and possible under-registration — [EFF, Jun 2025](https://www.eff.org/deeplinks/2025/06/why-are-hundreds-data-brokers-not-registering-states); [PRC](https://privacyrights.org/data-brokers)
- **Vermont:** about 283 brokers (2025–26 cycle). A registry snapshot shows 278 entries (177 active, 101 expired) — ⚠ [offlist.me snapshot](https://www.offlist.me/vt-broker); [privacylawmap](https://privacylawmap.com/blog/vermont-data-broker-delete-act-h211-2026). H.211 was signed Jun 16, 2026 as Act 138, effective Jan 1, 2027 — [FKKS](https://technologylaw.fkks.com/post/102n4qn/vermont-strengthens-data-broker-law); [Hunton](https://www.hunton.com/privacy-and-cybersecurity-law-blog/vermont-enacts-significant-amendments-to-data-broker-legislation)
- **Oregon:** 126 registrations (2024). For 2025, a legislative document says "345 active and 218 renewed", which is ambiguous — ⚠ [search summary; underlying document not identified]
- **Texas:** no published total. The registry operates under Bus. & Com. Code ch. 510 (recodified effective Sept 1, 2025) — [California Lawyers Assn. comparative](https://calawyers.org/privacy-law/data-broker-regulation-framework-a-comparative-analysis-of-california-texas-vermont-and-oregon/); [Texas SB 1343 analysis](https://capitol.texas.gov/tlodocs/89R/analysis/html/SB01343F.htm)
- Aggregators claim "750+ firms" across state registries in 2026 — [privacyterms.io](https://privacyterms.io/how-many-data-brokers-exist); [Monda](https://www.monda.ai/blog/data-broker-registries-in-the-us)

**DROP-like mechanisms in other states**
- **Connecticut:** ⚠ SB 4 / Public Act 26-64 (2026) creates a Department of Consumer Protection broker registry and accessible deletion mechanism. The portal is due by Jul 1, 2028, and brokers must check it every 45 days from Oct 1, 2028. This comes from a single search summary, most likely [Pandectes' 2026 guide](https://pandectes.io/blog/data-broker-compliance-in-2026-a-guide-to-california-connecticut-new-jersey-and-beyond/), and needs primary verification.
- **Vermont:** earlier drafts of H.211 included a one-portal deletion mechanism and audits. The Senate **removed the universal deletion right and centralized portal**, keeping a study (interim report Dec 1, 2027; final Dec 1, 2028) — [Privacy Daily, 2026-05-29](https://privacy-daily.com/article/2026/05/29/vt-data-broker-bill-goes-to-the-governor-after-losing-right-to-delete-2605290056?BC=bc_6a1a6531e2be3); [Citizen Portal](https://citizenportal.ai/articles/8034720/Vermont/Legislative/Committees/SENATE/Economic-Development/Housing-and-General-Affairs/Senate-committee-trims-data-broker-bill-removes-consumer-deletion-mandate-and-keeps-study); [State of Surveillance](https://stateofsurveillance.org/news/vermont-data-broker-delete-act-h211-march-2026/)
- **New Jersey:** A5328 was signed in 2026, making NJ the 7th state with a data broker law. IAPP calls it "costly." Registration starts around Apr 2027, with **no deletion or opt-out mechanism** in the broker provisions. A5332 (introduced Jun 28, 2026) is pending — [IAPP](https://iapp.org/news/a/independence-day-surprise-new-jersey-s-costly-new-data-broker-law); [CSG Law](https://www.csglaw.com/newsroom/csg-law-alert-new-jersey-enacts-comprehensive-data-broker-and-sensitive-data-amendments-to-the-njdpa/); [NJ A5328 text](https://pub.njleg.state.nj.us/Bills/2026/A5500/5328_I1.HTM)
- **New York:** S9088 (introduced Jan 30, 2026) would create registration plus a deletion mechanism. It was referred to committee with no further movement found — [DataGuidance](https://www.dataguidance.com/news/new-york-bill-data-brokers-registration-and-data)
- **Texas:** registry only. Advocates (PIRG) are pushing for a "one-button" deletion mechanism; no bill was found — [PIRG](https://pirg.org/edfund/resources/texas-data-privacy-and-security-act/)

### Inferences
- **Serviceable market today is about 600 entities, one jurisdiction.** At DropClerk's $99/mo, 100% penetration is about $0.7M ARR. At $500/mo it is about $3.6M, and at $1,000/mo about $7.2M. Excluding enterprises such as S&P Global and Experian-scale brokers that will use OneTrust/DataGrail-class platforms, a realistic small-broker addressable set is perhaps 300–450 firms. **This is a lifestyle-business TAM unless pricing is well above $500/mo or the product expands multi-state.**
- Connecticut (2028) would add a second "DROP" with likely heavy registrant overlap. That supports multi-jurisdiction value (one engine, many portals) more than new logos. Vermont, New Jersey and New York show momentum but no near-term second mechanism besides Connecticut.
- The skew toward firms declaring no sensitive data (66%) suggests many B2B-contact and lead-gen vendors: small, tech-light, cost-sensitive. They match the ICP but are likely to resist high prices.
- PRC/EFF's cross-registry gaps and CalPrivacy's registration enforcement point to an **unregistered tail** that enforcement keeps pulling into the registry (Cybba and SalesIntel registered after contact). That is a small but growing inflow.

### Gaps
- No authoritative breakdown of the California registry by company size (revenue or headcount) or category (people-search vs. marketing vs. B2B contact vs. risk/identity) was found. A founder could compute one from the official registry CSV.
- Current Texas and Oregon counts, and 2026 de-registrations or exits (brokers leaving California or the registry), could not be researched because the search budget ran out.
- Connecticut PA 26-64 details are unverified against primary text.

---

## 5. Competitive landscape (broker-side DROP tooling and consumer-side services)

### Takeaway
The broker-side "DROP engine" niche is **already contested** on both ends:
- **Enterprise privacy platforms** (DataGrail, TrustArc, Transcend, Ketch, Securiti, OneTrust) market DROP modules or workflows. DataGrail has a dedicated "fully automated" DROP product.
- **At least two or three DROP-specific micro-SaaS startups** target exactly the small-broker segment. **DropClerk** publicly prices at **$99/month per registration, first cycle free**, which sets a very low price anchor. Drop Privacy and DROP Autopilot also exist.
- **UnsubCentral**, a suppression-list incumbent for affiliate and email marketers, is positioning as DROP infrastructure.

### Cited Findings
**Enterprise and mid-market privacy platforms**
- **DataGrail:** dedicated "California DROP compliance, fully automated" product. It downloads the latest DROP lists, does hash-to-hash matching across connected systems, executes deletions, and reports status to CalPrivacy on schedule. It claims "no raw identifiers are ever exchanged with California or stored in your DataGrail environment." Launched around mid-2026 (blog roughly 3 months old as of search). Pricing not public — [DataGrail solution page](https://www.datagrail.io/solutions/drop-compliance/); [DataGrail launch blog](https://www.datagrail.io/blog/product/introducing-automated-drop-compliance-built-for-privacy-teams/); [DataGrail glossary](https://www.datagrail.io/glossary/what-are-the-delete-act-and-drop/)
- **TrustArc:** brokers can export a DROP deletion list and submit it into **Individual Rights Manager** as "a single, auditable request." This handles the back end of the cycle, not the matching — [TrustArc](https://trustarc.com/resource/california-delete-act-drop-platform-data-brokers/)
- **Transcend:** ingests DROP files by CSV or API, maps the state schema to the broker's identity map, and runs downstream erasure across the stack — [Transcend roadmap](https://transcend.io/blog/calprivacy-drop-compliance-guide); [Transcend broker governance](https://transcend.io/blog/privacy-governance-data-brokers)
- **Ketch:** once a DROP request is retrieved and matched, Ketch runs deletion across connected systems "without human intervention," with cascading deletion to service providers and data partners. It frames DROP as three needs: 45-day workflow automation, deletion enforcement, and audit documentation — [Ketch](https://www.ketch.com/blog/posts/california-drop-platform-data-broker-compliance)
- **Securiti:** whitepaper "Surviving the DROP Platform" describing a unified control plane for intake, identity resolution and end-to-end deletion — [Securiti](https://securiti.ai/whitepapers/surviving-drop-platform-rethinking-privacy-operations/)
- **OneTrust:** DROP explainer covering consent, preferences and deletion. Specific DROP feature not confirmed — [OneTrust](https://www.onetrust.com/blog/californias-drop-what-the-delete-act-changes-for-consent-preferences-and-data-deletion/)
- **Sentra** (data security posture management): blog "How to Automate CCPA DROP Compliance for Data Brokers." It says vendors can support discovery and deletion verification, but **"the DROP integration and status reporting must be the broker's own"** — [Sentra](https://sentra.io/blog/automating-ccpa-drop-compliance)
- **Truyo**, **Clym**, **Secure Privacy**, **Pandectes**, **SafeGuard Privacy** (multi-state data broker assessment) and **Captain Compliance** publish DROP or broker content. Product depth unverified — [Truyo](https://truyo.com/calprivacy-drop-requirements/); [Clym](https://www.clym.io/blog/california-drop-compliance-data-brokers); [Secure Privacy](https://secureprivacy.ai/blog/data-broker-registration); [SafeGuard Privacy](https://safeguardprivacy.com/resources/new-us-multi-state-data-broker-assessment/); [Captain Compliance](https://captaincompliance.com/news/californias-drop-platform-surpasses-300000-sign-ups-as-data-broker-registry-reaches-record-high/)

**Suppression and marketing-ops incumbent**
- **UnsubCentral:** an email and affiliate suppression-list platform and "opt-out system of record." Its DROP guide says it can centralize consumer identifiers, automate matching and suppression across systems, orchestrate downstream actions, and keep an auditable trail of DROP activity. It is not an official or endorsed CalPrivacy provider — [UnsubCentral DROP guide](https://www.unsubcentral.com/california-drop-and-the-delete-act-operational-guide-for-data-brokers/); [Suped review](https://www.suped.com/knowledge/email-deliverability/compliance/what-are-the-pros-and-cons-of-using-unsubcentral-for-managing-suppression-lists)

**DROP-specific startups (direct competitors to the idea)**
- **DropClerk** (dropclerk.com):
  - built for registered California brokers;
  - hashes and matches records **in the browser** against downloaded lists, and sends back only the state's work-item IDs with a status digit;
  - **$99/month per registration, first production cycle free**; "no tiers, no annual contract, no per-record fees"; free sandbox and practice mode.
  - Source: [DropClerk](https://dropclerk.com/)
- **Drop Privacy** (dropprivacy.com): "California Delete Act Compliance Engine for Data Brokers." Matches the state batch, responds through the DROP API, and keeps the audit record. Pricing not found, and one search could not confirm details — [Drop Privacy](https://dropprivacy.com/)
- **DROP Autopilot** (dropautopilot.com): publishes "CA DROP Program & Delete Act Audit Prep: 2028 Guide," which suggests a DROP and audit-prep offering. Product and pricing unverified — [DROP Autopilot](https://www.dropautopilot.com/prepare-california-privacy-audit.html)
- **gblock.app:** "California Data Brokers Now Face $200 a Day, Per Request" article. Unclear whether broker-side or consumer-side — [gblock](https://www.gblock.app/articles/california-drop-data-broker-deletion-deadline-2026)
- **GSDSI** publishes a state data broker registration tracker and a "what data buyers should know" piece on DROP. This points to downstream flow-down duties for data *buyers* — [GSDSI tracker](https://www.gsdsi.com/data-broker-registration-tracker); [GSDSI data buyers](https://www.gsdsi.com/resources/california-delete-act-drop-what-data-buyers-should-know)

**Third-party access to DROP: conflicting signals**
- One search summary claimed third-party platforms "are not permitted to access DROP directly on a broker's behalf." I could not trace this to a primary source ⚠.
- CalPrivacy's API reference describes broker-held, list-scoped API keys and says nothing about vendors — [API reference](https://cppa.ca.gov/orph/drop_tech_api_ref.pdf)
- Sentra says the integration and reporting "must be the broker's own" — [Sentra](https://sentra.io/blog/automating-ccpa-drop-compliance)
- DataGrail and DropClerk both market automated download and filing — [DataGrail](https://www.datagrail.io/solutions/drop-compliance/); [DropClerk](https://dropclerk.com/)
- Note that DropClerk's in-browser design keeps the broker's data and key client-side, which may be a deliberate answer to this constraint.

**Consumer-side services**
- Many consumer opt-out sites now run DROP explainers or registry tools: BrokerBlitzer, TraceKill, GhostVault, PrivacyOn, Offlist — [BrokerBlitzer](https://brokerblitzer.com/registry); [TraceKill](https://tracekill.com/blog/california-drop-delete-act); [GhostVault](https://www.ghostvault.live/data-brokers); [PrivacyOn](https://www.privacyon.com/blog/california-delete-act-and-drop-platform-explained)
- DeleteMe, Incogni, Optery and Kanary could not be researched (search budget exhausted). No evidence was found either way of a pivot to broker-side tooling.

### Inferences
- **The "small broker DROP engine" wedge is no longer empty.** DropClerk appears to be exactly this idea, priced at $99/mo with no contract. A new entrant must either undercut a $99 product (hard) or differentiate upward.
- Ways to differentiate upward:
  - **audit-evidence packs** mapped to the 9 audit components, with retention from Aug 1, 2026;
  - **suppression-at-ingest APIs** for data feeds (needed if the proposed amendments pass);
  - **service-provider and contractor deletion propagation with proof**;
  - **registry accuracy and filing management** (Advisory 2026-01 risk);
  - **metrics-report generation**, where 91% of brokers fail per Stanford;
  - **multi-state readiness** for Connecticut 2028.
- Enterprise vendors (DataGrail, Transcend, Ketch, TrustArc) will win brokers that already pay for DSR or privacy platforms. The small-broker gap they leave is real but already targeted by micro-SaaS.
- The architecture should assume the broker owns the DROP account and API key, with the product running under broker control (desktop or in-browser or self-hosted agent, or a delegated key in the broker's secret store) until CalPrivacy clarifies vendor access.

### Gaps
- No DROP-specific information was found for Osano, BigID, Privado, Didomi, Mine or LiveRamp. Search budget ran out before these could be queried. LiveRamp or other identity-resolution vendors adding DROP hash-matching is unverified.
- No public pricing was found for DataGrail, Transcend, Ketch, TrustArc, Securiti or OneTrust DROP modules (all appear quote-based).
- Founding dates, funding and customer counts for DropClerk, Drop Privacy and DROP Autopilot are unknown (no Crunchbase or press found).
- Consumer-service effects of DROP (e.g., DeleteMe or Optery positioning DROP as complementary vs. competitive) were not researched.

---

## 6. Business feasibility: willingness to pay, price benchmarks, demand evidence, risks

### Takeaway
**Demand is real and mandatory:**
- every registrant must run DROP every 45 days on 500k+ hashed records;
- audits arrive in 2028 and look back to Aug 2026;
- early adoption was weak (30% in week 1);
- enforcement is steady.

**Willingness to pay and market size are the problems:**
- about 600 firms;
- a live competitor charging **$99/mo**;
- enterprise platforms bundling DROP;
- evidence that many small brokers under-invest in compliance (9.2% metrics compliance; more than 40% ignore access requests);
- a fixed-cost backdrop (registration fee rising from $6k to $9.5k) that small brokers already resent.

### Cited Findings
**Cost and price anchors a small broker sees**
- Registration and DROP access costs $6,000 in 2026 and $9,500 in 2027 — [CalPrivacy fees](https://privacy.ca.gov/drop-for-data-brokers/account-creation-fees-and-annual-registration/); [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike)
- Recent settlements: $36,400 (SalesIntel), $45,000 (Datamasters), $52,400 (Cybba), $56,600 (ROR Partners), $62,600 (S&P Global) and $116,490 (LocateSmarter) — see §3 sources
- DropClerk charges **$99/month per registration** (about $1,188/yr) — [DropClerk](https://dropclerk.com/)
- Enterprise DROP modules (DataGrail and others) are quote-only — [DataGrail](https://www.datagrail.io/solutions/drop-compliance/)

**Demand and pain signals**
- About 30% of brokers were processing in week 1 (Aug 7, 2026) — [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike). Commentators attribute the slow start to "operational readiness," since integrating DROP into existing workflows and systems takes technical work — [search summary of the IAPP / other coverage]
- Stanford found that only 9.2% of 522 brokers were fully compliant with the metrics rules, and that 43% blocked some rights — [arXiv 2605.21376](https://arxiv.org/pdf/2605.21376)
- UC Irvine found that more than 40% of 543 brokers ignored access requests — [arXiv 2506.21914](https://arxiv.org/pdf/2506.21914)
- Trade-association engagement: the NAI filed preliminary DROP-audit comments on 2026-05-07 — [NAI](https://thenai.org/wp-content/uploads/2026/05/NAI-Preliminary-DROP-Audit-Comments-2026.05.07_FINAL.pdf). Consumer Reports and EPIC filed on the DROP NPRM in Jun 2025, from the consumer side — [CR/EPIC comments](https://advocacy.consumerreports.org/wp-content/uploads/2025/06/FINAL-CR-EPIC-Comments-Notice-of-Proposed-Rulemaking-on-Accessible-Delete-Mechanism-%E2%80%93-Delete-Request-and-Opt%E2%80%93out-Platform-DROP-System-Requirement.pdf)
- Heavy law-firm attention in 2026 indicates broad advisory demand: Kelley Drye "Getting Ready to Use the DROP," Alston "DROP Is Coming Due," Benesch, Manatt, Coblentz, Freshfields, WSGR — [Kelley Drye](https://www.kelleydrye.com/viewpoints/blogs/ad-law-access/getting-ready-to-use-the-drop); [Alston Privacy](https://www.alstonprivacy.com/drop-is-coming-due-what-californias-delete-act-means-for-data-brokers-in-august/); [Benesch](https://www.beneschlaw.com/insight/the-era-of-centralized-deletion-is-here-understanding-calprivacys-drop-platform-before-2026/); [Manatt](https://www.manatt.com/insights/newsletters/client-alert/california-s-first-of-its-kind-data-deletion-platform-goes-live-what-businesses-should-know); [Coblentz](https://www.coblentzlaw.com/news/navigating-californias-data-broker-requirements-in-2026/)
- Data *buyers* are being told to flow DROP obligations down contractually, which creates pull from buyers onto small sellers — [GSDSI](https://www.gsdsi.com/resources/california-delete-act-drop-what-data-buyers-should-know)

**Structural risks**
- CalPrivacy's consumer outreach depends on a one-time $7.9M allocation. If legislators do not renew it, DROP sign-up growth (and therefore per-cycle volume and perceived urgency) could slow — [Bloomberg Government](https://news.bgov.com/privacy-and-data-security/most-california-data-brokers-saw-few-privacy-opt-out-requests)
- The DROP data model is standardized (SHA-256 plus fixed normalization), so the core engine is easy to copy. Several vendors shipped within months of the Aug 2026 deadline — [DataGrail](https://www.datagrail.io/solutions/drop-compliance/); [DropClerk](https://dropclerk.com/); [Drop Privacy](https://dropprivacy.com/)

### Inferences
- **Willingness to pay is probably tiered:**
  - "Just make the 45-day filing happen": about $100–$300/mo, anchored by DropClerk.
  - "Audit-ready plus suppression-at-ingest plus service-provider proof plus registry and metrics filings": plausibly $500–$2,000/mo. That is still small next to a $9.5k fee and a $50k+ settlement.
  - Enterprise platforms are out of reach for small brokers.
- **The go/no-go hinges on differentiation and multi-state scope**, not on demand existing. A California-only, $99-class DROP filer is already on the market. The open question is whether there is room for a higher-value "compliance operations for small brokers" bundle: DROP plus suppression plus metrics plus registry accuracy plus audit evidence, with Connecticut from 2028.
- **The 2028 audit is the strongest upsell trigger.** Audit firms will need standardized evidence. Partnering with the independent auditors (or becoming the de facto evidence format) could be a moat that a $99 filer lacks.
- **Market-shrink risk:**
  - small brokers may exit California or restructure to avoid "broker" status, as Datamasters reportedly was ordered to stop selling Californians' data;
  - consolidation;
  - fee fatigue from the 58% increase.
  - The registry has kept *growing* through Sept 2026 (more than 600), so no evidence of net shrinkage yet.

### Gaps
- **Not researched (search budget exhausted):**
  - any legal challenge to the Delete Act or DROP (e.g., First Amendment suits by brokers or trade groups);
  - commentary from ANA, IAB, CDIA or ADDA/DMA;
  - forum or Reddit evidence of small-broker pain;
  - what small brokers currently pay for privacy tooling (OneTrust, Osano or Termly tiers);
  - evidence of brokers de-registering or exiting California in 2026.
  These are material to the go/no-go and should be covered in a follow-up pass.
- No survey data on broker willingness to pay was found.
- Whether CalPrivacy permits a vendor-operated DROP account (a hosted SaaS model) remains unconfirmed and should be asked of CalPrivacy directly or checked in the DROP for Data Brokers FAQ ([privacy.ca.gov/drop-for-data-brokers](https://privacy.ca.gov/drop-for-data-brokers/)).
