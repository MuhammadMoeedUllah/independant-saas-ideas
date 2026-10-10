# Idea 2 business feasibility: pay-transparency cure-clock and posting-provenance tool (as of 2026-10-10)

Scope and method. This round builds on the "Idea 2" section of `reports/State compliance SaaS deep dive.md` and does not repeat it. It covers demand trajectory, insurer and law-firm channels, pricing, procurement, competitors, M&A and unit economics. I ran 30 web searches. Direct page fetches were blocked: WebFetch returned DNS errors and the proxy returned 403 for dwt.com, seyfarth.com and census.gov. Most findings below therefore come from search-result summaries, not from reading the primary pages, and should be spot-checked before anyone relies on them. One dataset was pulled directly: the Indeed Hiring Lab CSV on GitHub (raw.githubusercontent.com was reachable). Every figure carries a date. Anything marked **[unverified]** or **[assumption]** is not backed by a source I could check.

---

## 1. Demand trajectory: are WA, VA and CT suits rising, flat or falling into 2027?

### Takeaway
The prior report expected new Washington filings to fall after SSB 5408. **The evidence says the opposite.** Washington employment class-action filings kept climbing through 2025 and 2026, and job-posting (EPOA) claims make up about 40% of them. That implies roughly 290–310 posting suits in 2025, with 2026 on pace to exceed that. But the 2026 filings target **pre-amendment postings** (class periods ending July 26, 2025), which are not curable. Plaintiffs can sue on them for about three years, until roughly mid-2028. So defense spending is rising, while demand for a *forward-looking* cure-clock has no evidence behind it yet. No Virginia suit (law effective 2026-07-01) or Connecticut suit (law effective 2026-10-01) was found.

### Cited Findings
- **Washington employment class-action volume (all claim types):** Seyfarth's August 5, 2026 webinar deck says filings grew from **62 in 2021 to 718 in 2025**, and that California-based plaintiff firms have entered Washington. — [Seyfarth deck, 2026-08-05](https://www.seyfarth.com/dir_docs/documents/presentation-slides/260805-early-warning-signs-of-class-actions-proactive-strategies-for-washington-employers.pdf). A search summary of Seyfarth and DWT gives **653 filings from 2026-01-01 to 2026-08-04, projected at about 1,100 for 2026**, and puts 2025 at **765 (Seyfarth) or 773 (DWT)**. — [Seyfarth legal update](https://www.seyfarth.com/news-insights/washington-employment-class-actions-are-surging-what-employers-need-to-know.html); [DWT, Aug 2026](https://www.dwt.com/blogs/employment-labor-and-benefits/2026/08/washington-employment-class-action-surge). **The baselines conflict:** 2025 is reported as 718, 765 or 773, and 2021 as 62 or about 68. One summary attributes "2023 = 54" to DWT, which looks implausible. All 2026 counts are interim.
- **Pay-transparency share:** Seyfarth says "approximately **40% of the cases brought in 2025** included claims challenging job posting practices," many filed "by a handful of law firms using nearly identical pleadings." — [Seyfarth legal update](https://www.seyfarth.com/news-insights/washington-employment-class-actions-are-surging-what-employers-need-to-know.html). Another search summary attributes "about 40% of filings to EPOA, vs. ~32% meal-and-rest-break" to the 2026 slides **[it is unclear whether 40% describes 2025 or 2026]**. The same summary says "six plaintiffs' firms account for ~75% of all filings in 2026" **[I could not confirm which source says this]**. — [DWT](https://www.dwt.com/blogs/employment-labor-and-benefits/2026/08/washington-employment-class-action-surge)
- **Earlier cumulative counts, for comparison:** about 250 suits since the 2023 enactment, "with the Seattle-based law firm Emery Reddy leading the charge" (source within this search result set; exact attribution unverified) — [Washington Retail Assn](https://washingtonretail.org/?p=91476). A lower-quality source claims "over 300 class-action lawsuits… since June 2024, nearly all in King County Superior Court." — [Clockspot](https://www.clockspot.com/articles/pay-transparency-laws-by-state)
- **2026 filings reach back to pre-amendment postings:** Emery Reddy's Redfin complaint, filed **2026-04-21** in King County Superior Court, covers applicants to postings without pay ranges from **2023-04-03 to 2025-07-26** and seeks **$5,000 per applicant**. — [Hoodline, Apr 2026](https://hoodline.com/2026/04/seattle-s-redfin-back-in-hot-seat-over-missing-pay-in-job-ads/); [Emery Reddy](https://www.emeryreddy.com/blog/emery-reddy-in-the-news/seattle-times-reports-on-pay-transparency-lawsuit-against-redfin-filed-by-emery-reddy). Office Depot is contesting an Emery Reddy proposed class action in W.D. Wash. (January 2026). — [Emery Reddy](https://www.emeryreddy.com/blog/emery-reddy-in-the-news/office-depot-challenges-class-action-advancing-pay-transparency-rights-in-washington). For scale, Emery Reddy filed 31 EPOA suits in roughly four months of 2023. — [Trusaic](https://trusaic.com/blog/emery-reddy-files-31-pay-transparency-lawsuits-in-washington/)
- **The settlement pipeline is still active in 2026:** Lily Transportation's settlement was preliminarily approved on 2026-08-08, with claims open through 2026-11-23. Jiffy Lube and Delphinus Engineering also have open WA job-posting settlements. — [OpenClassActions, Lily](https://openclassactions.com/settlements/wage-and-hours/lily-transportation-washington-job-postings-class-action-settlement.php); [Jiffy Lube](https://openclassactions.com/settlements/jiffy-lube-washington-pay-transparency-class-action-settlement.php); [Delphinus](https://openclassactions.com/settlements/delphinus-engineering-job-postings-washington-class-action-settlement.php); [OpenClassActions WA list](https://openclassactions.com/washington-job-posting-pay-transparency-settlements.php)
- **Regulatory and legislative movement in WA:** the cure applies to postings from 2025-07-27 through 2027-07-27 (5 business days after written notice). — [Lockton](https://global.lockton.com/us/en/news-insights/washington-supreme-court-ruling-could-lead-more-epl-insurance-claims); [Hunton](https://www.hunton.com/insights/publications/wash-ruling-raises-pay-transparency-litigation-risk). L&I adopted final rules on **2026-04-21, effective 2026-05-22** (from a search summary of the Lockton, Jackson Lewis and Hunton results; **[I did not confirm which page says this]**). — [Jackson Lewis](https://www.jacksonlewis.com/node/31771). **HB 2377 (2025–26 session)** would define "applicant"; its findings say the law "should not incentivize opportunistic litigation." **Its status is not confirmed.** — [WA Legislature, HB 2377](https://lawfilesext.leg.wa.gov/biennium/2025-26/Htm/Bills/House%20Bills/2377.htm)
- **Virginia:** effective 2026-07-01. Applicants and employees may sue within **one year**. A posting violation is not actionable if the employer corrects it within **15 business days on all original posting locations**. The AG can also seek civil penalties. **No filed suit found as of 2026-10-10.** — [Virginia Mercury, 2026-07-27](https://virginiamercury.com/2026/07/27/virginias-new-pay-transparency-law-changes-the-rules-for-job-postings/); [Williams Mullen](https://www.williamsmullen.com/insights/news/legal-news/virginia-mandates-pay-transparency-and-bans-pay-history-inquiries-starting)
- **Connecticut:** private right of action, **two-year** limitations period. The remedies listed (compensatory, attorney fees, punitive) come from commentary that mixes in the older pay-secrecy law. **No suit under the 2026-10-01 posting mandate found** (the law is 10 days old). — [Barclay Damon](https://www.barclaydamon.com/alerts/the-current-state-of-connecticuts-pay-transparency-law); [Paul Hastings](https://www.paulhastings.com/insights/client-alerts/connecticut-employers-face-new-pay-transparency-and-equal-pay-requirements)
- **The noncompliance surface is shrinking only slowly.** Indeed's US share of postings with explicit pay was **49.2% (Aug 2025), 50.4% (Jun 2026), 51.1% (Jul 2026) and 51.8% (Aug 2026)**, with a 3-month average of 51.1%. — [Indeed Hiring Lab data, `pay-transparency-country.csv`](https://github.com/hiring-lab/pay-transparency) (downloaded 2026-10-10). The current series shows 40.7% for Aug 2023, while earlier press reported "50% in Aug 2023" ([HR Dive](https://www.hrdive.com/news/pay-transparency-now-appears-in-majority-of-us-job-postings/694096/)), so the **series appears to have been revised**. A New York Fed analysis of Lightcast data (Oct 2025) found that about **a quarter of listings covered by these laws omit salary**. — [Liberty Street Economics](https://libertystreeteconomics.newyorkfed.org/tag/pay-transparency/) **[snippet-level]**

### Inferences
- **The WA defense market is growing, not shrinking.** About 40% of 718–773 filings implies roughly 290–310 posting suits in 2025, more than the cumulative ~250 reported through mid-2024. If the 40% share held in 2026, there would be about 260 suits by Aug 4 and about 440 by year-end **[extrapolation]**.
- **The growth is legacy liability the product cannot cure.** The Redfin class period, starting three years before filing and ending the day before the amendment, implies a roughly three-year lookback **[I did not confirm the EPOA limitations period]**. Plaintiffs can keep mining pre-July-2025 postings until about July 2028. For those cases the useful product is **litigation support**: reconstructing which copies were employer-placed, applicant counts per posting, and exposure under the sliding scale. A forward cure-clock does not help them.
- **Forward demand for the cure-clock is unproven.** There is no evidence on how many WA cure notices are being sent for post-July-2025 postings, or how often employers miss the 5-day window. The cure **expires 2027-07-27**. After that, WA reverts to no-cure liability. That brings back demand for prevention and monitoring of liable copies but removes the WA "clock." Virginia's 15-day cure (no sunset found) becomes the main permanent cure-clock use case.
- **Rising, flat or falling into 2027:** total WA defense demand is **rising**. Demand for the forward-looking product is **flat or unknown** until (a) the first VA or CT suits appear and (b) the WA cure sunsets in July 2027.

### Gaps
- No docket-level count of EPOA filings by month, and no split by posting date (pre vs post 2025-07-27). Law360 and Bloomberg Law dockets were not accessible.
- No data on the volume of WA cure notices or demand letters for post-amendment postings.
- No VA or CT filings or demand-letter campaigns found. I searched once per state; dockets were not checked.
- HB 2377's outcome and the EPOA limitations period were not confirmed.

---

## 2. Insurer channel: how the Mineral-style bundle works, and whether carriers offer pay-transparency tools or exclusions

### Takeaway
Carriers do distribute bundled risk-management services to EPL policyholders. The usual form is **a law-firm hotline (mostly Jackson Lewis) plus an online HR portal** (Littler's HR Center, ChubbWorks), included at no extra charge. Mineral's model runs mainly through **brokers, PEOs, HCM vendors and health insurers**, with the carrier or partner paying and the employer receiving it free. **No carrier was found offering a pay-transparency monitoring tool, and no 2026 pay-transparency exclusion form was found.** Carriers are split on coverage, and underwriters are expected to examine employers' monitoring processes. That makes a correction log a plausible underwriting artifact, but nothing shows carriers paying for one.

### Cited Findings
- **Mineral's distribution:** Mineral says it partners with "more than **2,500** industry-leading insurance brokers, PEOs and HCMs." — [Mineral partners page](https://trustmineral.com/partners/). Select Health embedded Mineral in its fully insured plans, so every **2–50 employee** fully insured client in Utah and Nevada got access from **2024-01-01**. — [Mineral/Select Health](https://trustmineral.com/?p=40971); [Reworked](https://www.reworked.co/the-wire/mineral-adds-select-health-to-embed-hr-and-compliance-solutions-in-employer-sponsored-health-plans/). UnitedHealthcare offers Mineral to its groups and says that offering "is different from what brokers can offer their clients directly." — [UHC](https://e-i.uhc.com/mineral). Mineral's self-reported figure: "82% of insurance partners rate Mineral's efficiency… as significant or better." — [Mineral partners](https://trustmineral.com/partners/)
- **Mineral ownership:** Mineral is now part of **Mitratech**, a deal dated to 2024 by one source. The exact close date and terms were not found. — [Mineral/Mitratech](https://trustmineral.com/mineral-mitratech/); [3Sixty Insights](https://3sixtyinsights.com/mineral-the-ai-revolution-in-hr-compliance/)
- **What carriers bundle with EPL policies:**
  - **Markel:** a hotline staffed by Jackson Lewis EPL attorneys, a free HR website and free Jackson Lewis seminars (article undated). — [Business Insurance](https://www.businessinsurance.com/markel-launches-phone-online-services-for-epl-policyholders/)
  - **Travelers:** a "Free EPL Hotline 1-866-EPL-TRAV… provided by… Jackson Lewis" (from a 2013-copyright form, possibly dated). — [policy form PDF](https://psc.ky.gov/pscecf/2022-00050/bob.miller@straightlineky.com/04182022124620/1c_2020_General_Liability_Policy.pdf)
  - **Chubb:** a loss-prevention program with a toll-free hotline to "a nationally recognized law firm" plus ChubbWorks online tools. — [Chubb](https://www.chubb.com/us-en/business-insurance/employment-practices-liability-loss-prevention-program.html)
  - **AIG Lexington:** a Jackson Lewis risk-management helpline plus a **Littler-sponsored online HR Center**. — [Lexington](https://orgn-lex.dmp.aig.com/content/dam/lexington-insurance/america-canada/us/documents/lex-hs-lexpro-rm-epl.pdf)
  - **SECURA, Guard, Acadia, GIG and CNA** offer similar hotlines. CNA excludes EPL bought by endorsement to CNA Connect, and its line can't give advice on specific actions. — [SECURA](https://www.secura.net/risk-management/employment-practices-liability-resources); [Guard](https://www.guard.com/asc/loss-control/epli-risk-management-help-line-website/); [GIG](https://insurance.glatfelters.com/hubfs/GIG/GIG_Documents/GIG-Risk-EPLI-Helpline-FLY_101824.pdf); [CNA](https://stg-www.cna.com/sites/default/files/assets/cna-hr-helpline-flyer.pdf)
- **Premium incentives:** some carriers give **5–15% premium discounts** for documented training, and many EPLI policies include online training platforms as a value-added service. This comes from an EPLI blog that also names ThinkHR and Mineral as such providers **[secondary, restaurant-focused]**. — [LatentInsure](https://www.latentinsure.com/blog/epli-cost-factors). Small-business EPLI (<50 employees) typically costs **$800–5,000 a year**. — [QuoteSweep](https://www.quotesweep.com/blog/epli-insurance-guide)
- **Pay-transparency coverage stance (Aug 2026):** "a split has occurred." Some carriers say pay-transparency allegations are not a "wrongful act"; others cover them more broadly. — [HUB International, Aug 2026](https://www.hubinternational.com/en-us/hub-resources/proex-advocate/2026/08/pay-transparency-laws-employer-risks-and-epl-insurance-coverage/). Commentary after *Branson* expects underwriters to "focus on the processes and systems employers have in place to monitor compliance," and expects carriers to "seek to limit or preclude coverage through new exclusionary wording or amendments to the definition of 'loss.'" — [Lockton](https://global.lockton.com/us/en/news-insights/washington-supreme-court-ruling-could-lead-more-epl-insurance-claims); [Hunton/Law360](https://www.hunton.com/insights/publications/wash-ruling-raises-pay-transparency-litigation-risk) **[which firm said which is unverified]**
- **Market capacity (Q1 2026):** EPL "remains widely available"; most carriers are not cutting capacity; underwriters are focused on **pay equity**, privacy and harassment. — [CRC Group EPL REDY Index Q1 2026](https://www.crcgroup.com/Tools-Intel/Specialty-Tools-Intel/epl-redy-index-q1-2026)
- **No specific 2026 pay-transparency exclusion endorsement was found** in any public source. — (search of HUB, CRC and IIABA endorsement-trend results: [IIABA](https://www.independentagent.com/vu_resource/discover-the-endorsement-and-exclusions-filling-trends-for-2026/))

### Inferences
- **Who pays in the analog:** the carrier or distribution partner pays the vendor; the policyholder sees it as free. Carriers buy **broad, cheap, scalable** services (hotlines, portals, training) that cover thousands of small insureds. A per-requisition web-monitoring tool for 500+ employee firms does not fit that template. Those firms are mid-market and large accounts, often brokered and underwritten individually. The realistic insurer-side play is **broker-led**: specialty EPL brokers such as HUB, Lockton and CRC recommend the tool to WA-, VA- and CT-exposed clients at renewal, and the employer pays. Carrier-paid embedding is unlikely.
- Because carriers are reclassifying these claims as wage-and-hour, the employer bears the settlement cost. That raises **employer** willingness to pay, not carrier willingness. It also makes carriers less motivated to fund loss control for a risk they are writing out.
- The Mineral path (thousands of channel partners, SMB-first, embedded in health and HCM) took a venture-funded company years to build. It is **not replicable** by a 1–2 person team in the time the window allows.

### Gaps
- Mineral or ThinkHR per-policyholder wholesale pricing and named EPL carrier partners: **not found**.
- Whether any carrier asks pay-transparency questions on EPL applications, or offers premium credits for posting-compliance tooling: **not found** (supplemental applications are not public).
- Whether Hiscox, Beazley or Travelers' current programs mention pay transparency: not checked (search budget).

---

## 3. Law-firm channel: do defense firms license, resell or build compliance tech?

### Takeaway
Large employment firms do productize, but in two specific forms: **(a) content and policy platforms**, such as ComplianceHR, which is linked to Littler and offers policy, reference, document and training centers; and **(b) hotlines and HR portals sold to EPL carriers** (Jackson Lewis and Littler, see §2). European-network firms have productized pay-transparency *reporting* (Ius Laboris "GAP IQ" for the EU Directive). **No US defense firm was found offering, reselling or partnering on posting-monitoring software.** The firms are high-volume content publishers and WA class-action webinar hosts, which makes them a referral and co-marketing channel, not a reseller.

### Cited Findings
- **ComplianceHR** sells an "on-demand… suite of compliance applications" (Policy Center, Reference Center, Document Center, Training Center). Its pay-transparency activity is blogs and webinars (e.g., a March 2025 coast-to-coast pay-transparency webinar), not monitoring. The site footer links to Littler Mendelson. — [ComplianceHR pay-transparency tag](https://compliancehr.com/tag/pay-transparency-laws); [ComplianceHR, Apr 2024](https://compliancehr.com/2024/04/03/new-pay-transparency-policies/)
- **Ius Laboris** (a global employment-law alliance) offers **GAP IQ**, a pay-transparency compliance service aimed at the EU Pay Transparency Directive. — [Ius Laboris](https://iuslaboris.com/about/expertise/pay-transparency-compliance/)
- **Jackson Lewis and Littler already earn carrier-funded "risk management" revenue** via EPL hotlines and the Littler HR Center at AIG Lexington. — [Lexington](https://orgn-lex.dmp.aig.com/content/dam/lexington-insurance/america-canada/us/documents/lex-hs-lexpro-rm-epl.pdf); [Business Insurance/Markel](https://www.businessinsurance.com/markel-launches-phone-online-services-for-epl-policyholders/)
- **Seyfarth** ran a 2026-08-05 webinar for WA employers, "Early warning signs of class actions: proactive strategies," citing the EPOA filing surge. — [Seyfarth deck](https://www.seyfarth.com/dir_docs/documents/presentation-slides/260805-early-warning-signs-of-class-actions-proactive-strategies-for-washington-employers.pdf)
- Searches for Ogletree, Jackson Lewis or Seyfarth software subscriptions for pay transparency returned **nothing**. — (search on 2026-10-10; no results)

### Inferences
- **Partner or build?** Firms build where the product is *legal content* they can bill or bundle (policies, 50-state surveys, hotlines). Crawling, ATS integration and uptime are outside their core work and carry vendor-risk liability, so they are unlikely to build monitoring. They are equally unlikely to *resell* it. Firms typically avoid recommending a specific vendor in a way that looks like a referral arrangement **[ethics analysis not researched; ABA rules on fee-sharing and referrals should be checked before offering any referral fee]**.
- **Realistic law-firm channel motions:**
  - (1) **Litigation-support tool for defense counsel** on the roughly 300+ annual WA cases: posting reconstruction, applicant counts and an exposure model. Billed per matter, with the client or counsel paying as a case expense.
  - (2) **Post-settlement remediation**: settlements and demand-letter resolutions often require compliance changes. Counsel can point the client to a monitoring tool as "proof of remediation."
  - (3) **Co-hosted webinars** at each trigger date (Columbus 2027-01-01, WA cure sunset 2027-07-27, Delaware 2027-09-26).
- Mid-size WA defense firms (e.g., DWT, Perkins Coie, Stokes Lawrence, Seyfarth Seattle) are more reachable for a solo founder than Littler or Jackson Lewis national tech groups **[assumption]**.

### Gaps
- Whether Littler, Ogletree, Jackson Lewis, Fisher Phillips or Seyfarth have any tech-partner or marketplace program for third-party compliance tools: **not found**. "SeyfarthLink" and Ogletree 50-state tool details were not verified.
- No evidence on how defense counsel currently reconstruct historical posting distribution in EPOA cases (manual Wayback/aggregator pulls vs vendors).

---

## 4. Willingness to pay and pricing benchmarks

### Takeaway
Adjacent HR-compliance and comp tools sell to mid-market employers at **$5k–$40k ACV**. Vendr medians: **Textio about $24.7k, Syndio about $35k (n=2), Pave about $36.8k (n=192)**. Ongig lists **$4.9k / $14.9k / $39.9k** tiers. SixFifty-style SMB compliance runs **$1.2k–2.4k a year**, sold through payroll providers. A posting-provenance tool for 500–5,000-employee employers can plausibly price at **$10k–$25k a year**, with a sub-$5k entry tier. Pricing above about $40k would compete with full comp platforms.

### Cited Findings
- **Textio** (job-ad language and compliance): Vendr median **$24,677/yr** from 40 purchases, range about $9,945–$52,967, average savings 18%. — [Vendr Textio marketplace](https://www.vendr.com/marketplace/textio). Vendr buyer guide: average about **$30,000/yr** from 44 deals, maximum about $130,000 (conflicts with the marketplace range). — [Vendr buyer guide](https://vendr.com/buyer-guides/textio). Textio does not publish prices (checked Sept 2026). — [noon.ai](https://www.noon.ai/blog/articles/331-textio-pricing-2026)
- **Syndio** (pay equity): Vendr median **$35,000/yr**, range $33k–$37k, **n=2**, so treat it as anecdotal. — [Vendr Syndio](https://vendr.com/marketplace/syndio)
- **Pave** (comp benchmarking and planning): Vendr median **$36,750/yr**, range $9,550–$72,281, **n=192**. — [Vendr Pave](https://www.vendr.com/marketplace/pave)
- **Ongig** (JD and posting compliance, hourly salary rescans per the prior round): **Lite $4,900/yr** (100 jobs, 3 users), **Professional from $14,900/yr**, **Enterprise from $39,900/yr**, per Ongig's blog and FitGap. Another Ongig post says "starting $13,900/yr." G2 and TrustRadius say pricing is unpublished. — [FitGap](https://us.fitgap.com/products/047568/ongig); [G2](https://www.g2.com/products/ongig/pricing); [TrustRadius](https://www.trustradius.com/products/ongig/pricing)
- **SixFifty** (HR compliance docs plus a pay-transparency posting check): Employment Docs **from $200/mo ($2,400/yr)**, varying by headcount and states, with unlimited users. — [SixFifty](https://www.sixfifty.com/hr-compliance-software). SurePayroll resale tiers are **$30, $60 and $200/mo**. — [SurePayroll](https://www.surepayroll.com/employment-law). Capterra lists $1,200/yr flat. — [Capterra](https://www.capterra.com/p/206938/Return-to-Work-Toolkit-for-COVID-19/). SixFifty is also distributed through **Paychex**. — [Paychex](https://www.paychex.com/human-resources/hr-compliance)
- **Prior-round anchors (not re-verified):** the Apify checker at $5 per 1,000 postings; Trusaic at $20–80 per user per month (unverified).
- **Recurring public buyers exist:** Salt Lake County issued an RFP on 2026-05-13 for a cloud pay-equity platform covering more than 700 job classifications (responses due 2026-06-16). — [SamSearch/Cleat listing](https://www.cleat.ai/government/contracts/slco-hr130990-pay-equity-software-70bz)

### Inferences
- **Price anchors for the buyer:** TA leaders will compare the tool to Ongig and Textio ($5k–$30k). Legal will compare it to a single WA settlement ($0.4M–$4.75M, prior round) or defense fees. A **$12k–$20k/yr** core price (say about $1–1.5k a month for up to about 300 active requisitions, with jurisdiction packs) sits inside the anchor band and is less than 1% of one settlement **[assumption]**.
- The **SMB motion** (VA and CT cover employers of all sizes) is dominated by $30–$200/mo bundles sold through payroll. A solo founder cannot win there without a payroll or PEO channel.
- Willingness to pay is **event-driven**. The most motivated buyers are employers that just got sued or received a demand letter. That favors the litigation-support and remediation wedge (§3) over cold prevention selling.

### Gaps
- No Vendr or G2 pricing for Datapeople/Payscale, Pequity, Trusaic or Appcast/Joveo add-ons (search budget).
- No survey data on HR or legal willingness to pay for posting compliance specifically.

---

## 5. Sales cycle, security and procurement; ATS marketplace programs

### Takeaway
Selling to employers with 500–5,000 employees means **SOC 2 (Type II preferred) plus a DPA as a procurement gate**. Type I can be reached in weeks using compliance-automation tools; Type II needs an observation period plus a 10–16 week audit. **Greenhouse's partner program has no public listing fee.** It requires an MNDA and partnership agreement, a sandbox build, documentation, a screen recording, a beta-customer verification and Greenhouse security standards, with monthly application reviews. Lever, Workday and iCIMS terms were not verified.

### Cited Findings
- Security review is a common deal gate for HR tools. A deal "can die in procurement" without SOC 2 Type II or a completed data-processing questionnaire. SOC 2, a clear DPA and a subprocessor explanation are called "table stakes for selling to any mid-market people ops team." — [Stackmatix, GTM for HR-tech startups](https://www.stackmatix.com/blog/gtm-for-hrtech-startups) **[vendor/consultancy source]**
- Enterprise procurement teams increasingly reject Type I reports from mature vendors. Type II audits take about **10–16 weeks** (consultancy estimate). Vendors claim deals close "30–50% faster" with Type II (**unverified vendor claim**). — [iomergent](https://iomergent.com/does-soc-2-help-close-deals/); [TCSA](https://www.tcsa.in/frameworks/soc-2/for-hr-tech)
- One HR-tech vendor reached a SOC 2 **Type I in under 30 days** using a compliance platform (a single case study). — [Secureframe/Headcount365](https://secureframe.com/customers/headcount365)
- **Greenhouse Partner Program:**
  - Integration applications are reviewed on the **first Monday of each month**. Approved partners sign the Greenhouse Partnership Agreement and get **sandbox and API access**.
  - Launch requires an MNDA, integration documentation, a screen recording, verification with a beta customer and marketing assets, followed by review before a Partner Directory listing.
  - Tiers are **Official, Preferred and Alliance**. Official partners must meet Greenhouse security standards; higher tiers are chosen on customer overlap. Benefits include co-marketing, referrals and "revenue sharing."
  - **No listing fee found.**
  - Sources: [Greenhouse blog](https://www.greenhouse.com/blog/unlocking-more-value-introducing-the-new-and-improved-greenhouse-partner-program); [Greenhouse integration request form](https://www.greenhouse.com/become-a-greenhouse-partner-integration-request-form); [Partnerfleet directory](https://partner-program-directory.partnerfleet.io/partners/greenhouse-integration-partner-program)

### Inferences
- **Time and cost to "procurable":** about 1–2 months for SOC 2 Type I plus a DPA template, then about 6–9 months to a Type II report **[assumption]**. Budget about **$15k–$40k in year one** for automation tooling plus an auditor **[assumption from general market knowledge; no source this session]**.
- **Sales cycle:** no source found. For a new vendor touching candidate data, a reasonable planning assumption is **3–6 months** mid-market with a security review, and shorter (**4–8 weeks**) when counsel sponsors it after a lawsuit **[assumption]**.
- **ATS listing timeline:** at least about 1 month for application review, plus build time, plus a beta customer. So about **3–4 months** to a Greenhouse listing **[inference]**. Greenhouse's public Job Board API (prior round) means integration does not have to wait for partnership.

### Gaps
- Lever, Workday Marketplace and iCIMS Marketplace partner fees and requirements: **not researched** (search budget). Workday's marketplace is generally believed to charge partner fees, but this is **unverified**.
- No independent sales-cycle benchmarks for mid-market HR or legal compliance tools.

---

## 6. Competitor response: incumbents not checked in the prior round

### Takeaway
ATS and job-ad incumbents already handle **getting the range into the career-site copy and its crawl** (iCIMS) and the **economic case for pay in ads** (Appcast). None of the vendors checked (iCIMS, Appcast, Joveo, Textio, Workday, LinkedIn) showed **third-party copy provenance or cure-deadline workflow**. The gap is real but shallow. Ongig (hourly rescans), Payscale/Datapeople, SixFifty and programmatic vendors could each add a copy audit in a quarter or two if demand appears.

### Cited Findings
- **iCIMS:** the ATS "makes it easy… to set up the sharing of salary range data by automating the inclusion of salary data in job postings on your career site," which then "always [is] displayed… and when your jobs are crawled by Google." — [iCIMS blog](https://www.icims.com/blog/pay-transparency-how-icims-solutions-helps-you-do-it-right/)
- **Appcast:** an analysis of **10.8M jobs** found ads with pay in the title had a cost per click about **35% lower**. — [SHRM](https://shrm.org/topics-tools/news/talent-acquisition/study-pay-transparency-reduces-recruiting-costs). No Appcast or Joveo compliance feature was found in search.
- **Payscale acquired Datapeople on 2025-09-16** (terms undisclosed) "to help talent acquisition… streamline job postings." HR Brew reported monetization of some functions was "still in development." — [Payscale press release](https://www.payscale.com/press-releases/payscale-acquires-datapeople); [HR Brew](https://www.hr-brew.com/stories/2025/09/16/payscale-acquires-datapeople)
- **LinkedIn:** no official pay-range posting policy found. — (search on 2026-10-10; [AuditSocials, secondary](https://www.auditsocials.com/blog/linkedin-salary-transparency-compliance-2026-eu-pay-transparency-directive-mandatory-salary-ranges-job-postings))
- **Workday:** no pay-transparency posting feature found in search.
- Jurisdiction count keeps growing: Brightmine counts **27 US jurisdictions** with pay-transparency laws as of 2026-07-29. This includes on-request laws, and the chart's footer date conflicts. — [Brightmine](https://www.brightmine.com/us/resources/charts/u-s-pay-transparency-laws-by-state-and-locality/)

### Inferences
- **How fast incumbents could copy:** a copy audit means search plus crawling the known board and partner list, diffing against the ATS source and running a timer. That is about **1–2 quarters** of work for Ongig, Payscale or SixFifty, which already parse JDs and push to boards **[inference]**. What they lack is legal-grade **provenance evidence and counsel-facing logs**, which are slow to earn trust in. That evidence layer, not detection, is the defensible piece.
- **Programmatic vendors** (Appcast, Joveo, PandoLogic) control the paid-distribution copies, which are exactly the copies employers are liable for. If they added "pay-field pass-through verification," a large share of the liable surface would be covered at the source. That is the **biggest substitution risk** and should be watched.
- Incumbents have shown no urgency. Payscale had not even monetized Datapeople a year after the deal (per HR Brew), which suggests a 12–18 month window before a credible incumbent copy feature ships **[inference]**.

### Gaps
- PandoLogic, Pequity and Workday Recruiting pay-field behavior on syndication: not checked.
- No data on how often authorized third-party copies drop pay fields that the source included. This is the **single most important unmeasured product assumption**.

---

## 7. Exit and M&A

### Takeaway
Pay and comp acquirers exist and buy small tuck-ins at undisclosed prices: Payscale (CURO 2021, Agora, Datapeople 2025), beqom (PayAnalytics 2023) and Mitratech (Mineral, about 2024). HR-tech revenue multiples are modest, roughly **2–9x revenue** depending on quartile and segment. Talent-acquisition tools are the slowest-growing segment (about 1.8% 2026E growth). A realistic exit for a small provenance tool is a **tuck-in or acqui-hire by a posting or comp vendor at low single-digit ARR multiples**, not a venture outcome.

### Cited Findings
- **Payscale–Datapeople**, 2025-09-16, undisclosed. — [Payscale](https://www.payscale.com/press-releases/payscale-acquires-datapeople); [PrivSource](https://www.privsource.com/acquisitions/deal/6pSqr0). Payscale also bought **CURO** (pay equity, 2021) and **Agora Solutions**, and is majority-owned by Francisco Partners. — [Payscale/CURO](https://www.payscale.com/press-releases/payscale-continues-growth-trend-through-acquisition-of-pay-equity-analysis-and-compensation-management-software-leader-curo); [PrivSource Agora](https://www.privsource.com/acquisitions/deal/e4SLxw); [PrivSource Francisco Partners](https://www.privsource.com/acquisitions/deal/2VSjwE)
- **beqom–PayAnalytics** (pay equity), Dec 2023, undisclosed. — [Unleash](https://www.unleash.ai/hr-technology/beqom-focuses-in-on-pay-equity-with-payanalytics-acquisition)
- **Mitratech–Mineral** (dated 2024 by one source). — [3Sixty Insights](https://3sixtyinsights.com/mineral-the-ai-revolution-in-hr-compliance/); [Mineral](https://trustmineral.com/mineral-mitratech/)
- **Multiples:**
  - Meridian Capital, Q4 2025 HR-tech update (PitchBook as of 2025-10-07): EV/LTM revenue values that appear to be **3.6x / 6.1x / 8.6x** for bottom quartile / median / top quartile (**mapping ambiguous in extracted text**). Meridian says valuations stay resilient for companies with "compensation transparency tools." — [Meridian](https://meridianib.com/wp-content/uploads/HR-Tech_Market-Update_Q4-2025_Meridian-Capital-.pdf)
  - Citizens, Q1 2026: EV/2026E revenue of about **1.9x–4.3x** by segment (mapping ambiguous). — [Citizens Q1 2026](https://www.citizensbank.com/dam/918c3fda-847b-481e-8f9d-b42d01083c47/hr-tech-market-update-original-file.pdf)
  - Citizens, Q2 2026 (as of 2026-06-30): 2026E revenue growth of **1.8% for talent acquisition**, versus 10.2% for payroll/benefits and 8.9% for WFM/HRMS. — [Citizens Q2 2026](https://www.citizensbank.com/dam/601f2d03-ebf3-4065-907c-b491010792b8/hr-technology-q2-2026-market-update-original-file.pdf)
- Vista Point (Q4 2025): investment favored "scaled HR tech platforms with clear AI monetization and strong revenue visibility." — [Vista Point Q4 2025](https://cms.vistapointadvisors.com/system/uploads/fae/file/asset/867/HR_Tech_Quarterly_Report_Q4_2025_.pdf). Notable 2026 deals include Payoneer–Boundless and Remote–Atlas. — [Unleash, Mar 2026](https://www.unleash.ai/hr-technology/analysis/the-five-2026-hr-tech-acquisitions-that-put-hr-buyers-in-a-strong-position)

### Inferences
- **Likely acquirers:** Payscale/Datapeople, Ongig, SixFifty, Mitratech (compliance roll-up), Trusaic, Syndio, and the programmatic vendors (Appcast, Joveo).
- Public-comp multiples apply to scaled platforms. Sub-$2M-ARR tools usually trade lower, and many deals are undisclosed acqui-hires **[assumption; no micro-SaaS multiple data gathered]**.
- Exit is a bonus, not the thesis. The business must work as a cash-flowing niche product.

### Gaps
- No disclosed deal values or multiples for any pay-transparency or HR-compliance tuck-in.
- Syndio and Trusaic transactions in 2025–2026: none found.

---

## 8. Unit economics: bottom-up model for a 1–2 person team

### Takeaway
On labeled assumptions, the core market is about **3,500–5,000 multi-channel employers** with WA, VA or CT exposure. At about $15k ACV that is a **$50–75M serviceable market**. A solo founder breaks even at roughly **7–16 customers** and a two-person team at roughly **30 customers**. The first revenue could come in **Q1 2027** via paid design-partner pilots. The binding constraints are **sales velocity into legal and TA buyers, and SOC 2**, not build cost or data cost.

### Cited Findings (inputs)
- Census SUSB 2022 tables give firm counts by enterprise size, nationally and by state. **I could not download them** (census.gov returned 403 through the proxy). — [Census SUSB 2022](https://www.census.gov/data/tables/2022/econ/susb/2022-susb-annual.html). One unreliable document cites **16,845 firms with 500+ employees for 2018**. — [Scribd](https://www.scribd.com/doc/19612418/null) **[low quality; conflicts with my prior-knowledge figure of about 20–21k]**
- Small businesses (<500 employees) are 99.9% of US firms and 45.9% of employment (2023 data), so 500+ firms employ about 54% of workers. — [SBA Advocacy media kit](https://advocacy.sba.gov/wp-content/uploads/2024/10/Advocacy-Media-Kit-101624.pdf)
- Price anchors (from §4): Ongig $4.9k / $14.9k / $39.9k; Textio median $24.7k; Pave median $36.8k; SixFifty $1.2k–2.4k.
- Data COGS (prior round): about **$100–600/month** for an employer with 200 open requisitions using licensed job feeds; Greenhouse and Lever public APIs are free.
- Build effort (prior round): MVP in about **2–3 months**.

### Model (all **[assumption]** unless cited)
| # | Input | Low | High | Basis |
|---|---|---|---|---|
| A1 | US firms with 500+ employees | 17,000 | 21,000 | SUSB not downloadable; prior knowledge of about 20–21k, conflicting Scribd 16.8k |
| A2 | Share posting into ≥1 of WA/VA/CT/CA/NY/IL, including remote | 65% | 80% | These states hold a large share of employment; remote roles widen reach |
| A3 | → Addressable firms (TAM count) | ~11,000 | ~17,000 | A1×A2 |
| A4 | Core ICP share: material third-party distribution (paid boards, programmatic, staffing) **and** WA/VA/CT exposure | 25% | 35% | Judgement |
| A5 | → Core ICP firms | ~3,500 | ~5,000 | A3×A4 (rounded) |
| A6 | Core ACV | $12k | $20k | Between Ongig Pro and Textio median |
| A7 | → SAM (ARR) | ~$42M | ~$100M | A5×A6. Point estimate about $50–75M at $15k |
| A8 | Data and infra COGS per customer per year | $1.5k | $8k | Prior-round data cost plus hosting and LLM |
| A9 | Gross margin at $15k ACV | ~50% | ~90% | Plan on about 80% |
| A10 | Fixed non-salary cost per year: SOC 2 tooling and audit, cyber/E&O insurance, legal rules review, tools, events | $60k | $110k | Not sourced |
| A11 | Founder cash comp: solo ramen / solo modest / two-person | $0 / $120k / $280k | | |

**Break-even (contribution of about $12k per customer at $15k ACV and 80% GM):**
- Solo, ramen: ~$75k fixed → **about 7 customers** (about $105k ARR)
- Solo, modest salary: ~$195k → **about 16 customers** (about $240k ARR)
- Two-person: ~$375k → **about 31 customers** (about $470k ARR). At an $8k ACV, about 59 customers.
- SOM sanity check: 31 customers is about **0.6–0.9% of core ICP**.

**CAC and velocity [assumption]:**
- **Direct, founder-led:** 3–6 month cycles, about 20 active opportunities, 20–25% win rate → roughly **1–2 closes/month after month 6**, so about 30 customers by **month 18–30**. Cash CAC is low (time-dominated), but the opportunity cost is the founder's time.
- **Law-firm referral:** near-zero cash CAC. Deal flow tracks lawsuit and demand-letter events; cycles of 4–8 weeks when counsel sponsors. Volume is unpredictable, and the founder controls little.
- **Broker:** realistic only as a referral at renewal for WA-exposed accounts, with no carrier embedding (§2). Treat as upside.
- **Carrier embedding (Mineral-style):** 12+ month partner cycles and per-policyholder wholesale pricing that does not fit the 500+ segment. **Not viable** for this team.

**Time to first revenue [assumption]:**
- Q4 2026: MVP plus design partners.
- Q1 2027: paid pilots of $2–5k each, plus litigation-support engagements via counsel.
- Q2 2027: first annual contracts, gated on SOC 2 Type I and a DPA.
- 2027-07-27: the WA cure sunset is the main marketing event.

### Inferences
- The model works **if** the founder can close about 1–2 mid-market deals a month. That rate is the riskiest number in the model, and the lowest-cost way to test it is a **pre-sale campaign through 10–20 WA defense firms** before writing much code.
- A **litigation-support SKU** (per-matter posting reconstruction plus an exposure model for EPOA defense, roughly $5–15k per matter) could create revenue in Q4 2026–Q1 2027 from the rising legacy docket. At 300+ new WA cases a year, 5–10% capture means about **15–30 matters a year, roughly $0.1–0.45M** **[assumption]**.
- Revenue at plausible scale (30–60 customers, $0.45–1M ARR) is a **good lifestyle business, not a venture business**.

### Gaps
- Actual SUSB 2022 counts by enterprise size and state (WA, VA, CT, CA, NY, IL): **not retrieved**. They should be downloaded from census.gov on an unblocked network.
- No data on the share of 500+ employers using programmatic distribution or staffing agencies.
- No benchmark for mid-market HR or legal win rates or sales-cycle length.

---

## 9. Verdict: go, no-go or conditional go, and kill criteria

### Takeaway
**Conditional go, scoped narrowly and validated before the build.** The pain is real and growing. WA posting suits are running at about 300 a year or more, with settlements of $0.4M–$4.75M, insurance coverage is shrinking, and VA and CT have new private rights of action. Pricing anchors support $10k–$25k ACV, and the build is small. But the evidence does not yet show demand for the *specific* product: forward cure-clocks and provenance for authorized copies. Today's suits are about uncurable legacy postings. The WA cure ends in July 2027. Neither insurers nor law firms buy or resell such tools. Incumbents could copy the detection layer within 1–2 quarters. The founder should therefore lead with a **counsel-facing litigation-support and remediation wedge**, extend into ongoing monitoring, and stop quickly if the kill criteria trip.

### Cited Findings
- Rising WA demand: 718–773 WA employment class actions in 2025, about 40% posting-related; 653 by 2026-08-04. — [Seyfarth](https://www.seyfarth.com/news-insights/washington-employment-class-actions-are-surging-what-employers-need-to-know.html); [DWT](https://www.dwt.com/blogs/employment-labor-and-benefits/2026/08/washington-employment-class-action-surge)
- Suits target pre-amendment postings (Redfin class period ends 2025-07-26). — [Hoodline](https://hoodline.com/2026/04/seattle-s-redfin-back-in-hot-seat-over-missing-pay-in-job-ads/)
- Insurers bundle hotlines and portals, not monitoring tools; coverage for pay-transparency claims is split. — [Lexington](https://orgn-lex.dmp.aig.com/content/dam/lexington-insurance/america-canada/us/documents/lex-hs-lexpro-rm-epl.pdf); [HUB](https://www.hubinternational.com/en-us/hub-resources/proex-advocate/2026/08/pay-transparency-laws-employer-risks-and-epl-insurance-coverage/)
- Price anchors: $4.9k–$39.9k (Ongig), about $24.7k (Textio median), about $36.8k (Pave median). — [FitGap](https://us.fitgap.com/products/047568/ongig); [Vendr Textio](https://www.vendr.com/marketplace/textio); [Vendr Pave](https://www.vendr.com/marketplace/pave)
- Pay-in-posting share is still only 51.8% (Indeed US, Aug 2026). — [Indeed Hiring Lab data](https://github.com/hiring-lab/pay-transparency)

### Inferences
**Recommended scope:**
- **Wedge 1, for counsel in Q4 2026:** posting-history reconstruction and exposure modeling for active EPOA defenses, billed per matter.
- **Wedge 2, for employers from Q1 2027:** monitoring of liable copies only, a VA 15-day and WA 5-day cure clock with a notice inbox, and a counsel-exportable correction log. Sold on the remediation story ("after your settlement, prove it won't recur") and on the WA cure-sunset deadline.
- **Skip for now:** carrier embedding, a public free "exposure check" (it arms testers), and SMB self-serve.

**Kill criteria (stop or pivot if any trips):**
1. **No paid validation by 2027-01-31:** fewer than 3 signed design partners or litigation-support matters at ≥$2k each, from outreach to at least 20 WA, VA or CT defense firms and 50 sued or at-risk employers.
2. **The problem doesn't exist at measurable scale:** a 4-week data study of 100–200 employers with ranges on their career sites finds authorized third-party copies (paid boards, programmatic, agency) dropping or garbling pay fields in **<5% of copies**. That would mean the "liable copy" problem is too rare to sell.
3. **Channel silence:** no defense firm agrees to a co-webinar or referral after 60 days of outreach. Separately, if fewer than 2 of 10 EPL brokers will introduce the tool to clients, drop the broker channel.
4. **Legal regime defuses demand:** the WA legislature extends the cure past 2027-07-27 or adds a bona-fide-applicant rule (HB 2377-type), **and** no VA or CT suits or demand-letter campaigns appear by 2027-06-30.
5. **An incumbent ships it first:** Ongig, Payscale/Datapeople, SixFifty, iCIMS or a programmatic vendor (Appcast, Joveo) ships third-party copy verification with a cure workflow before the founder has 10 paying customers.
6. **Economics break:** realized ACV <$8k, data COGS >25% of ACV, or median sales cycle >6 months on the first 10 deals.
7. **Procurement wall:** more than half of qualified deals stall on SOC 2 Type II before a Type II report is achievable (about 9 months in).

**If go, the decision dates:** 2027-01-31 (validation), 2027-07-27 (WA cure sunset; target about 10 customers), and 2027-12-31 (target about 25–30 customers or about $400k ARR, otherwise wind down or sell to an incumbent).

### Gaps
- The verdict rests on search summaries. The Seyfarth and DWT filing counts, the EPOA limitations period, HB 2377's status and SUSB counts should be verified from primary sources before committing.
- The frequency of pay-field loss in authorized syndication was never measured, and it is the crux of the product's value.
