# Decisive facts verification: four state-compliance SaaS ideas (as of 2026-10-10)

**How this was verified.** Direct fetches to state, agency, lab and PRO sites were blocked from this environment (proxy 403 or DNS failure for cppa.ca.gov, privacy.ca.gov, leginfo, app.leg.wa.gov, cga.ct.gov, leg.colorado.gov, courtlistener, sgs.com, dropclerk.com and circularactionalliance.org). WebFetch could not resolve any host. Primary text therefore comes from four GitHub mirrors:

- **PUBINFO-2025**: the California Legislative Counsel database export, dated July 9, 2026. It holds codified law sections and bill versions.
- **tannewt/wa-law.org**: Washington bill text, last commit May 4, 2026.
- **api-evangelist/california-privacy-protection-agency**: CalPrivacy API docs and blog feed, generated 2026-09-17, with blog items through 2026-09-28.
- **OCR'd lab reports** posted in public repositories.

Everything else comes from search-engine summaries of the cited pages. Those pages were not opened, so treat quoted phrases from them as the search tool's extract, not verified wording. I used 30 web searches; GitHub code search was used on top of that budget.

**Verdict summary**

| # | Fact | Verdict |
|---|---|---|
| 1 | Vendor may hold a broker's DROP API key / operate its account | **Still unverified.** No CalPrivacy text either way. The DROP Terms of Use bar sharing account access. Transcend's documented setup has the broker hand its API key to the vendor. |
| 2 | DropClerk $99/mo per registration; scope | **Still unverified.** The site is blocked and not indexed. The prior notes contradict each other on whether pricing was ever retrieved. |
| 3 | DROP audit: first report Nov 1, 2028 vs Jan 1, 2029; Aug 1, 2026 look-back; nine components | **Corrected.** CalPrivacy's Aug 2026 board deck lists **Apr 1, 2029** for the first triennial audit-cycle certifications. The rule is still *proposed* (45-day comment period opened Aug 2026). The nine components are named. The look-back is unverified. |
| 4 | CT PA 26-64 dates; AB 883 / SB 1106 | **Partly confirmed / Corrected.** CT: mechanism by **Jul 1, 2028**, then 45-day checks. **AB 883 was signed** (30-day DROP cadence, reported effective Jan 1, 2027). SB 1106 appears to have died in committee. Separately, **SB 923** (Becker) was signed. |
| 5 | WA 5-business-day cure and its sunset; CT PA 26-12 private right of action / cure | **Confirmed (WA, verbatim).** The 2026 bills that would have made the cure permanent did not advance. CT: private right of action confirmed (2-year limitations period). Absence of a cure is **still unverified**. |
| 6 | Lab terms on sharing reports | **Partly confirmed.** SGS: no reproduction "except in full, without prior written approval". Intertek: only the client may permit copying, in full. BV Labs: full-only. Eurofins and BV CPS were not found. |
| 7 | AB 1817 wording; "AB 347 (2025)" DTSC timeline | **Confirmed (verbatim)** on "product or product component". The DTSC timeline is confirmed verbatim, but the bill label is **Corrected**: 2025–26 AB 347 is an unrelated Education Code bill. |
| 8 | CAA 2027 Oregon rates; California plan status; first year of CA fees | **Still unverified** (OR rates). CA: final plan due to CalRecycle in Oct 2026, with no approval found. Draft plan says annual invoices begin **early 2027**. |
| 9 | Colorado bar on showing EPR fees as a separate line item | **Still unverified.** The allegation is confirmed as NAW's claim, but the statutory or rule text was not located. The preliminary-injunction motion is pending. |

---

## 1. May a third-party vendor hold a broker's DROP API key or operate its DROP account?

### Takeaway
**Still unverified.** No CalPrivacy statute, regulation, FAQ or API document found says yes or no. The available evidence pulls in both directions:
- The DROP Terms of Use (as summarized by search) forbid sharing passwords or account access.
- DROP issues one active API key per account; issuing a new key deactivates all earlier keys.
- A major vendor (Transcend) documents a setup in which the broker supplies its CalPrivacy-issued broker ID and API key to the vendor.

TrustArc's "not permitted" line remains untraced to any CalPrivacy text.

### Cited Findings
- **Claim in prior report:** TrustArc says third-party platforms "are not permitted to access DROP directly on a broker's behalf", while DataGrail and Ketch market automated processing — [TrustArc](https://trustarc.com/resource/california-delete-act-drop-platform-data-brokers/) (as cited in prior notes, `idea1_drop_product_launch.md`).
- **Statute is silent on vendors.** Civ. Code §1798.99.86 (text as of the July 9, 2026 export) puts every duty on "a data broker":
  - "(c)(1) Beginning August 1, 2026, a data broker shall access the accessible deletion mechanism … at least once every 45 days."
  - The broker must "(C) Direct all service providers or contractors associated with the data broker to delete all personal information in their possession…"
  - Under (b)(8), "authorized agents" are mentioned only on the consumer side ("support the ability of a consumer's authorized agents to aid in the deletion request").
  - Source: [PUBINFO-2025 LAW_SECTION_TBL_4822 (Civ. Code §1798.99.86), export dated 2026-07-09](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_4822.lob)
- **Key model.** The published OpenAPI 1.2.0 (July 2026) states:
  - "All requests require an API key passed in the `X-API-KEY` header. API keys are generated in the Data Broker Portal … after registration and fee payment are complete."
  - The notification table includes "API Key Changed | A new API key has been issued; all previous keys have been deactivated."
  - The mirror's summary: "Single static API key … no OAuth, no scope vocabulary"; keys should be stored "in environment variables or a secret management system."
  - Sources: [api-evangelist mirror, OpenAPI original and authentication profile, generated 2026-09-17](https://github.com/api-evangelist/california-privacy-protection-agency/blob/main/openapi/_original/california-privacy-protection-agency-drop-data-broker-api-openapi.yaml); [authentication profile](https://github.com/api-evangelist/california-privacy-protection-agency/blob/main/authentication/california-privacy-protection-agency-authentication.yml)
- **Account terms.** Per the search summary of the DROP portal Terms of Use:
  - "access to secure areas is limited to authorized users";
  - users "must not share their password or hand account access to anyone else";
  - users are "fully responsible for all activities that occur through their account."
  - The same summary also mixes in consumer-side terms, so it is unclear whether this is the broker-portal or the consumer-portal Terms of Use. Sources: [DROP data broker portal](https://camc-dr.databroker.drop.privacy.ca.gov) and [consumer DROP site](https://www.consumer.drop.privacy.ca.gov) (search summary, n.d.; page not fetched).
- **CalPrivacy account guidance** (search summary): "DROP accounts are reserved exclusively for businesses operating as data brokers. Each business entity operating as a data broker must create its own DROP account and pay relevant fees." — [privacy.ca.gov, Account creation, fees, and annual registration](https://privacy.ca.gov/drop-for-data-brokers/account-creation-fees-and-annual-registration/) (search summary, n.d.)
- **Vendor practice** (search summary): Transcend's DROP setup guide says the broker must supply its own CalPrivacy-issued broker ID and API key, and Transcend pulls the CalPrivacy download through the API. The summary also says Transcend does not perform the matching for the broker. — [Transcend docs, "Set up and run California DROP"](https://docs.transcend.io/docs/articles/dsr-automation/california-drop) (search summary, n.d.; fetch blocked)
- Searches for a CalPrivacy FAQ answer on vendor access returned none. Secondary FAQs say only that a registered broker "still ha[s] to access DROP" itself. — [In-House Privacy DROP FAQ](https://www.inhouseprivacy.com/blog/california-drop-faq); [Nelson Mullins on CalPrivacy's DROP enforcement advisory FAQs](https://www.nelsonmullins.com/insights/alerts/privacy_and_data_security_alert/all/calprivacy-drops-latest-drop-enforcement-advisory-faqs-and-another-clear-warning-to-data-brokers) (search summaries, n.d.)

### Inferences
- The statute assigns the access duty to the broker but does not forbid using an agent to perform it. The plain prohibition found is on **sharing portal account access and passwords**, not on a vendor making API calls with a broker-issued key.
- A hosted vendor that holds the key is therefore not clearly prohibited. It is, however, unblessed and carries contract risk under the Terms of Use. Transcend's documented key-handoff model shows large vendors accept that risk.
- Each account has only one live key ("all previous keys have been deactivated"). The broker and a vendor therefore cannot hold separate keys. A vendor-held key is a *shared* credential, and DROP's logs cannot tell vendor calls from broker calls.
- **Business implication for idea 1:** keep the default architecture broker-controlled: a self-hosted agent, an in-browser tool, or the key kept in the broker's own secret store. Offer a hosted mode only with a broker-signed authorization and a key-rotation runbook. Before launch, ask CalPrivacy in writing through the DROP support contact ([databroker.drop.privacy.ca.gov/Contact](https://databroker.drop.privacy.ca.gov/Contact)) and keep the reply as part of the audit evidence.

### Gaps
- The full DROP Terms of Use text (broker portal) and any CalPrivacy FAQ entry on vendors or authorized representatives could not be fetched.
- The DROP system regulations (11 CCR §7600 et seq.) were not reachable. They may contain an agent or service-provider clause.
- The origin of TrustArc's "not permitted" statement remains untraced.

---

## 2. DropClerk: current price and feature scope

### Takeaway
**Still unverified.** dropclerk.com was blocked by the proxy, a web search for "dropclerk" returned no index of the product, and GitHub has no trace of it. The $99/month figure rests on a single earlier extract, and the prior notes contradict themselves on whether pricing was ever retrieved.

### Cited Findings
- **Claim in prior report:** "DropClerk sells a browser-based filer at $99/month per registration with the first cycle free." — [DropClerk](https://dropclerk.com/) (prior report).
- **Internal conflict in prior notes.** `idea1_drop_market_competitors.md` states "$99/month per registration" (citing dropclerk.com). `idea1_drop_product_launch.md` says "DropClerk … (pricing not retrieved)" and "DropClerk's pricing, customer count and team were not retrieved." — prior research notes in this repo, dated 2026-10-09.
- **Scope, per the earlier extract:** DropClerk "hashes your records, matches them against those lists, and sends back only the state's own work item ids, each with a status digit." That describes the core download-hash-match-upload cycle only. — [DropClerk](https://dropclerk.com/) (prior notes; not re-verified)
- A web search on 2026-10-10 for "dropclerk" returned no results for the product. — search log, this session.

### Inferences
- Treat "$99/month" as an unconfirmed price anchor. Nothing found shows that DropClerk offers suppression-list operations, service-provider deletion notices, or audit-evidence packs. Those remain the plausible differentiation space, but that is unconfirmed.
- **Business implication:** before pricing idea 1, someone must load dropclerk.com in a normal browser and record the page with its date. The page should be screenshotted or archived, because it is the competitive anchor.

### Gaps
- Current price, tiers, free-cycle terms, suppression, service-provider notice, audit-log features, and company or team details are all missing.

---

## 3. DROP audit regulation: first report date, look-back, nine components

### Takeaway
**Corrected.** CalPrivacy's own Aug 6–7, 2026 board presentation lists **"APR. 1, 2029 – First triennial audit cycle certifications due."** That differs from both the Nov 1, 2028 and the Jan 1, 2029 figures in the prior report.

The rule is **proposed, not final**: the Board opened a 45-day comment period on Aug 7, 2026. The nine components, as reported, are:
1. deletion list selection
2. DROP access
3. standardization
4. hashing
5. matching
6. actioning
7. status reporting
8. suppression list
9. service providers/contractors

The Aug 1, 2026 look-back was not verified.

### Cited Findings
- **Prior claims:** "first audit reports due **Nov 1, 2028**, covering an audit period that starts **Aug 1, 2026**" — [WSGR](https://www.wsgr.com/en/insights/calprivacy-authorizes-rulemaking-on-opt-out-signals-raises-data-broker-fees-and-starts-the-clock-on-drop-amendment-comment-period.html) / [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/drop-is-live-what-data-brokers-need-to-know-as-calprivacy-ramps-up-oversight-102nqhf). Versus "first results due to CalPrivacy by **Jan 1, 2029**" — [Clark Hill](https://www.clarkhill.com/news-events/news/is-your-business-a-data-broker-californias-drop-goes-live-and-calprivacy-continues-to-enforce-delete-act/) (both from prior notes).
- **Statute (verbatim, export of 2026-07-09), Civ. Code §1798.99.86(e):**
  - "(1) Beginning January 1, 2028, and every three years thereafter, a data broker shall undergo an audit by an independent third party to determine compliance with this section."
  - "(2) … the data broker shall submit a report resulting from the audit and any related materials to the California Privacy Protection Agency within five business days of a written request…"
  - "(3) A data broker shall maintain the report and materials … for at least six years."
  - The statute itself requires submission only *on request*. AB 883 leaves (e) unchanged in its June 17, 2026 text.
  - Sources: [PUBINFO LAW_SECTION_TBL_4822](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_4822.lob); [AB 883 as amended 2026-06-17, BILL_VERSION_TBL_15276](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/BILL_VERSION_TBL_15276.lob)
- **Agency deck:** "APR. 1, 2029 — First triennial audit cycle certifications due," shown alongside the Jan 1, 2028 start of mandatory triennial audits. — [CalPrivacy Board presentation, Aug 6–7, 2026 (20260806_07_10_presentation.pdf)](https://privacy.ca.gov/wp-content/uploads/sites/357/2026/07/20260806_07_10_presentation.pdf) (search summary; PDF not fetched)
- **Rulemaking status:** "At its August 7 meeting, the board began formal rulemaking on DROP audit regulations. The draft is now subject to a 45-day public comments period." Under the draft, auditors may not base findings "primarily on assertions, attestations, or a review of policies and procedures alone," must meet criteria for a "qualified, objective, and independent auditor," and must include deletion-system testing and in-person interviews. — [IAPP, "CalPrivacy discusses DROP enforcement, data broker fee hike"](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [CalPrivacy DROP Audits page](https://privacy.ca.gov/laws-and-regulations/drop-audits/) (search summaries, ~Aug 2026)
- **Nine components** (search summary): "Auditors must independently verify nine components, which include deletion list selection, DROP access, standardization, hashing, matching, actioning, status reporting, suppression list, and service providers/contractors." Evidence reviewed would include "policies and procedures, hashing evidence, deletion commands, system logs, status reports, and suppression lists." — [IAPP](https://iapp.org/news/a/calprivacy-discusses-drop-enforcement-data-broker-fee-hike); [Freshfields, "DROP is live"](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/drop-is-live-what-data-brokers-need-to-know-as-calprivacy-ramps-up-oversight-102nqhf) (search summaries, Aug 2026)
- **Preliminary comment round:** closed May 7, 2026, with 12 comments (77 pages). Themes included auditor qualifications and independence, evidence over assertions, identifiers and match rates, and backups and downstream deletion. — [CalPrivacy Aug 2026 presentation](https://privacy.ca.gov/wp-content/uploads/sites/357/2026/07/20260806_07_10_presentation.pdf); [MoFo, May 4, 2026](https://www.mofo.com/resources/insights/260504-data-broker-audits-are-coming) (search summaries)

### Inferences
- The agency's own date (Apr 1, 2029, for "certifications") should replace both earlier dates. The Nov 1, 2028 date may come from the pre-rulemaking draft. The Apr 2029 deliverable appears to be a certification to CalPrivacy, while the full report is produced on request within 5 business days.
- **Business implication:** the audit-driven demand wave is real but later than modeled. Audits can start Jan 1, 2028, and the first certifications are due Apr 1, 2029. Audit-readiness selling therefore runs through 2027–2028.
- The evidence pack should be organized as nine modules mapped to the components above. Each module needs system logs and test evidence, not policy documents, because the draft bars findings based primarily on attestations or policy review.
- An audit period starting Aug 1, 2026 is consistent with the statute (duties began that day), so logging should be retroactive to Aug 1, 2026 wherever possible.

### Gaps
- The proposed regulation text, its section numbers, the defined "audit period", the exact first-certification wording and the comment deadline were all unavailable (cppa.ca.gov and privacy.ca.gov blocked).
- No final rule exists yet; the comment period opened Aug 2026.

---

## 4. Connecticut PA 26-64 deletion-mechanism dates; enactment of California AB 883 and SB 1106

### Takeaway
**Connecticut (partly confirmed):**
- signed May 27, 2026, with registration from Jan 1, 2027 at a $2,500 fee;
- a centralized deletion mechanism must be built by **Jul 1, 2028**, after which brokers check it at least every 45 days;
- independent audits begin Jul 1, 2031.

The exact first-access date (Oct 1, 2028 in the prior notes) is unverified, and sources conflict on effective dates.

**California (Corrected):** **AB 883 was signed** in September 2026, per Venable and Freshfields. DROP cadence moves from 45 to **30 days**, reported effective **Jan 1, 2027**, and elected-official and judge provisions are operative **Jul 1, 2027**. **SB 1106 appears to have died** (held in committee, Aug 13, 2026, per a tracker). **SB 923** (Becker, CalPrivacy-sponsored), which extends the CCPA deletion right to third-party-sourced data, was also signed.

### Cited Findings
- **CT PA 26-64 (SB 4)** (search summary):
  - signed May 27, 2026;
  - "Connecticut must set up a centralized system by July 1, 2028, where a consumer can submit one request that directs all registered data brokers to delete their data. Once it is running, brokers must check the system at least every 45 days";
  - section 1 effective Oct 1, 2026, with registration from Jan 1, 2027;
  - $2,500 annual fee; independent audits begin July 1, 2031.
  - Pandectes gives conflicting dates (effective May 27, 2026; registration active from Oct 1, 2026). The search tool judged the Davis+Gilbert timeline consistent with the act text.
  - Sources: [Davis+Gilbert via Mondaq](https://www.mondaq.com/unitedstates/privacy-protection/1798652/connecticuts-newly-enacted-data-broker-law-how-it-stacks-up-against-californias-delete-act); [dglaw.com](https://www.dglaw.com/connecticuts-newly-enacted-data-broker-law-how-it-stacks-up-against-californias-delete-act/); [Pandectes 2026 guide](https://www.pandectes.io/blog/data-broker-compliance-in-2026-a-guide-to-california-connecticut-new-jersey-and-beyond/); official act PDF [2026PA-00064-R00SB-00004-PA.pdf](https://prdext3.cga.ct.gov/2026/act/pa/pdf/2026PA-00064-R00SB-00004-PA.pdf) (located, not fetchable; ~June 2026)
- **AB 883 text (primary, as amended in the Senate 2026-06-17):**
  - "(c)(1) Beginning August 1, 2026, a data broker shall access the accessible deletion mechanism … at least once every 30 days and … (A) Within 30 days after receiving a request … process all deletion requests…"
  - (d)(1) changes the recurring deletion to "at least once every 30 days".
  - New §1798.99.86.5 (elected officials and judges): "(i) This section shall become operative on July 1, 2027." It lets an official or judge, "or the Attorney General, a county counsel, or a city attorney" sue; "the court may award punitive damages" for willful violations. In this version, deletion is processed "by complying with Section 1798.99.86 and its implementing regulations."
  - Source: [PUBINFO BILL_VERSION_TBL_15276 (20250AB__088394AMD)](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/BILL_VERSION_TBL_15276.lob)
- **AB 883 votes:** Assembly 75-0 (2026-01-26); Senate 40-0 (2026-08-26); Assembly concurrence 71-2 (2026-08-27). — [LegiScan AB 883](https://legiscan.com/CA/bill/AB883/2025); [GovBuddy, verified 2026-08-25](https://www.govbuddy.com/california/bills/ab-883/) (search summaries)
- **AB 883 signed:** Venable's September 2026 update lists AB 883 among bills Newsom signed and says "the deletion-timing provisions take effect January 1, 2027." Freshfields' Oct 1, 2026 post covers it in the "end-of-session privacy package."
  - Conflict on the officials' and judges' expedited deadline: Freshfields says "10 days"; GovBuddy's earlier version says "five days." The June 17 text above routes deletion through the normal §1798.99.86 cycle, so the final text changed after June.
  - Sources: [Venable, Sept 2026](https://www.venable.com/insights/publications/2026/09/state-quick-hits-california-privacy-and-ai); [Freshfields, Oct 1, 2026](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/californias-end-of-session-privacy-package-102o404) (search summaries)
- **SB 1106 (Cabaldon):**
  - Introduced 2026-02-13 to amend §1798.99.86 — [PUBINFO BILL_VERSION_TBL_10630 (20250SB__110699INT)](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/BILL_VERSION_TBL_10630.lob).
  - CalPrivacy staff recommended support — [CalPrivacy May 1, 2026 board memo](https://www.cppa.ca.gov/meetings/materials/20260501_item3_sb1106.pdf).
  - GovBuddy says it was "held in committee and under submission on August 13, 2026", though the page is mislabeled — [GovBuddy SB 1106](https://www.govbuddy.com/california/bills/sb-1106/) (search summary).
- **SB 923 signed:** Newsom signed SB 923 (Becker; CalPrivacy-sponsored). It extends the CCPA deletion right to data obtained from third parties and requires a web form for online-only businesses, effective Jan 1, 2027. AB 1542 (ban on sales of sensitive data) was vetoed. — [Bloomberg Law](https://news.bloomberglaw.com/business-and-practice/newsom-vetoes-ban-of-sensitive-data-sales-expands-privacy-laws); [Freshfields](https://www.freshfields.com/en/our-thinking/blogs/a-fresh-take/californias-end-of-session-privacy-package-102o404) (search summaries, ~Oct 2026)
  - CalPrivacy's own feed shows a 2026-09-28 post, "California Expands Privacy Protections by Strengthening Deletion Rights": "The legislation was authored by Senator Josh Becker (D-Menlo Park) and sponsored by the California Privacy Protection Agency." — [CalPrivacy feed mirror](https://github.com/api-evangelist/california-privacy-protection-agency/blob/main/blogs/2026-09-28-california-expands-privacy-protections-by-strengthening.md) (original: [privacy.ca.gov](https://privacy.ca.gov/2026/09/california-expands-privacy-protections-by-strengthening-deletion-rights/))

### Inferences
- **Business implication for idea 1:**
  - The scheduler must switch to a **30-day cycle from Jan 1, 2027**. That raises the operational burden by 50% and the penalty exposure from missed cycles.
  - A new elected-official and judge path (Jul 1, 2027) brings AG, county and city-attorney enforcement and punitive damages. Both strengthen the "reliable operations plus evidence" pitch.
  - SB 923 expands deletion of third-party data under CCPA, which affects brokers' direct consumer requests.
  - Connecticut is not a 2027 revenue market. Its mechanism arrives by Jul 1, 2028, so expansion revenue starts in H2 2028 at the earliest. Registration-only tooling (Jan 2027) is a thin wedge.

### Gaps
- No chaptered AB 883 text or chapter number was found. The final deadline for officials and judges (5 vs 10 days) is unresolved.
- No official record of SB 1106's final status was found.
- CT PA 26-64 section 5 text, and whether brokers' first access date is Jul 1 or Oct 1, 2028, were not verified.

---

## 5. Washington RCW 49.58.110 (SSB 5408) cure and sunset; Connecticut PA 26-12

### Takeaway
**Washington: confirmed verbatim.** The 5-business-day cure applies only to postings from July 27, 2025 through **July 27, 2027**. The provision says "does not apply after July 27, 2027". Scraped copies "digitally replicated and published without an employer's consent" are not "postings". Three 2026 bills to change this (SB 6100 and SB 6221 would have made the cure permanent; HB 2377 would have tightened the "applicant" definition) never advanced past introduction.

**Connecticut PA 26-12: private right of action confirmed**, effective Oct 1, 2026, with a 2-year limitations period. **No cure provision surfaced** in any summary, but its absence is not verified against the act text.

### Cited Findings
- **SSB 5408 session law (Laws of 2025, ch. 383), §1(1)(a)–(b), verbatim:**
  - "'Posting' does not include a solicitation for recruiting job applicants that is digitally replicated and published without an employer's consent."
  - "(b) For any postings from the effective date of this section through July 27, 2027, an employer must be afforded an opportunity to correct a violation of this subsection (1) before a job applicant may seek remedies under subsection (4) or (5) of this section. Any person may provide written notice to an employer alleging that the employer's posting does not comply with this subsection (1). If an employer receives notice from any person as to a particular posting, this constitutes adequate notice for the duration of that posting for any job applicant seeking remedies under subsection (4) or (5) of this section. If the employer corrects the posting within five business days of receiving the written notice and, where applicable, contacts any applicable third-party posting entity with a demand to correct the posting, then neither the department nor the court may assess or award penalties, damages, or other relief under this section for the violation. This subsection (1)(b) does not apply after July 27, 2027."
  - Remedies: statutory damages "no less than $100 and no more than $5,000 per violation"; private suit within "three years"; "exclusive remedies". The act applies only to employers with 15 or more employees.
  - Source: [wa-law.org mirror of 5408-S.SL (repo last updated 2026-05-04)](https://github.com/tannewt/wa-law.org/blob/main/site/bill/2025-26/sb/5408/S.SL/README.md); official PDF [lawfilesext.leg.wa.gov 5408-S.SL.pdf](http://lawfilesext.leg.wa.gov/biennium/2025-26/Pdf/Bills/Session%20Laws/Senate/5408-S.SL.pdf)
- **Effective date and chapter:** "Effective July 27, 2025, RCW 49.58.110 is amended to provide employers an opportunity to correct … within five business days… See LAWS OF 2025, ch. 383, § 1(b)." — [Branson v. Washington Fine Wine & Spirits, Wash. Sup. Ct. No. 103394-0, filed Sept 4, 2025, n.8 (text mirror)](https://github.com/jafrank88/CaseStrainer/blob/48e162775a6977c146ed226cb092f3542ebbae54/1033940_full_text.txt). The same opinion held that a "job applicant" must apply to a specific posting but need not prove a bona fide intent to be hired.
- **2026 bills that did not advance:**
  - SB 6100 ("Wage disclosure corrections") and SB 6221 ("Wage and salary disclosures") both restate (1)(b) **without** the date limits ("An employer must be afforded an opportunity to correct…"). That would make the cure permanent.
  - HB 2377 keeps the July 27, 2027 sunset and adds "'applicant' means a person who applies for a position with a genuine intent to be considered for employment."
  - The mirror lists only "Original Bill" for all three, with no substitute or passed version, as of the May 4, 2026 commit. Washington's 2026 session had ended by then.
  - Sources: [SB 6100](https://github.com/tannewt/wa-law.org/blob/main/site/bill/2025-26/sb/6100/README.md); [SB 6221](https://github.com/tannewt/wa-law.org/blob/main/site/bill/2025-26/sb/6221/README.md); [HB 2377](https://github.com/tannewt/wa-law.org/blob/main/site/bill/2025-26/hb/2377/README.md)
- **CT PA 26-12 (HB 5003)** (search summaries):
  - signed May 2026, effective **Oct 1, 2026**;
  - wage range plus a general description of benefits required in every internal and external posting, including remote roles reporting into Connecticut;
  - applicants and employees can sue, and a "private right of action must be brought within two years";
  - the Department of Labor can investigate and issue civil penalties but cannot obtain individual damages.
  - Sources conflict on whether punitive damages remain available. No source mentions a cure period.
  - Sources: [Littler](https://www.littler.com/news-analysis/asap/public-act-no-26-12-gamechanger-connecticut-workplace-compliance-here-are); [Foley, Sept 2026](https://www.foley.com/insights/publications/2026/09/connecticut-expands-pay-transparency-requirements-starting-october-1-2026/); [Epstein Becker Green](https://www.ebglaw.com/insights/publications/connecticut-private-employers-new-workplace-rules-take-effect-october-1); [Shipman & Goodwin](https://www.shipmangoodwin.com/insights/best-practices-for-connecticut-employers-wage-transparency-recordkeeping-and-multistate-compliance.html)

### Inferences
- **Business implication for idea 2:**
  - Washington exposure returns in full for postings made after **July 27, 2027**: no cure, $100–$5,000 per violation, and a 3-year limitations period.
  - The 2027 legislative session (Jan–Apr 2027) is the last chance to extend the cure. The 2026 attempts died, but employer groups will likely try again, which keeps legal-reversal risk.
  - The cure clock (5 business days from written notice, plus a demand to third-party posting sites) is a concrete product feature until then.
  - Scraped copies without employer consent are outside liability. Monitoring should therefore focus on channels the employer controls or has consented to: ATS feeds, job-board syndication and agency postings.
  - Connecticut is live now (Oct 1, 2026) with private suits. If no cure exists, Connecticut is the stronger "pre-publish and monitor" market today.

### Gaps
- The text of CT PA 26-12 was not retrieved, so the absence of a cure period and the damages scope (punitive or not) remain unverified.
- The current codified text of RCW 49.58.110 on app.leg.wa.gov (blocked) was not checked against the session law.

---

## 6. PFAS lab report sharing: SGS, Intertek, Bureau Veritas, Eurofins

### Takeaway
**Partly confirmed.** Standard lab terms allow the **client** to share reports, but only **in full**. Partial reproduction, and any use of the lab's name or marks in marketing, needs the lab's written approval. Labs also disclaim any duty to third parties.

SGS's General Conditions expressly authorize SGS to deliver reports to third parties on the client's instruction. At least one regional version requires prior notice to SGS and lets SGS invoice for the added liability.

Eurofins and Bureau Veritas Consumer Products Services terms were **not found**.

### Cited Findings
- **SGS report legend (verbatim, SGS-CSTC Guangzhou test report GZES230100125901, issued 2023-02-01):**
  - "This document is issued by the Company subject to its General Conditions of Service printed overleaf, available on request or accessible at www.sgs.com/terms_and_conditions.htm…"
  - "The Company's sole responsibility is to its Client and this document does not exonerate parties to a transaction from exercising all their rights and obligations under the transaction documents."
  - "This document cannot be reproduced except in full, without prior written approval of the Company."
  - "Any unauthorized alteration, forgery or falsification of the content or appearance of this document is unlawful…"
  - Source: [OCR text mirror, adhikaribibek231/evidence-review-engine](https://github.com/adhikaribibek231/evidence-review-engine/blob/ab7d531bd0a70322d617419042625911775be600/outputs/extracted_text/DSS_GZES230100125901_combined-1.txt)
- **SGS General Conditions of Service** (several regional versions; search summary): "Client hereby irrevocably authorises the Company to deliver Reports of Findings to a third party where so instructed by Client" or where implied by "circumstances, trade custom, usage or practice."
  - The Mozambique version: each Report of Findings "shall be issued by the Company exclusively in the interest of the Client". Before sharing with a third party, "prior notice must be given to the Company, which reserves the right to invoice the Client" for the added liability. Data collected for reports "shall remain available to the Company."
  - Sources: [SGS GCS (FR/CI/CM versions)](https://www.sgs.com/-/media/sgscorp/documents/corporate/technical-documents/legal-documents/general-terms-of-service/sgs-general-conditions-of-services-en.cdn.fr-CI.pdf); [SGS GCS Mozambique](https://www.sgs.com/-/media/sgscorp/documents/corporate/technical-documents/legal-documents/conditions-of-services/sgs-general-condition-service-en.cdn.en-MZ.pdf); [SGS Taiwan GCS](https://sgs.com.tw/uploads/footer/SGS%20Legal%20General%20Conditions%20of%20Services%20EN.pdf) (search summaries; version dates not shown)
- **Intertek report legend** (search summary of Intertek-issued reports hosted by customers):
  - The report "is for the client's exclusive use under its agreement with Intertek"; Intertek owes no duty to other parties.
  - "Only the client may authorize copying or distribution, and only for the whole document."
  - Use of "the Intertek name or its marks" to sell or advertise the tested product "requires Intertek's prior written approval."
  - Sources: [Intertek photometric test report hosted by Full Compass](https://www.fullcompass.com/common/files/28748-AntariUVWash2000PhotometricTestReport.pdf); [Intertek ASTA licence hosted by Legrand](https://assets.legrand.com/pim/Certif/LGVKGKPWUI.PDF) (search summaries, n.d.)
- **Bureau Veritas Laboratories (Canada; environmental):** "This Certificate shall not be reproduced except in full, without the written approval of the laboratory." — [BV Labs certificate inside a 2021-07-20 geotechnical report (text mirror)](https://github.com/j-christie/ASEC_Data). This is BV's environmental lab, not BV Consumer Products Services, which does PFAS textile testing.
- No Eurofins terms on third-party sharing were found (GitHub code search and web search, 2026-10-10).

### Inferences
- Under these terms, a network where **the brand (the lab's client) uploads and authorizes sharing of complete, unaltered report PDFs** appears permitted without a lab contract. A network that **extracts data, shows partial results, or uses lab names or logos** (for example, "SGS-verified") needs written lab approval.
- Labs disclaim reliance by third parties, so retailers viewing a shared report have no contract claim against the lab. Liability stays with the brand, which fits the earlier recommendation to keep liability with the brand.
- **Business implication for idea 4:** the network can start brand-side (client-authorized, full PDFs, a tamper-evident hash, no lab branding in the UI) without lab partnerships. Lab partnerships become necessary only for structured data feeds, verification APIs or co-marketing. SGS regional terms may require notice to SGS before third-party sharing, so the onboarding flow should include a client attestation that any required notice was given.

### Gaps
- The full current global SGS GCS clause text (with date) was not retrieved.
- Terms from Intertek's own website, Eurofins' general terms, and Bureau Veritas CPS terms were not found.
- No lab policy on platform-hosted reports or on data extraction was found.

---

## 7. California AB 1817 (H&SC §108970 et seq.) wording; DTSC enforcement timeline ("AB 347 (2025)")

### Takeaway
**Confirmed verbatim.** The threshold test applies to "a **product or product component**", measured as total organic fluorine: 100 ppm from Jan 1, 2025 and **50 ppm from Jan 1, 2027**.

The DTSC enforcement timeline is **confirmed verbatim**:
- test methods and lab accreditations published by Jan 1, 2029;
- regulations adopted by Jan 1, 2029;
- manufacturer registration and statement of compliance by **Jul 1, 2029**;
- DTSC enforcement from **Jul 1, 2030**.

The **bill label is corrected**: the 2025–26 session's AB 347 is an unrelated Education Code bill. The enforcement chapter was already "existing law" in September 2025, which fits AB 347 of the 2023–24 session (inference).

### Cited Findings
- **§108970 (definitions; Chapter 13.5 "commencing with Section 108970"), verbatim (export 2026-07-09):**
  - "(g) 'Regulated perfluoroalkyl and polyfluoroalkyl substances or PFAS' means either of the following: (1) PFAS that a manufacturer has intentionally added to a product and that have a functional or technical effect in the product, including the PFAS components of intentionally added chemicals and PFAS that are intentional breakdown products of an added chemical that also have a functional or technical effect in the product. (2) The presence of PFAS in a product or product component at or above the following thresholds, as measured in total organic fluorine: (A) Commencing January 1, 2025, 100 parts per million. (B) Commencing January 1, 2027, 50 parts per million."
  - "(i)(1) 'Textile articles' means textile goods of a type customarily and ordinarily used in households and businesses, and include, but are not limited to, apparel, accessories, handbags, backpacks, draperies, shower curtains, furnishings, upholstery, beddings, towels, napkins, and tablecloths."
  - (i)(2) excludes:
    - carpets and rugs, and PFAS treatments for converted textiles or leathers (both regulated under the Safer Consumer Products program);
    - vehicles and their component parts; vessels and their component parts;
    - industrial filtration media; laboratory textiles; aircraft;
    - "stadium shades or other architectural fabric structures."
  - "(h) 'Textile' means any item made in whole or part from a natural, manmade, or synthetic fiber, yarn, or fabric, and includes, but is not limited to, leather…"
  - Source: [PUBINFO LAW_SECTION_TBL_95558](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_95558.lob). The chapter and section identity is confirmed by [LAW_SECTION_TBL_138812](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_138812.lob): "Chapter 13.5 (commencing with Section 108970)… Textile articles, as defined in Section 108970."
- **Prohibition and certificate (next section, presumably §108971), verbatim:**
  - "(a)(1) … commencing January 1, 2025, no person shall manufacture, distribute, sell, or offer for sale in the state any new, not previously used, textile articles that contain regulated [PFAS]."
  - "(2) Paragraph (1) does not apply to outdoor apparel for severe wet conditions until January 1, 2028," but such apparel must carry the disclosure "Made with PFAS chemicals," including online.
  - "(c) A manufacturer of a textile article shall provide persons that offer the product for sale or distribution in the state with a certificate of compliance … signed by an authorized official of the manufacturer… may be provided electronically."
  - "(d) A distributor or retailer … shall not be held in violation … if they relied in good faith on the certificate of compliance."
  - Source: [PUBINFO LAW_SECTION_TBL_95559](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_95559.lob)
- **DTSC enforcement chapter, verbatim:**
  - "Covered product" includes "(2) Textile articles, as defined in Section 108970" — [LAW_SECTION_TBL_138812](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_138812.lob).
  - Registration section (§108079 per SB 682's cross-reference): "(a) On or before July 1, 2029, a manufacturer of a covered product shall register with the department and provide … (3)(A) A statement of compliance… (B) The department may request, and a manufacturer shall provide, technical documentation, including analytical test results…"; "(b) On or before January 1, 2029, the department shall publish on its internet website a list of accepted methods for testing … and appropriate third-party accreditations for laboratories"; "(d) On and after July 1, 2030, the department shall enforce and ensure compliance with this chapter." — [LAW_SECTION_TBL_138844](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_138844.lob)
  - "On or before January 1, 2029, the department shall adopt regulations…" — [LAW_SECTION_TBL_94749](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_94749.lob)
  - DTSC may receive "reports of alleged violations … including analytical test results, from consumers, businesses, research institutions…" and verify them by its own testing — [LAW_SECTION_TBL_138878](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_138878.lob).
  - Notices of violation are published on DTSC's website — [LAW_SECTION_TBL_139822](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/LAW_SECTION_TBL_139822.lob).
- **The label "AB 347 (2025)" is wrong:**
  - In the 2025–26 session, AB 347 (20250AB__0347) is "An act to amend Sections 32255… of the Education Code, relating to pupil instruction" — [PUBINFO BILL_VERSION_TBL_680](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/BILL_VERSION_TBL_680.lob).
  - SB 682's enrolled digest (2025-09-13) already describes the DTSC regime as "Existing law requires the Department of Toxic Substances Control, on or before January 1, 2029, to adopt regulations … on and after July 1, 2030, to enforce … manufacturers … on or before July 1, 2029, to register…" — [PUBINFO BILL_VERSION_TBL_9025 (SB 682 ENR)](https://github.com/aaronjuar-ez/PUBINFO-2025/blob/main/BILL_VERSION_TBL_9025.lob).

### Inferences
- "Product **or product component**" means each component (shell fabric, lining, membrane, trim, thread, print) must be at or below 50 ppm TOF from Jan 1, 2027. Component-level testing and component-level evidence are what the law implies. The data model should store reports per component per SKU.
- Total organic fluorine is a screening method that does not distinguish PFAS from other organofluorine. That favors labs offering TOF and creates false-positive dispute workflows.
- The good-faith reliance shield for distributors and retailers (§108971(d)) gives retailers a reason to demand signed, electronic certificates of compliance. That supports a certificate network or checkout block.
- DTSC's Jan 1, 2029 list of accepted test methods and lab accreditations will decide which reports count from 2029. Registration (Jul 2029) requires producing analytical test results on request.
- **Business implication for idea 4:** the network's durable value peaks around 2029–2030. Until then, enforcement is by the AG, local prosecutors and private parties under other provisions, not DTSC.
- The enforcement law is most likely AB 347 from the 2023–24 session (chaptered 2024). This is an inference from the chronology, not verified.

### Gaps
- The exact section numbers of the DTSC chapter (around §108075–108083) and its enacting bill and chapter number were not confirmed.
- No DTSC rulemaking status (as of Oct 2026) was found.

---

## 8. CAA 2027 Oregon fee schedule; California program plan status; first year of full California fees

### Takeaway
**Still unverified (Oregon rates).** The CAA site was blocked and no search surfaced the 2027 rate table. The prior figures (PE film 12¢, PP film 56¢, PET clear 19¢ final; base 29¢/97¢/28¢) come from a search tool's reading of PDF fragments with uncertain columns. Corrugated 2027 was never captured.

The reserve-return mechanism is corroborated: CAA's 2025 annual report showed $145.5M collected against $56.5M spent, and a federal court noted that surplus could reduce 2026 and 2027 Oregon fees.

**California:**
- CAA submitted its draft plan June 15, 2026, and comments ran to Aug 14, 2026.
- The final plan was due to CalRecycle in **October 2026**; **no approval was found** as of Oct 10, 2026.
- The draft plan expects **annual invoices to begin in early 2027**.

The "2028" first-year claim (EPR Atlas) is not corroborated.

### Cited Findings
- **Prior claims (from search excerpts):** CAA's OR 2027 schedule was published Oct 1, 2026 (OR-2027FeeSchedule_100126.pdf), with PE film 0.12 $/lb (base 0.29), PP film 0.56 (base 0.97) and PET clear 0.19 (base 0.28). About $80M in reserves plus $3M in SIM fees are returned through lower rates, and the lowest-tier flat fee falls from $1,200 to $700. — [CAA OR 2027 fee schedule PDF](https://circularactionalliance.org/s/OR-2027FeeSchedule_100126.pdf); [CAA OR 2027 Producer Fees](https://circularactionalliance.org/or-2027-producer-fees) (prior notes flag "column reading uncertain")
- **2026 Oregon comparators** (prior notes, from the CAA 2026 PDF via search excerpt): corrugated 8.0¢/lb, PE film 43¢, PP film 102¢, PET clear bottles 25¢ — [CAA OR 2026 Fee Schedule](https://circularactionalliance.org/s/OR-2026-Fee-Schedule-Public.pdf)
- **Searches this session** found no published 2027 per-material rates. One Oregon producer summary (May 2026) says fees are set per pound across ~60 categories in 8 classes and invoiced 50% in January and 50% in July. — [Personal Care Products Council, Oregon EPR Summary, May 2026](https://www.personalcarecouncil.org/wp-content/uploads/2026/06/Oregon-EPR-Summary_May-2026.pdf) (search summary)
- **Surplus corroboration:** "CAA's 2025 Annual Report … showed $145.5 million in fees collected but only $56.5 million expended, yielding an apparent surplus of approximately $90 million. A federal court said CAA's surplus funds could reduce Oregon's 2026 and 2027 producer fees." — [O'Melveny alert on the Oregon district court ruling](https://www.omm.com/insights/alerts-publications/federal-district-court-in-oregon-rejects-industry-challenge-to-state-epr-law-on-plastics-and-packaging/); [CAA 2025 Oregon Annual Report](https://www.oregon.gov/deq/recycling/Documents/CAA2025AnnualReport.pdf) (search summaries, ~Aug–Sept 2026)
- **California plan status:** "CAA submitted its draft plan on June 15, 2026, and the public comment period … is open until August 14, 2026. CAA expects to revise the plan before submitting a final version to CalRecycle in October 2026." The draft projects a five-year budget of $9.3B–$17.2B, and "Annual invoices are expected to begin in early 2027." No approval was found. — [Bergeson & Campbell / NatLawReview, "EPR: California Draft Program Plan Open for Public Comment"](https://natlawreview.com/article/epr-california-draft-program-plan-open-public-comment); [Mondaq version](https://www.mondaq.com/unitedstates/waste-management/1812816/epr-california-draft-program-plan-open-for-public-comment); [DLA Piper, Jun 2026](https://www.dlapiper.com/en-us/insights/publications/2026/06/californias-epr-program-plan) (search summaries)
- **Conflicting claim:** one tracker puts California's full fee structure in 2028 — [EPR Atlas California](https://epratlas.com/california/) (prior notes).

### Inferences
- **Business implication for idea 5:** do not ship hard-coded 2027 Oregon numbers from the prior notes. Transcribe the CAA PDF directly and keep base, adjustment and final columns separate, because the 2027 rates include one-time reserve returns.
- California's 2027 full-fee start depends on CalRecycle approving the plan, which by statute is due on or before Jan 1, 2027. Model 2027 as the first fee year, with a scenario flag in case approval slips.

### Gaps
- The CAA OR 2027 fee schedule itself (all categories, including corrugated) remains unverified.
- No CalRecycle approval notice or final CA 2027 rates (preliminary Oct 1, 2026 per prior notes) were retrieved.

---

## 9. Colorado packaging EPR: bar on disclosing EPR fees as a separate line item (NAW v. Ryan)

### Takeaway
**Still unverified.** NAW alleges that Colorado's law bars producers from telling customers about EPR fees and from listing them on invoices. It treats this as a First Amendment claim and likens it to California SB 54. Trade press repeats the allegation. The statute or rule text (HB22-1355, C.R.S. 25-17-701 et seq.; 6 CCR 1007-2) containing such a bar was **not located**. No ruling on NAW's preliminary-injunction motion was found; NAW's reply was filed Sept 28, 2026.

### Cited Findings
- **The case:** NAW v. Ryan, D. Colo. No. 1:26-cv-03460, filed July 30, 2026 by NAW (represented by NCLA) against CDPHE's executive director, with a preliminary-injunction motion.
  - Claims: unconstitutional delegation of fee-setting to CAA (a confidential methodology, with arbitration as the only recourse), compelled membership, use of dues for policy positions, and the speech restriction.
  - Sources: [NAW press release](https://www.naw.org/naw-files-colorado-epr-lawsuit/); [Waste Dive](https://www.wastedive.com/news/naw-files-lawsuit-challenging-colorado-epr-law/826698/); [Resource Recycling, 2026-07-30](https://resource-recycling.com/policy-now/2026/07/30/naw-sues-colorado-over-epr-packaging-law/) (search summaries)
- **The allegation** (search summary): "Like California's SB 54, Colorado's law also bars businesses from telling their own customers about the fees they're required to pay." Coverage of NAW's Oregon appeal says NAW claims "Colorado bars businesses from listing EPR fees on their invoices." — [NAW](https://www.naw.org/naw-files-colorado-epr-lawsuit/); [PackWorld, "NAW appeals Oregon EPR ruling to Ninth Circuit"](https://www.packworld.com/sustainable-packaging/recycling/article/22975450/naw-appeals-oregon-epr-ruling-to-ninth-circuit) (search summaries)
- **Procedure** (search summary): Colorado opposed the preliminary-injunction motion. NAW's Sept 28 reply says Colorado's defense rests on membership being voluntary and on CDPHE controlling CAA. — [MDM, "NAW's Colorado EPR Challenge Enters Next Court Phase"](https://www.mdm.com/?p=436786)
- **Statute:** the dues provision found (C.R.S. 25-17-709, per search summary) says only that "a producer shall pay producer responsibility dues to the organization based on the funding mechanism … pursuant to section 25-17-705(4)(i)" and must make related records available for inspection. No customer-disclosure language surfaced. — [colorado.public.law C.R.S. 25-17-709](https://colorado.public.law/statutes/crs_25-17-709) (search summary)
- **Related 2026 bill:** Colorado SB26-192 ("Producer Responsibility Dues Appeals Process") passed the Senate 21–12 on 2026-05-12 per a roll-call dataset; its final status is unknown. — [electionssimplified roll-call worklist (LegiScan-derived)](https://github.com/shu1513/electionssimplified/blob/main/backend/evidence/rollcall/legiscan-co-2243/survey/worklist.tsv)
- **Context conflict on Oregon:** the prior report says Oregon's law was "upheld in full" in Aug 2026 and is on appeal (9th Cir. No. 26-6404). One search summary this session said a February 2026 ruling granted NAW members preliminary relief on the compelled-membership issue. These may be different stages of the case, and neither was verified. — [O'Melveny](https://www.omm.com/insights/alerts-publications/federal-district-court-in-oregon-rejects-industry-challenge-to-state-epr-law-on-plastics-and-packaging/); [MDM](https://www.mdm.com/?p=436786) (search summaries)

### Inferences
- **Business implication for idea 5:** until counsel locates the operative text (likely in 6 CCR 1007-2 or CAA's participant terms rather than the statute), assume an itemized "Colorado EPR fee" line on customer quotes or invoices is risky. A converter-facing quote feature should therefore show EPR cost as an internal estimate or an embedded price component, not as a separately labeled pass-through charge.
- If NAW wins a preliminary injunction on the speech claim, the line-item feature becomes lawful and more valuable. Watch the D. Colo. docket.
- The restriction may sit in CAA's producer participation agreement rather than in law. If so, it binds only CAA members, which is relevant to NAW's "compelled membership" theory.

### Gaps
- The operative statutory, regulatory or contractual text barring fee disclosure was not found.
- The D. Colo. docket (CourtListener blocked) and the complaint's paragraph citing the provision were not retrieved.
- SB26-192's enactment status is unknown.
