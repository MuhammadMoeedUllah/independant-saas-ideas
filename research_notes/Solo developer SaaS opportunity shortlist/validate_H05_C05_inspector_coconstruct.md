# Validation: H05 (AI report writer for solo home inspectors) and C05 (CoConstruct Exit Kit)

> **Method and dating.** Research date is 2026-10-10, and every price or fact below was retrieved that day unless another date is given. I used 35 web searches; one was rejected because reddit.com is blocked for the search tool. **Direct page fetches failed** (DNS errors on forum.nachi.org, coconstruct.com and spectora.com), so every web finding comes from **search-engine summaries of the cited page**, not from reading the page. Read each "per [Source]" as "per a search summary of [Source]". GitHub was reachable. Reddit and Facebook could not be searched or fetched. Vendor and competitor pages are marked as marketing where relevant. Rubric: `_solo_dev_rubric.md`. Corpus inputs: H05 and C05 idea files, plus the group 2 and group 3 screens.

---

## H05 Q1: Is the Spectora trigger still live? (pricing, portal ads, the $4 fee, inspector reaction, seasonality)

### Takeaway
Spectora's pricing is unchanged at $109/mo or $1,090/yr, with Advanced at **$4 per published inspection** (raised from $3; date unknown). The April 2026 "ads in client portals" trigger was Fixle warranty offers, switched on automatically on **Apr 7 2026**. It caused a real backlash, but Spectora has since **added an opt-out**, so the trigger is mostly spent. The Nov–Feb slow season is real, but it is only a season.

### Cited Findings
- **Base price:** $109/mo, or $1,090/yr. Additional inspectors cost $99/mo or $999/yr. All features are in both plans, including "AI Comment Assist". — [Spectora pricing](https://spectora.com/pricing); [Capterra Spectora pricing](https://www.capterra.com/p/157144/Spectora/pricing/); [Capterra UAE](https://www.capterra.ae/software/157144/spectora)
  - Conflict: a third-party API profile (created Jul 4 2026) lists additional inspectors at "~$89/month (~$828/year)" and base annual at "~$1,099" — [api-evangelist/spectora (GitHub)](https://github.com/api-evangelist/spectora). The vendor page wins. Unverified.
- **The $4 Advanced fee is still current.** Spectora's support article says Advanced is an optional add-on costing "$4.00 per published inspection". An older Spectora article and a NACHI forum post say $3, so the price rose at some point, but I found no announcement or date. — [Spectora support: what's included](https://support.spectora.com/en/articles/9236552-what-s-included-in-spectora-s-software); [Spectora Advanced demo (older, $3)](https://support.spectora.com/en/articles/3694075-spectora-advanced-demo-video); [NACHI forum "Spectora Pricing"](https://forum.nachi.org/t/spectora-pricing/127929)
- **Advanced gates the integrations.** It is required for Zapier, which offers only contact triggers, and for outbound webhooks ("Advanced Actions"). Spectora has **no public self-serve API**. — [api-evangelist/spectora (GitHub, Jul 2026)](https://github.com/api-evangelist/spectora)
- **What the "ads" were:** Fixle warranty and protection offers placed in the client portal next to the report. Spectora's support article says the Fixle warranty feature "was automatically enabled... for US customers starting **April 7, 2026**". The same article now says inspectors "can disable it independently in your Spectora account settings". — [Spectora support: Warranty offers by Fixle](https://support.spectora.com/en/articles/14008167-warranty-offers-by-fixle-overview-for-inspectors)
- **Inspector reaction:**
  - InterNACHI "Forced Partnership" thread, at least 10 pages long. Inspectors objected to Spectora marketing to their clients without consent. One poster said a Spectora sales rep "confirmed that FIXLE is mandatory and that you cannot opt out". A Spectora representative said the offers are Fixle-branded and clients can click "No Thanks". — [NACHI forum: Forced Partnership](https://forum.nachi.org/t/forced-partnership/266387); [page 10](https://forum.nachi.org/t/forced-partnership/266387?page=10)
  - G2: a pop-up ad was added "after a change in ownership" with about a week's notice at the start of busy season and no way to disable it. — [G2 Spectora reviews](https://g2.com/products/spectora/reviews)
    - Note: I found **no report that Spectora itself was acquired**. Spectora *acquired* HomeGauge (below), so the "ownership change" claim is unverified.
  - Capterra, Apr 2 2026: "a large number of inspectors will leave for a different software company because of this mandatory Fixle integration". Another reviewer said Fixle "is going to cause them to switch", and another was "looking into Hive". A **later** review says Spectora "caved into some public pressure and... you can opt out of it". — [Capterra Spectora reviews](https://www.capterra.com/p/157144/Spectora/reviews/)
  - An AI-generated review summary lists opt-out controls for third-party marketing as the most-requested feature. — [Marlvel review summary](https://marlvel.ai/apps/spectora-inspection-software/reviews). Low-quality aggregator.
  - Spectora's older partnerships help article said partner offers were "fully optional", and a 2023 Spectora post said partnerships could be turned off. — [Spectora support: partnerships](https://support.spectora.com/en/articles/6192116-spectora-partnerships); [Spectora: 23 reasons (2023)](https://spectora.com/r/23-reasons-to-switch-to-spectora-in-2023)
- **Consolidation:** Spectora announced its acquisition of **HomeGauge on Apr 1 2025**. Both platforms run independently, HomeGauge users are not required to switch, and pricing is unchanged "for now". — [Spectora announcement](https://www.spectora.com/r/spectora-announces-acquisition-of-homegauge); [Spectora support: what it means](https://support.spectora.com/en/articles/11003317-spectora-acquires-homegauge-what-it-means-for-you); [HomeGauge notice](https://www.homegauge.com/resources/homegauge-joins-forces-with-spectora/)
- **Seasonality (anecdotal, from inspector forums):**
  - Business slows in Nov/Dec and picks up in February. One inspector put the slow window at Thanksgiving through Feb 1.
  - A Wisconsin pattern: January is "really slow", with the peak in Mar–Jun.
  - An informal poll found the busiest month is "about 2–3X our slowest".
  - Inspectors use the slow season for marketing, team building and learning.
  - Sources: [NACHI: does inspection slow down in winter](https://forum.nachi.org/t/does-inspection-slow-down-during-winter/173446); [NACHI: seasonal patterns](https://forum.nachi.org/t/seasonal-patterns/190655); [NACHI: end-of-year volume](https://forum.nachi.org/t/end-of-year-volume-of-requests/236658); [InspectorsJournal: slow season](https://inspectorsjournal.com/topic/13409-slow-season). I could not attribute each quote to a specific thread from the summary.

### Inferences
- The "ads with no opt-out" story, the core switching trigger in the corpus, was **largely defused within weeks to months** by an opt-out. It is now a grievance, not a forcing event. Urgency drops from "live trigger" to "season plus residual distrust".
- The $4/inspection fee is real, but it only hits inspectors who choose Advanced (automations and integrations). Base Spectora has no per-inspection fee, so the corpus's "$3,389/yr" savings example rests on an optional add-on.
- Spectora now owns HomeGauge as well, which concentrates the market. A future HomeGauge sunset or forced migration would be a stronger trigger than Fixle, but none has been announced.

### Gaps
- The date of the Fixle opt-out, the date of the $3→$4 change, and how many inspectors actually left. Not available from summaries.
- A July 2026 PDF titled "Spectora Survey" on structuretech.com came up in search, but its contents could not be read: [structuretech.com Spectora-Survey.pdf](https://structuretech.com/wp-content/uploads/2026/07/Spectora-Survey.pdf).

---

## H05 Q2: Competitor sweep (incumbents, cheap tools, AI-native tools) with prices

### Takeaway
The corpus missed the most important fact: **AI report drafting is already commoditized in this niche.**
- Spectora bundles AI Comment Assist at base price.
- Hive Inspect is an "AI-first" challenger that does Spectora template import and costs about $10/mo less.
- At least six AI-native newcomers sell between $0 and $79/mo. One of them, Fielded, is **free to InterNACHI members through Dec 31 2026**.
- Legacy tools sit at $69–$89/mo.

### Cited Findings
**Incumbents and legacy (prices as listed Oct 2026; third-party listings unverified)**

| Tool | Price | Source |
|---|---|---|
| Spectora | $109/mo or $1,090/yr. Extra inspector $99/mo. Advanced $4/published inspection. AI Comment Assist included. | [Spectora pricing](https://spectora.com/pricing) |
| HomeGauge (Spectora-owned since Apr 2025) | From $89, flat rate. G2 promo: "HomeGauge ONE" at $6.90/mo for 3 months. | [Capterra HomeGauge pricing](https://www.capterra.com/p/29014/HomeGauge/pricing/) |
| Home Inspector Pro | $74/mo cloud, or $799 one-time on-premise | [G2 HIP pricing](https://www.g2.com/products/home-inspector-pro/pricing); [TrustRadius](https://trustradius.com/products/home-inspector-pro/pricing) |
| Palm-Tech | "Contact for pricing" (G2). GetApp shows "$50 per user/month" (unverified). | [G2 Palm-Tech pricing](https://www.g2.com/products/palm-tech/pricing); [GetApp](https://www.getapp.com/operations-management-software/a/palm-tech-home-insp-software/alternatives/) |
| Tap Inspect (iOS only) | $35–$99/mo (one guide); $60/mo Standard (GoodFirms, unclaimed listing) | [InspectAndTest guide](https://inspectandtest.net/guides/home-inspector-app/); [GoodFirms](https://www.goodfirms.co/software/tap-inspect) |
| Inspector Toolbelt | 5 free published reports, then $69/mo unlimited. Scheduling "FREE for life". Techjockey says $79. | [Capterra CA](https://www.capterra.ca/reviews/1023367/inspector-toolbelt); [Techjockey](https://www.techjockey.com/alternatives/spectora) |
| ISN (scheduling/back office) | Per inspection: $7.25 each for the first 50/mo, falling to $3.75 at higher tiers. ISN's Report Writer has two AI tools, including image defect detection that suggests comments. | [Capterra NZ ISN](https://www.capterra.co.nz/software/144012/inspection-support-network); [ISN blog](https://www.inspectionsupport.com/isn-home-inspection-software-features-save-time/) |
| Horizon | $79/mo Basic, flat rate, free trial | [Capterra Horizon pricing](https://www.capterra.com/p/29052/HORIZON/pricing/) |
| Property Vision (a la mode) | "Switching from Spectora" page: credit for the rest of your Spectora contract plus Spectora template import | [Property Vision: not Spectora](https://propertyvision.alamode.com/not-spectora) |
| Report Host | No pricing found | n/a |

**AI-native challengers (2025–2026; mostly vendor claims)**
- **Hive Inspect:**
  - Spectora's own comparison page calls Hive "AI-first" with "less than 1,000 inspectors". Its monthly rate is "$10 less" than Spectora's (about $99, inferred). Onboarding includes "template import". Spectora also offers guided template migration. — [Spectora vs Hive Inspect](https://www.spectora.com/spectora-and-hive-inspect-comparison) (Spectora marketing)
  - A public GitHub repo created Sep 2026, described as a "Hive Inspect take-home", is titled "Import, edit, and duplicate **Spectora** inspection report templates". This suggests Hive is actively hiring engineers for Spectora template import. — [GitHub: hive-inspect-template-importer](https://github.com/Annu-rai/hive-inspect-template-importer)
- **Fielded (Recordo, LLC):**
  - Turns photos and voice notes into a report before the inspector leaves the property.
  - **Free through Dec 31 2026 for InterNACHI members**, then $49/mo with 20% off for life.
  - Listed as an official InterNACHI vendor offer. — [InterNACHI vendor offer: Fielded](https://www.nachi.org/vendor-offers/fielded-ai-inspection-report-app-free-through-2026-then-20-off-for-life)
- **InspectorData:** AI photo analysis, a comment library, scheduling, CRM and payments. **$79/mo flat**, 45-day free trial. — [SaaSHub InspectorData](https://www.saashub.com/inspectordata)
- **Binsr Inspect:**
  - Founded 2023. Raised a pre-seed round of about $1M+ (New Stack Ventures, Silence VC).
  - Offline mode, voice input, and AI that interprets photos and places comments. Inman reviewed it on Dec 15 2025.
  - Vendor claims a 30–50% time saving.
  - Sources: [Inman tech review](https://news2.inman.com/2025/12/15/binsr-inspect-proves-ai-can-improve-transactions-tech-review/); [Binsr blog](https://binsrinspect.com/blog/ai-home-inspection-software-for-solo-inspectors)
- **InspectionX:** Photos and voice notes become a report in real time. Claims 1,100+ reports a month and a rollout to "a large U.S. home inspection franchise". — [Latitud profile](https://reveal.latitud.com/companies/inspectionx)
- **FieldScribe:** **$149 one-time license.** Photo analysis, transcription and report writing. — [DolphinVoice listing](https://dolphinvoice.ai/en/ai-apps/fieldscribe-1084454)
- **SwiftReporter:** AI template creation, writing help and photo defect identification. $12.99 per report or $39/mo. 0 reviews. — [Capterra SwiftReporter](https://www.capterra.com/p/10035853/SwiftReporter/)
- **InspectPro:** AI comment writer, label scanner, roof analyzer, voice-to-text, client and realtor portals. — [Capterra InspectPro](https://www.capterra.com/p/10037492/InspectPro/)
- **AEYES:** "Snap and move" workflow. AI files each photo's finding into a report section, with an approval queue. — [AEYES blog](https://aeyes.digitalpress.blog/streamlined-inspection-workflow/)
- **Roof Report Pro:** Roof-only AI damage tagging, $45 one-time. — [Capterra Roof Report Pro](https://www.capterra.com/p/10049961/Roof-Report-Pro/)
- **Mach One:** Presented at a Golden Gate ASHI chapter meeting. It does voice-driven retrieval of comments from a database. — [GGASHI meeting](https://ggashi.starchapter.com/meetinginfo.php?id=28)
- Spectora's 2026 buyer guide claims AI report writing cuts inspection time about 25%. It says buyers expect reporting, scheduling, payments and CRM in one platform. — [Spectora: choosing software in 2026](https://www.spectora.com/r/how-to-choose-home-inspection-software-in-2026) (vendor)

### Inferences
- Every feature in the proposed H05 wedge is now available elsewhere, often cheaper:
  - **AI drafting:** Spectora (included), Hive, Fielded, InspectorData, Binsr, SwiftReporter.
  - **Template import:** Hive, Property Vision, Spectora onboarding.
  - **Ad-free reports:** Spectora now allows an opt-out, and every competitor is ad-free.
  - **E-sign agreements and payments:** Spectora, InspectorData, ISN.
- The price floor has collapsed: free (Fielded until Dec 31 2026), $39 (SwiftReporter), $49 (Fielded later), $149 one-time (FieldScribe). A $59/mo new entrant has no price advantage and no feature advantage.
- Rubric criterion 6 (Gap versus cheap indie tools) scores **1**, and the "crowded with cheap indie tools" kill flag applies.

### Gaps
- Report Host pricing.
- Hive Inspect's exact price and funding.
- Independent quality comparisons of the AI drafting tools. No user reviews were found for most of them, and the Capterra listings show 0 reviews.

---

## H05 Q3: Buyers and reachability (counts, license lists, associations, groups)

### Takeaway
There are roughly **25k–40k US inspectors** (no official count). Spectora claims 10,000+ users. **Texas and Florida publish downloadable licensee files**, so cold outreach is cheap. InterNACHI (25.6k members) is the main gathering place, and an AI competitor already holds a free InterNACHI member offer.

### Cited Findings
- **National counts:**
  - There is no federal count. Industry estimates run "roughly 30,000 to 40,000 active home inspectors". — [InspectAndTest: becoming a home inspector](https://inspectandtest.net/guides/to-become-a-home-inspector/) (trade guide)
  - One summary cites about 25,000 U.S. firms. — [Keenable summary](https://select.keenable.ai/r/u-s-home-inspection-cycle-consolidation-inspector-sentiment/q95WOIMSCmKGPkH7TPq3xA) (low-quality aggregator)
  - An exam body said in 2007 that the number is unknown because there are no federal requirements. — [InspectorsJournal NHIE stats](https://inspectorsjournal.com/topic/4076-nhie-stats) (dated)
- **InterNACHI:** "currently 25,638 InterNACHI® members". This includes students and applicants, and is not US-only. — [InterNACHI membership stats](https://nachi.org/membership-stats.htm)
- **Spectora:** "used by more than 10,000 inspectors" (third-party profile, likely from Spectora marketing) — [api-evangelist/spectora](https://github.com/api-evangelist/spectora). **Hive:** "<1,000" (per Spectora) — [Spectora vs Hive](https://www.spectora.com/spectora-and-hive-inspect-comparison)
- **Texas (TREC):**
  - Feb 2023 license count: 4,975 inspectors, 4,287 active. — [TREC license holder count, Feb 2023](https://WWW.TREC.TEXAS.GOV/sites/default/files/pdf-forms/sr2023_02.pdf)
  - TREC's "High Value Data Sets" page links an **"Inspector License Holder Information"** open dataset on the Texas Open Data Portal, updated daily. — [TREC High Value Data Sets](https://www.trec.texas.gov/public/high-value-data-sets)
- **Florida (DBPR):**
  - DBPR offers **downloadable home inspector licensee files** (active, inactive, voluntarily inactive). — [DBPR Home Inspectors public records](https://www2.myfloridalicense.com/home-inspectors/public-records/)
  - Third-party counts conflict: 7,433 active (as of Aug 9 2026) versus "10,168 active". — [StateCreds FL guide](https://www.statecreds.com/guides/home-inspector-florida-license-data)
- **Facebook:** the only result was an "Inspector Brotherhood" Facebook group, mentioned in an InterNACHI forum post. Size unknown. — [NACHI forum](https://www.nachi.org/forum/f11/inspector-brotherhood-111570/index2.html)
- **Cross-reference:** the corpus says the market is "a few tens of thousands" of inspectors, which is consistent with the figures above — [H05 corpus file].

### Inferences
- Reachability is good: TX plus FL alone give roughly 11k–15k named licensees in public files. The pool is small, though, and saturated with vendor outreach. InterNACHI's member-benefit channel already carries a free AI report app (Fielded).
- Spectora at 10k+ out of roughly 30k means about a third of the market is on Spectora. The rest is spread across HomeGauge (also Spectora-owned), ISN, Palm-Tech, HIP, Horizon, Tap and others.

### Gaps
- ASHI membership count, the size of the inspector Facebook groups, and a current TREC count (the 2023 figure is the latest seen).
- Whether the TX and FL files include email addresses. Unknown; probably not, in which case outreach is by mail or phone, or by enriching the data.

---

## H05 Q4: Demand signals (complaints, AI adoption)

### Takeaway
2026 complaints are about **Fixle and marketing to clients** and **fees**, not about the cost of writing reports. Inspectors are adopting AI, but mainly through tools they already have or free and cheap offers.

### Cited Findings
- **Complaint themes:**
  - Fixle and marketing to clients: April 2026 Capterra reviews and the NACHI thread. — [Capterra](https://www.capterra.com/p/157144/Spectora/reviews/); [NACHI](https://forum.nachi.org/t/forced-partnership/266387)
  - Fees: "the only couple of cons I have for Spectora are the fees". — [Software Advice UK](https://www.softwareadvice.co.uk/software/263351/spectora)
  - Many 2026 reviews still call Spectora "the industry standard" and "probably one of the best in the industry". Recent reviewers describe switching **to** Spectora from HomeGauge, HIP and others. — [Capterra Spectora reviews](https://www.capterra.com/p/157144/Spectora/reviews/)
- **Spectora's response:** its replies on Capterra focused on automation and AI features and did not address Fixle. — [Capterra reviews](https://www.capterra.com/p/157144/Spectora/reviews/)
- **AI adoption signals:**
  - Spectora ships AI Comment Assist.
  - ISN has AI image defect detection.
  - InterNACHI promotes Fielded.
  - ASHI chapters host AI demos (Mach One).
  - Sources: [Spectora pricing](https://spectora.com/pricing); [ISN](https://www.inspectionsupport.com/isn-home-inspection-software-features-save-time/); [InterNACHI Fielded offer](https://www.nachi.org/vendor-offers/fielded-ai-inspection-report-app-free-through-2026-then-20-off-for-life); [GGASHI](https://ggashi.starchapter.com/meetinginfo.php?id=28)

### Inferences
- The demand that exists ("AI writes my comments") is being met inside the incumbent and by subsidized challengers. Residual Spectora distrust is what Hive, Property Vision and others are already targeting, with migration credits.

### Gaps
- No Reddit (r/HomeInspections) data: the domain is blocked for search. No Facebook group data.

---

## H05 Q5: Build feasibility (report formats, photos, offline, e-sign, pay-to-release)

### Takeaway
The pieces are buildable, but the sellable product is a mobile field app with offline capture and heavy photo handling. Inspectors also expect scheduling, agreements, payments and an agent portal around it. That is a feature-parity build, not a 4–6 week wedge.

### Cited Findings
- Buyers expect reporting, scheduling, payments and CRM in one platform. — [Spectora 2026 guide](https://www.spectora.com/r/how-to-choose-home-inspection-software-in-2026) (vendor)
- Binsr markets offline mode and voice capture as differentiators. — [Inman review](https://news2.inman.com/2025/12/15/binsr-inspect-proves-ai-can-improve-transactions-tech-review/)
- Spectora has no public API, only Advanced-gated Zapier contact triggers and outbound webhooks. Template import must therefore work from exports or PDFs. — [api-evangelist/spectora](https://github.com/api-evangelist/spectora)
- The corpus calls the MVP an "offline-first mobile report writer" and flags offline reliability in basements and crawlspaces, plus TREC and Florida OIR form accuracy — [H05 corpus file].

### Inferences
- Rubric criterion 1 (Solo build scope) scores **2**. The "offline-first mobile app" kill flag applies (partly; a PWA with local storage can ease it), and so does the feature-parity flag (scheduling, agreements, payments and agent portal are table stakes).
- E-sign and pay-to-release through Stripe Payment Links or Checkout are easy. Payouts *to the inspector* need Stripe Connect, which adds onboarding and dispute support load.

### Gaps
- The Spectora template export format (whether there is a clean JSON or CSV export, or only PDF) could not be verified.
- Typical photos per report. Not researched; no source found.

---

## H05 Q6: Verdict, refined wedge, price, first 30 days, revenue path

### Takeaway
**Verdict: DON'T BUILD.**
- The trigger has mostly expired: an opt-out was added after the Apr 7 2026 Fixle rollout.
- The AI-drafting wedge is already a commodity, from free (Fielded until Dec 31 2026) to $49–$79/mo, and it is bundled in Spectora.
- An AI-first challenger (Hive) already does Spectora template import.
- The sellable product is an offline mobile suite.

Rubric re-score: **24/40** (corpus screen 29). Kill flags: crowded with cheap indie tools; offline mobile; partial feature parity.

### Cited Findings
- AI included in Spectora's base price — [Spectora pricing](https://spectora.com/pricing)
- Fielded is free for InterNACHI members until Dec 31 2026, then $49/mo — [InterNACHI](https://www.nachi.org/vendor-offers/fielded-ai-inspection-report-app-free-through-2026-then-20-off-for-life)
- InspectorData costs $79/mo flat — [SaaSHub](https://www.saashub.com/inspectordata)
- FieldScribe costs $149 one-time — [DolphinVoice](https://dolphinvoice.ai/en/ai-apps/fieldscribe-1084454)
- SwiftReporter costs $39/mo — [Capterra](https://www.capterra.com/p/10035853/SwiftReporter/)
- Hive is AI-first, has template import and has <1,000 inspectors — [Spectora vs Hive](https://www.spectora.com/spectora-and-hive-inspect-comparison)
- Property Vision credits switchers for the rest of their Spectora contract — [Property Vision](https://propertyvision.alamode.com/not-spectora)
- The Fixle opt-out now exists — [Spectora support](https://support.spectora.com/en/articles/14008167-warranty-offers-by-fixle-overview-for-inspectors); [Capterra](https://www.capterra.com/p/157144/Spectora/reviews/)

### Inferences
**Rubric re-score (judgment):**

| Criterion | Score | Reason |
|---|---|---|
| Build | 2 | |
| Regulatory | 4 | |
| Self-serve | 4 | Template migration is the switching cost |
| Distribution | 4 | |
| Willingness to pay | 4 | |
| Gap | 1 | |
| Urgency | 2 | |
| Support and retention | 3 | |
| **Total** | **24/40** | |

**Refined wedge if the founder insists (build-if, not recommended):** Do not build a report writer. The only defensible slice I can see is a **non-mobile, desktop add-on**: "Comment Library Doctor". It imports an inspector's Spectora or HomeGauge comment library or past PDF reports, then AI-rewrites and dedupes them into a consistent, liability-safer narrative style, and exports them back into the inspector's existing tool. It is sold during the Nov–Feb template-rebuild season.
- Price: one-time $149–$249. This is anchored to FieldScribe's $149, so it is not MRR.
- Build-if: only if 10 inspectors pre-pay within 14 days of outreach.
- Unverified: whether Spectora and HomeGauge allow comment-library import and export in a usable format.

**First 30 days (validation only; stop at day 14 if the bar is missed):**
- Days 1–3:
  - Download the TREC Inspector License Holder dataset and the Florida DBPR home inspector file.
  - Pick about 300 licensees with websites. A footprint search for "spectora.com" report links on their sites can identify Spectora users (assumption).
- Days 3–10:
  - Email and DM offering a free sample: "send 3 of your comments, get them rewritten".
  - Post a before/after in the InterNACHI forum (vendor rules permitting) and in inspector Facebook groups.
- Days 10–14:
  - Stripe Payment Link pre-order. Kill if fewer than 10 paid.
  - Do not build booking, agreements or payments.

**Revenue path (if the full H05 report writer were built anyway; judgment):**

| Price | Customers for $5k MRR | Customers for $10k MRR |
|---|---|---|
| $49/mo | 103 | 205 |
| $59/mo (corpus price) | 85 | 170 |
| $79/mo | 64 | 127 |

- Comparable: Hive, an AI-first challenger with template import, sits at "<1,000" inspectors, launch date unknown. A solo founder with no inspector credibility, entering against free and bundled AI in a seasonal market, should expect **18–30+ months to $5k MRR**. **$10k MRR is not a realistic near-term target.** This is my estimate, not sourced.

### Gaps
- No Reddit or Facebook validation of willingness to pay for a third AI tool.
- Hive Inspect's growth rate and funding are unknown, which weakens the comparable.

---

## C05 Q1: The CoConstruct cutoff: exact terms, access afterward, Buildertrend's offer, exports, terms of service

### Takeaway
- **Cutoff:** CoConstruct's migration page (per the corpus, verified Sep 24 2026, and repeated by secondary sources) says **projects can be added through Mar 31 2027**. JobTread adds "migrations to Buildertrend must begin by **June 30 2027**", which I could not find on CoConstruct's own pages.
- **Access afterward:** past and current CoConstruct projects remain accessible "indefinitely".
- **Buildertrend's offer:** current CoConstruct pricing for months 1–3, then a matched Buildertrend package with "preferred customer pricing" from month 4.
- **Built-in export:** a per-project data ZIP that **excludes files and photos**.
- **API:** closed to new users.

### Cited Findings
- **The cutoff date:**
  - "Projects can still be added through March 31, 2027", after which new projects must run in Buildertrend. Historical data stays viewable. — [CoConstruct migration page](https://coconstruct.com/migration) (corpus-verified Sep 24 2026; I could not fetch it, and the Oct 10 search snippet did not show the date). Also: [Gappsy CoConstruct review](https://gappsy.com/tools/coconstruct/); [Gappsy comparison](https://gappsy.com/compare/buildertrend-vs-coconstruct/)
  - JobTread blog: no new CoConstruct projects from **Apr 1 2027**, and migrations to Buildertrend "must begin by June 30, 2027". JobTread also says Buildertrend's migration notices put the entry-level APV price at **$699/mo**. — [JobTread: leaving CoConstruct](https://www.jobtread.com/blog/leaving-coconstruct-here-is-why-builders-are-choosing-jobtread) (competitor marketing; the June 30 date and $699 are unverified)
  - CoConstruct's "when to migrate" page: teams review each account to pick a start time based on the features used, and builders who mainly use project-management features are "ready for migration today". A version of the migration page says that once a builder fully commits to Buildertrend, new projects can no longer be added in CoConstruct. — [CoConstruct: when to migrate](https://coconstruct.com/when-to-migrate); [co-construct.com/migration](https://co-construct.com/migration)
- **Access afterward:** "Access to past and current CoConstruct projects will remain indefinitely". Active projects can stay in CoConstruct until finished. A credit card is required to create the Buildertrend account. — [CoConstruct migration page](https://coconstruct.com/migration)
- **Buildertrend's migration offer:**
  - Timeline runs from day 1 to day 91. Week 1 covers data transfer and discovery.
  - "Existing customers continue current CoConstruct pricing for months one through three, then transition to a matched Buildertrend package with preferred customer pricing from month four onward".
  - Post-migration pricing and onboarding fees are listed as unknown.
  - Sources: [CoConstruct when-to-migrate](https://coconstruct.com/when-to-migrate); [rfp.wiki Buildertrend vs CoConstruct (verified Jun 2026)](https://www.rfp.wiki/specialty-industries/construction-engineering/buildertrend/coconstruct)
- **What Buildertrend migrates:** contacts, accounting codes, cost catalog, and selection, schedule and estimate templates. **Not job-specific data.** — [Projul migration guide](https://projul.com/blog/coconstruct-shutdown-migration-guide/) (competitor's summary of CoConstruct's page)
- **Not sold to new customers:** CoConstruct is no longer sold to new customers. — [rfp.wiki](https://www.rfp.wiki/specialty-industries/construction-engineering/buildertrend/coconstruct)
- **Built-in export:** Settings → Account → "Other Settings" → **"Download Project Data"**, for a single project or several. It **excludes files and photos**, and the ZIP link is emailed. — [CoConstruct: How do I get a copy of my project's data?](https://www.coconstruct.com/learn-construction-software/how-do-i-get-a-copy-of-my-projects-data)
- **API:** CoConstruct is "not establishing new API endpoints or connecting additional users to existing endpoints". Existing connections are maintained without changes. — [CoConstruct developers](https://coconstruct.com/developers). An **unofficial** third-party CoConstruct API exists: [Supergood CoConstruct API](https://supergood.ai/docs/coconstruct-api). I found no Zapier integration.
- **Buildertrend terms:**
  - The Website Services Agreement says Buildertrend has no obligation to retain, export or return data after cancellation. — [Buildertrend Website Services Agreement](https://buildertrend.com/web-services-terms-and-conditions/)
  - A third-party guide says Buildertrend can extract data **for a fee for up to one year** after a subscription ends. — [BuildBook: cancel Buildertrend](https://webflow.buildbook.co/blog/how-to-cancel-your-buildertrend-account)
  - A Buildertrend reply to a BBB complaint (Dec 9 2025) says there is no bulk "Export All" feature, but specific types of data can be exported "as outlined in our terms and conditions". — [BBB Buildertrend reviews](https://bbb.org/us/ne/omaha/profile/computer-software/buildertrend-0714-300027310/customer-reviews)
  - Buildertrend also offers API data sync and Domo reporting under a Business Insights Agreement. — [Buildertrend Business Insights Agreement](https://conference.buildertrend.com/analytics-agreement/)
- **Acquisition date conflict:** sources disagree on whether Buildertrend bought CoConstruct in Feb or Nov 2021. — [Choate](https://choate.com/insights/coconstruct-serent-capital-portfolio-company-acquired-by-buildertrend.html); [CoConstruct update](https://coconstruct.com/updates/coconstruct-has-joined-the-buildertrend-family)
- **Contradictory claim:** Projul's pages say CoConstruct "has now officially shut down". This contradicts CoConstruct's own pages and reads as competitor marketing. — [Projul migration guide](https://projul.com/blog/coconstruct-shutdown-migration-guide/)

### Inferences
- **Builders staying in the Buildertrend family need no archive tool.** Their history stays viewable "indefinitely", and templates and contacts are migrated for them. This removes much of the "archive before it's gone" fear the C05 wedge assumes.
- **The real pain is narrower.** It belongs to builders **leaving for a non-Buildertrend tool** (JobTread, Projul, Contractor Foreman and others) who will eventually cancel. When they do:
  - The built-in export omits **files and photos**.
  - Job-level data is not migrated by anyone automatically.
  - Buildertrend's terms promise nothing after cancellation.
  - Whether "indefinite" historical access survives cancelling the paid relationship is **unverified, and is the single most important fact to confirm**.
- The urgency is real and dated (Mar 31 2027, possibly Jun 30 2027), so rubric criterion 7 (Urgency) scores **5**.

### Gaps
- The exact current wording of coconstruct.com/migration on Oct 10 2026. It could not be fetched; the corpus verified it Sep 24 2026.
- Whether historical access requires an active paid account.
- The format and contents of the "Download Project Data" ZIP (CSV, XLS, PDF?).
- Whether CoConstruct's or Buildertrend's terms forbid automated access by the customer's own agent or extension. No scraping clause was found; a different vendor (BuildOps) prohibits scraping — [BuildOps ToS](https://tostracker.app/document/buildopscom-tos).

---

## C05 Q2: Competitor sweep and existing CoConstruct migration offers

### Takeaway
Funded project-management vendors already offer **free, hands-on CoConstruct migration** as a sales tool (JobTread, Projul, BuildTools and others). Fiverr freelancers sell CoConstruct-to-X data transfers. A standalone Exit Kit would compete with "free, done for you by your next vendor".

### Cited Findings
- **JobTread:** $199/mo plus $20 per internal user. Its migration path (Jun 2026) includes hands-on data help, onboarding and training. — [JobTread press release](https://www.jobtread.com/news/jobtread-opens-a-migration-path-for-builders-facing-the-coconstruct-phase-out); [JobTread CoConstruct alternative](https://www.jobtread.com/coconstruct-alternative)
- **Projul:** a migration specialist reviews your CoConstruct usage and builds a plan, then transfers the data. — [Projul: switching from CoConstruct](https://projul.com/switching-from-coconstruct/). Projul also advises exporting everything before cancelling, and warns that most platforms don't export who-did-what history. — [Projul migration guide](https://projul.com/blog/switching-construction-software-migration-guide)
- **BuildTools:** a CoConstruct migration post dated Apr 7 2026, with a gated "what to export from CoConstruct" checklist. — [BuildTools blog](https://www.buildtools.com/blog/2026-04-07-coconstruct-alternative-buildtools-migration); [BuildTools CoConstruct alternative](https://www.buildtools.com/coconstruct-alternative)
- **Others with CoConstruct landing pages or roundups:** Ressio, Buildern, Ingenious. — [Ressio LP](https://go.ressiosoftware.com/lp/co-construct); [Buildern](https://buildern.com/resources/blog/coconstruct-alternatives/); [Ingenious](https://www.ingenious.build/blog-posts/coconstruct-alternatives)
- **Fiverr gigs:** "migrate data coconstruct projul buildertrend jobtread" and "coconstruct to projul... migration data transfer". Prices were not visible. — [Fiverr gig 1](https://fiverr.com/onoiza160/migrate-data-coconstruct-projul-buildertrend-jobtread-construction-crm-builder); [Fiverr gig 2](https://fiverr.com/onoiza133/coconstruct-to-projul-migration-data-transfer-setup-construction-crm-builder)
- **Buildertrend:**
  - CostBench: Essential $339/mo, Advanced $499/mo, Complete $829/mo.
  - Projul: up to $1,099/mo.
  - The 2026 revenue-bracket model is in the corpus. JobTread claims a $699 floor for migrants.
  - Sources: [CostBench Buildertrend vs CoConstruct](https://costbench.com/compare/buildertrend-vs-coconstruct/); [Projul Buildertrend pricing](https://projul.com/blog/buildertrend-pricing-analysis-2026/); [JobTread blog](https://www.jobtread.com/blog/leaving-coconstruct-here-is-why-builders-are-choosing-jobtread)
- **Contractor Foreman:** $49–$415/mo across nine plans (as of Aug 2026), no free plan. Dupple gives $49–$332. — [CostBench Contractor Foreman](https://costbench.com/software/construction-management/contractor-foreman/); [Dupple](https://dupple.com/learn/best-construction-project-management-software)
- **Knowify:**
  - CostBench: Core $99/mo, Advanced $149/mo.
  - ITQlick: Advanced $249/mo, +$10 per user.
  - SimplyWise: $99 annual or $149 monthly, +$29 per user.
  - Sources conflict: [CostBench Knowify](https://costbench.com/software/construction-management/knowify/); [ITQlick](https://www.itqlick.com/knowify-for-field-services-software/pricing); [SimplyWise](https://www.simplywise.com/blog/?p=9887)
- **Houzz Pro:** $149/mo (Dupple) versus $399/mo (Capterra), unresolved. — [Dupple](https://dupple.com/learn/best-construction-project-management-software); [Capterra Knowify vs Houzz Pro](https://www.capterra.com/compare/135791-199689/Knowify-vs-Houzz-Pro)
- **Buildxact:** free tier; Foundation $199/mo. — [CostBench CoConstruct alternatives](https://costbench.com/software/construction-management/coconstruct/alternatives)
- **Projectmark and Builder Prime:** no pricing or CoConstruct offers found in search.

### Inferences
- The importer is a **cost center that competitors give away** to win a $199–$800/mo subscription. A solo founder charging for the same migration starts at a disadvantage, unless the product does something vendors don't:
  - a vendor-neutral archive of **files and photos** (excluded from the built-in export);
  - per-job PDF records;
  - multi-target import files.
- Fiverr gigs prove that someone is paying for manual migration, and set a likely price anchor in the low hundreds (unverified).
- Rubric criterion 6 (Gap versus cheap indie tools) scores **3**: there is a gap for vendor-neutral file and photo archiving, but not for "importer".

### Gaps
- Fiverr gig prices.
- Projectmark and Builder Prime offers.
- Whether JobTread's or Projul's migration covers files and photos.

---

## C05 Q3: Buyers, reachability and demand signals (how many CoConstruct customers remain, and where they gather)

### Takeaway
No reliable count of remaining CoConstruct customers exists. Third-party figures run from 10k customers (2020) to 602 companies tracked. They gather in places I could not search (Reddit is blocked, and I found no Facebook data). Distribution is the weakest part of C05.

### Cited Findings
- **Customer counts:**
  - Latka: "$4M revenue and 10K customers in 2020", and separately "40,000+ residential contractors" (conflicting, undated). — [Latka CoConstruct](https://getlatka.com/companies/coconstruct)
  - Enlyft: 602 companies using CoConstruct. — [Enlyft](https://enlyft.com/tech/products/coconstruct)
  - BuiltWith: 98 live websites using CoConstruct (79 US). — [BuiltWith](https://trends.builtwith.com/cms/Co-construct)
- **Product status:** CoConstruct is no longer sold to new customers (Jun 2026), so the base can only shrink. — [rfp.wiki](https://www.rfp.wiki/specialty-industries/construction-engineering/buildertrend/coconstruct)
- **Demand signals (all secondhand through competitor blogs):**
  - "Multiple Reddit users and forum posts have flagged sticker shock". One Reddit user cited the lack of Zapier, QuickBooks and Google integrations. — [Projul guide](https://projul.com/blog/coconstruct-shutdown-migration-guide/)
  - Buildertrend support quality declined after the acquisition. — [BuildTools blog](https://www.buildtools.com/blog/2026-04-07-coconstruct-alternative-buildtools-migration)
- **Corpus outreach idea:** find CoConstruct client-portal links on builder sites — [C05 corpus file]. BuiltWith detects only 98 sites, which suggests the footprint list is small.

### Inferences
- If roughly 10k accounts in 2020 shrank through churn and five years of Buildertrend migrations, the remaining base is plausibly in the **low thousands**. This is an assumption, not a sourced figure.
- Most of the remaining base will take Buildertrend's matched-pricing path and keep its history, so the addressable "leaving the Buildertrend family" segment is a fraction of that.
- Rubric criterion 4 (Distribution) scores **2**. There is no public list, the competitors outspend on SEO, and the communities could not be verified.

### Gaps
- Remaining customer count, the share already migrated, and what share are leaving the Buildertrend family entirely.
- Reddit (r/Construction, r/Remodeling, r/Contractor) and Facebook group discussion of the shutdown. Not searchable here.

---

## C05 Q4: Build feasibility (export formats, API, files and photos, terms of service)

### Takeaway
The data side is a converter plus an archive. That is buildable in 3–4 weeks **if** the ZIP format is sane. The valuable part (files and photos) is exactly what the export excludes. Getting it would mean automating the customer's own logged-in session, which carries terms-of-service and fragility risk because no new API keys are issued.

### Cited Findings
- **Export contents:** the built-in export is per project or for multiple projects, excludes files and photos, and arrives as an emailed ZIP link. — [CoConstruct help](https://www.coconstruct.com/learn-construction-software/how-do-i-get-a-copy-of-my-projects-data)
- **API:** no new API users. — [CoConstruct developers](https://coconstruct.com/developers). An unofficial API vendor exists. — [Supergood](https://supergood.ai/docs/coconstruct-api)
- **Buildertrend:** no obligation to retain or export after cancellation. — [Buildertrend terms](https://buildertrend.com/web-services-terms-and-conditions/)
- **GitHub:** a search for "coconstruct" found no open-source export tools, only unrelated projects and a third-party API profile stub ("merged into Buildertrend (2021)"). — [api-evangelist/coconstruct](https://github.com/api-evangelist/coconstruct)

### Inferences
- **MVP pieces:**
  1. A ZIP parser that normalizes to CSV and JSON.
  2. Import-ready templates for JobTread, Contractor Foreman, Buildxact and Buildertrend (contacts, cost codes, catalog, selections).
  3. A per-job PDF "closeout book" (budget, change orders, selections, daily logs).
  4. Optional: a browser extension the builder runs in their own session to save files and photos per job.
  5. Optional: a read-only "warranty vault" with shareable links.
- **Risk register:**
  - Terms of service on automated access (unverified).
  - CoConstruct UI changes breaking the extension.
  - Client PII and financial documents in the vault (low regulatory burden, but a breach is costly).
  - One-time use, so support is front-loaded.
- Rubric scores: Build 3, Regulatory 4.

### Gaps
- An actual sample of the "Download Project Data" ZIP.
- Photo and file volume per job.
- Whether builders need photos for warranty or defect claims after handover. Plausible, but no source.

---

## C05 Q5: Verdict, refined wedge, price, first 30 days, revenue path

### Takeaway
**Verdict: BUILD-IF, as a time-boxed cash project, not an MRR business.** Build only if two checks pass in week 1:
- (a) a real export ZIP shows that the data is convertible;
- (b) at least 5 builders pre-pay.

**Do not expect $5k–$10k MRR from it.** The need ends around mid-2027, the reachable pool is small, and competitors give migration away for free.

Rubric re-score: **25/40** (corpus screen 28). Kill-flag risks: one-time use, and distribution that could not be verified.

### Cited Findings
- **Hard date:** Mar 31 2027 for new projects. — [CoConstruct migration](https://coconstruct.com/migration). Possibly migration start by Jun 30 2027, per [JobTread blog](https://www.jobtread.com/blog/leaving-coconstruct-here-is-why-builders-are-choosing-jobtread) (unverified).
- **The export gap is files and photos.** — [CoConstruct help](https://www.coconstruct.com/learn-construction-software/how-do-i-get-a-copy-of-my-projects-data)
- **Free vendor migrations exist.** — [JobTread](https://www.jobtread.com/news/jobtread-opens-a-migration-path-for-builders-facing-the-coconstruct-phase-out); [Projul](https://projul.com/switching-from-coconstruct/)
- **Paid freelance migrations exist.** — [Fiverr](https://fiverr.com/onoiza160/migrate-data-coconstruct-projul-buildertrend-jobtread-construction-crm-builder)

### Inferences
**Rubric re-score (judgment):**

| Criterion | Score |
|---|---|
| Build | 3 |
| Regulatory | 4 |
| Self-serve | 4 |
| Distribution | 2 |
| Willingness to pay | 3 |
| Gap | 3 |
| Urgency | 5 |
| Support and retention | 1 |
| **Total** | **25/40** |

**Refined wedge: "CoConstruct Exit Kit: take your jobs, files and photos with you."** For builders leaving the Buildertrend family.
1. A guided bulk run of the built-in Project Data export, plus a converter that produces vendor-neutral CSV and JSON, and import files for JobTread, Contractor Foreman and Buildxact.
2. A per-job PDF closeout book.
3. A files-and-photos grabber that runs in the builder's own session. Ship it only after a terms-of-service read; otherwise it becomes a done-with-you screen-share service.
4. Optional: a read-only "Job Vault" to keep the archive searchable and shareable with past clients.

Do not build a client portal or PM features; that is the parity trap.

**Price (judgment):**
- Self-serve kit: **$399 one-time** per company, up to 50 jobs, with +$4 per extra job.
- Done-with-you: **$1,200**.
- Job Vault: **$19/mo** or $190/yr.
- Wholesale to project-management vendors or Fiverr migrators: **$150 per migration**. This is speculative; no vendor has been asked.

**First 30 days:**
- **Days 1–5:**
  - Get one real export ZIP. Offer a free conversion to 3 builders from the BuiltWith CoConstruct list ([BuiltWith](https://trends.builtwith.com/cms/Co-construct)) and from Google searches for CoConstruct client-portal links.
  - Read the Buildertrend and CoConstruct terms for automated-access clauses.
  - Ask Buildertrend support in writing whether historical access survives cancellation.
- **Days 3–10:**
  - Landing page targeting "CoConstruct export photos", "download CoConstruct data" and "CoConstruct shutdown checklist".
  - Stripe Payment Link pre-order at $399.
- **Days 7–21:**
  - Cold-email 300–500 builders found by portal footprint and NARI or HBA member directories (availability unverified).
  - Post a free "CoConstruct exit checklist" in remodeler communities (ContractorTalk, r/Contractor, Facebook remodeler groups; not verified).
- **Days 14–30:**
  - Pitch white-label conversion to the migration teams at Contractor Foreman, Buildxact, Projul and smaller vendors.
  - Pitch Fiverr migrators as resellers.
- **Kill rule:** fewer than 5 paid pre-orders by day 21.

**Revenue path (judgment; assumes a remaining base in the low thousands):**
- **One-time revenue:**
  - $5k in a month needs about 13 kits at $399, or 4–5 done-with-you jobs.
  - Capturing 1–3% of an assumed 3,000–6,000 remaining accounts (30–180 kits) gives **about $12k–$72k total one-time revenue** between Nov 2026 and about Jul 2027, then close to zero.
- **MRR from Job Vault at $19/mo:**
  - $5k MRR needs **264** subscribers; $10k needs **527**. That is implausible from this pool.
  - Realistic vault MRR is **$0.3k–$2k** after 6–9 months.
- **Bottom line:** C05 can produce fast cash in 1–3 months if the pre-sale test passes. It does **not** lead to $5k–$10k MRR on its own. Use it as a bridge, or as a lead source for a separate recurring product.

### Gaps
- All revenue figures rest on the unverified size of the remaining CoConstruct base.
- It is unverified whether builders who stay with Buildertrend (likely the majority) would pay anything at all.

---

## Cross-check against the corpus and screens (summary for the report writer)

### Takeaway
Both corpus claims hold on the facts but fail on solo viability. H05's trigger expired and its gap closed. C05's trigger is real, but the wedge is a one-time service in a shrinking pool where competitors migrate for free.

### Cited Findings
- **H05 corpus claim "portal pop-up ads with no opt-out (Apr 2026)":** true at launch on Apr 7 2026, but an opt-out now exists. — [Spectora support](https://support.spectora.com/en/articles/14008167-warranty-offers-by-fixle-overview-for-inspectors)
- **H05 corpus claim "$4 per inspection Advanced":** still true. — [Spectora support](https://support.spectora.com/en/articles/9236552-what-s-included-in-spectora-s-software)
- **C05 corpus claim "Projects can still be added through March 31, 2027":** consistent with secondary sources, but not re-fetched. — [CoConstruct migration](https://coconstruct.com/migration)
- **C05 corpus claim "CoConstruct exports are limited":** confirmed. Files and photos are excluded, and the API is closed to new users. — [CoConstruct help](https://www.coconstruct.com/learn-construction-software/how-do-i-get-a-copy-of-my-projects-data); [CoConstruct developers](https://coconstruct.com/developers)

### Inferences
- **Recommendation order for a cash-hungry solo developer:**
  - C05 Exit Kit: a short, pre-sold test (2–3 weeks of effort).
  - H05: drop it.
- **Neither reaches $10k MRR within 6–12 months on the evidence found.**

### Gaps
- This pass could not read Reddit or Facebook, and all pages were read through search summaries only. Verify anything load-bearing (the Mar 31 / Jun 30 2027 dates, historical access after cancellation, the export ZIP format, Spectora's opt-out) directly before building.
