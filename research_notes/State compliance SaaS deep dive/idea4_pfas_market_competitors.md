# Idea 4: PFAS Proof-of-Absence Network + Geo-Fenced Catalogs — Laws, Market, Competitors, Feasibility (as of 2026-10-09)

> **Method note for the report writer (read first):** This research was done on 2026-10-09. Direct page fetching (WebFetch/curl) was blocked by the sandbox's egress policy for every domain tried (saferstates.org, morganlewis.com, bdlaw.com, pca.state.mn.us, ecology.wa.gov, apps.shopify.com, walmart.com, etc.). Every finding below therefore comes from **search-engine result extracts** of the cited pages, not full-page reads. Partway through, the shared web-search budget for the session also ran out, so several planned lookups (Amazon/Costco supplier policies, Avalara/ShipperHQ, Source Intelligence, Toxnot, OEKO-TEX/bluesign PFAS rules, Oregon/Hawaii/New Hampshire detail, Maine 2026 enforcement detail) were never run. Those are listed under **Gaps**. Treat exact dates and thresholds as "verify against statute before use." Where two sources conflict, both are shown.

---

## Q1. Which US states have PFAS consumer-product restrictions, reporting or labeling rules as of Oct 2026, and what do they require?

### Takeaway
As of Oct 2026, at least 16 states have enacted bans on consumer goods containing intentionally added PFAS (Bloomberg Law, Mar 2026). Most of them phase in category bans between 2025 and 2028, and several (Maine, Minnesota, New Mexico, Illinois) then extend to almost all products in 2032. The rules are a patchwork. Effective dates and product categories differ by state. Some states define PFAS as "intentionally added", others use total-organic-fluorine (TOF) thresholds (100 ppm, then 50 ppm). Reporting runs on separate state portals (Minnesota PRISM, Connecticut DEEP form, Washington Ecology), and certificate-of-compliance and good-faith-reliance rules also differ. On top of that, states keep amending and delaying: Maine in 2024, Vermont H.238, Minnesota's deadline moved three times, Illinois pushed to 2032, and California's SB 682 was vetoed. That complexity is the core of the rules-engine value proposition.

### Cited Findings

**Overall counts and verification of claims in the brief**
- **"18 states have PFAS product restrictions": NOT VERIFIED as stated.** Bloomberg Law (Mar 18, 2026, using figures as of late Feb 2026) says "at least 16 states have now passed bans on the sale of certain types of consumer goods that contain intentionally added PFAS." It also says six states began enforcing new laws in 2026 and at least nine states had introduced new consumer-product PFAS bills for the 2026 session — [Bloomberg Law](https://news.bloomberglaw.com/litigation/expanding-state-pfas-regulations-prove-challenging-to-business); [PDF copy via Hollingsworth](https://hollingsworthllp.com/wp-content/uploads/2026/03/Feldon-Expanding-State-PFAS-Regs-prove-challenging_Bloomberg-Law_03-18-26.pdf). A count of 18 is plausible if you add states enacted later in 2026 or count food-packaging-only states, but I found no source that says 18.
- Safer States' 2026 analysis: **24 states** have adopted a common definition of PFAS as a class. At least **31 states** were expected to consider PFAS policies in 2026, and at least **17 states** were expected to consider **50 prevention policies** (product bans, disclosure) — [Safer States 2026](https://www.saferstates.org/resource/2026-analysis-of-state-policy-addressing-toxic-chemicals-and-plastics/pfas-forever-chemicals-policies-lead-in-2026/).
- MultiState (Mar 20, 2026) headline: "State PFAS Legislation in 2026: Hundreds of Bills Across 23 States." Only the headline was retrieved — [MultiState](https://www.multistate.us/insider/2026/3/20/state-pfas-legislation-in-2026-hundreds-of-bills-across-23-states).
- **"~200 PFAS-related bills per year": SUPPORTED for 2025.**
  - NCEL (May 6, 2025): at least **203 bills in 37 states**. At least 19 had advanced out of committee, and New Mexico and Virginia had enacted bills — [NCEL](https://www.ncelenviro.org/articles/confronting-forever-chemicals-states-continue-to-lead-the-way-in-2025/).
  - Safer States data via 3E (as of July 17, 2025): **36 states considering 201 bills**, and **9 states adopted 17 new PFAS policies** — [3E](https://www.3eco.com/article/states-pfas-regulations-2025/).
  - Pace Labs: **191 PFAS bills in the first four months of 2025** — [Pace Labs blog](https://blog.pacelabs.com/keeping-pace-with-analytical-services/tag/state-pfas-legislation).
  - I found no full-year 2025 total and no 2026 total.

**State-by-state matrix (verify each date against statute)**

| State | What's in force / coming | Key details for a rules engine | Sources |
|---|---|---|---|
| **Maine** (38 MRSA §1614, amended 2024) | **Jan 1, 2026 sales bans:** cleaning products, cookware, cosmetics, dental floss, juvenile products, menstruation products, textile articles (carpets/rugs and some treatments excluded), ski wax, upholstered furniture. **Jan 1, 2032:** most other products, unless a Currently Unavoidable Use (CUU) is granted. | The 2024 amendment **eliminated the general notification requirement** (originally due Jan 1, 2025). Reporting now applies only to products with a CUU determination. Manufacturers with **≤100 employees are exempt** from reporting. CUU proposals for the 2026 bans were due Jun 1, 2025. CUU proposals for the 2032 ban open Jan 1, 2027 and are due Jul 1, 2030. DEP received **11 CUU proposals** for the 2026 bans (5 cookware, 2 cleaning, 1 cosmetic container, 1 upholstered furniture, and others) and **proposed approving only 2**. | [Kelley Drye](https://www.kelleydrye.com/viewpoints/blogs/kelley-green-law/maine-dramatically-revamps-and-delays-pfas-reporting-rules-and-consumer-product-bans); [Bureau Veritas](https://www.cps.bureauveritas.com/newsroom/maine-significantly-amends-pfas-reporting-and-product-bans); [BV final rule](https://www.cps.bureauveritas.com/newsroom/maine-approves-final-rule-pfas-products); [Beveridge & Diamond](https://www.bdlaw.com/publications/precedent-to-be-set-for-state-pfas-in-products-laws-as-maine-proposes-currently-unavoidable-use-determinations-for-certain-cleaning-product-container-components/) |
| **Minnesota** (Amara's Law, Minn. Stat. §116.943) | **Jan 1, 2025:** bans in **11 product categories**. **2032:** all products with intentionally added PFAS unless CUU. **Reporting:** all products with intentionally added PFAS. | **Initial reports due Sept 15, 2026.** This deadline was extended from Jul 1, 2026, which had itself been delayed from Jan 1, 2026. Manufacturers granted a 90-day extension have until **Dec 14, 2026**. Extension and waiver requests had to be postmarked by Aug 16, 2026. Reporting runs through the **PRISM** portal. There is a **one-time $800 fee per manufacturer** (final rule Dec 2025). Annual updates are due **Feb 1**. The rule lets **suppliers report on a manufacturer's behalf**, lets a **group of manufacturers report together**, and allows grouping of similar products and reporting of **concentration ranges**. Reports become **public in PRISM** after MPCA review, except trade secrets. The 2025 amendment (SF 3, signed Jun 14, 2025) exempts PFAS only in **electronic or internal components** and exempts certain children's vehicles. | [Beveridge & Diamond](https://www.bdlaw.com/publications/minnesota-extends-pfas-in-products-reporting-deadline-to-september-15-2026/); [Pillsbury](https://www.pillsburylaw.com/en/news-and-insights/minnesota-extends-initial-pfas-deadline-september-15-2026.html); [BCLP (earlier delay)](https://www.bclplaw.com/en-US/events-insights-news/minnesota-delays-pfas-reporting-deadline-six-months-to-july-1-2026.html); [RVIA final rule](https://www.rvia.org/news-insights/minnesota-adopts-final-rules-pfas-reporting-and-fees); [MPCA PFAS reporting](https://www.pca.state.mn.us/pfas-reporting); [Clark Hill](https://www.clarkhill.com/news-events/news/pfas-in-products-minnesota-adopts-pfas-reporting-and-fees-rule/); [Greenberg Traurig Jun 2026](https://www.gtlaw.com/es/insights/2026/6/schools-out-for-summer-but-minnesotas-amaras-law); [SGS on SF 3](https://www.sgs.com/en-us/news/2025/07/safeguards-10125-minnesota-usa-revises-law-on-pfas-ban-in-products-to-include-certain-exemptions) |
| **California** | **AB 1817 (textiles), Jan 1, 2025:** bans regulated PFAS at **≥100 ppm TOF**, falling to **50 ppm on Jan 1, 2027**. Outdoor apparel for severe wet conditions is exempt until **Jan 1, 2028**, but must carry a "Made with PFAS chemicals" disclosure. **AB 2771 (cosmetics), Jan 1, 2025:** bans intentionally added PFAS. **AB 347 (signed Sep 29, 2024):** DTSC enforcement for juvenile products, textiles and food packaging. **SB 682** (cookware 2030, other products 2028) was **vetoed Oct 13, 2025**. | **Certificate of compliance: VERIFIED for textiles.** Under AB 1817, manufacturers must give a signed certificate (electronic allowed) to anyone who sells or distributes their textile articles in California. Sellers who rely on it in good faith are protected. Under **AB 347**, manufacturers must **register with DTSC by Jul 1, 2029**, pay a fee (amount not yet set), and file a **statement of compliance** for each product. DTSC must publish **accepted test methods and recognized lab accreditations by Jan 1, 2029**, and starts enforcing on **Jul 1, 2030**. | [Bureau Veritas](https://www.cps.bureauveritas.com/newsroom/california-signs-pfas-textile-articles-bill-ab-1817); [Morgan Lewis 2024](https://morganlewis.com/pubs/2024/11/new-york-and-california-bans-on-pfas-in-textiles-and-apparel-begin-january-1-2025); [BCPP AB 2771](https://www.bcpp.org/resource/california-pfas-free-cosmetics-act-ab-2771-friedman/); [BCLP AB 347](https://www.bclplaw.com/en-US/events-insights-news/pfas-update-california-enacts-new-pfas-enforcement-and-registration-law.html); [BV AB 347](https://cps.bureauveritas.com/newsroom/california-adds-enforcement-body-and-registration-certain-pfas-laws); [DLA Piper AB 347](https://www.dlapiper.com/insights/publications/2024/10/california-adds-teeth-to-pfas-laws-covering-juvenile-products-textiles-and-food-packaging); [Packaging Gateway veto](https://www.packaging-gateway.com/news/governor-vetoes-california-pfas-ban-bill-citing-affordability-issues/); [Exponent veto](https://www.exponent.com/article/governor-vetoes-californias-latest-pfas-ban) |
| **Washington** (Safer Products WA, Ch. 173-337 WAC, "Cycle 1.5") | Rule adopted **Nov 20, 2025**, effective **Dec 21, 2025**. **Restrictions from Jan 1, 2027:** apparel and accessories, automotive washes, cleaning products. Products made before that date are exempt. **Reporting** covers 9 categories: extreme/extended-use apparel, footwear, recreation and travel gear, automotive waxes, cookware and kitchen supplies, firefighting PPE, floor waxes and polishes, hard-surface sealers, ski waxes. | **"First reports due Jan 31, 2027": SUPPORTED.** Reporting covers products manufactured on or after Jan 1, 2026, and reports are due by **Jan 31** each year, so the first report is due Jan 31, 2027. That date is inferred from the rule's structure, not quoted from Ecology. **Burden-of-proof presumption:** total fluorine **above 50 ppm** is presumed to mean intentionally added PFAS, which the manufacturer can rebut with credible evidence. Penalties are up to **$5,000 per violation** for a first offense and **$10,000** for repeat offenses. | [WA Ecology](https://ecology.wa.gov/spwa-pfas); [Exponent](https://www.exponent.com/article/washington-state-adopts-new-pfas-restrictions-and-reporting); [BV](https://www.cps.bureauveritas.com/newsroom/washington-state-finalizes-cycle-15-pfas-rule); [Kelley Drye](https://www.kelleydrye.com/viewpoints/blogs/kelley-green-law/washington-state-adopts-restrictions-and-reporting-requirements-for-pfas-flame-retardants-phthalates-and-bisphenols-in-wide-range-of-consumer-products); [Eurofins](https://www.eurofins.com/textile-leather/media-centre/knowledge-e-news/tech-watch-washington-state-adopts-new-pfas-restrictions-and-reporting-requirements-under-updated-safer-products-rule/) |
| **Colorado** (PFAS Consumer Protection Act) | **Jan 1, 2026:** cleaning products, cookware, dental floss, menstruation products, ski wax, and artificial turf installation. This follows 2024–2025 bans and disclosure rules. **Jan 1, 2028:** textile articles, outdoor apparel for severe wet conditions, commercial food-service equipment (per a 2024 roundup). | Turnout gear and outdoor apparel for severe wet conditions are banned Jan 1, 2028. | [Pace Labs](https://www.pacelabs.com/analytical-environmental/pfas-in-consumer-products-new-year-new-limits-on-intentionally-added-pfas/); [Baker Hostetler](https://www.bakerlaw.com/insights/new-state-laws-limiting-the-use-of-pfas-in-consumer-products-continue-to-proliferate); [Morgan Lewis Jan 2026](https://www.morganlewis.com/pubs/2026/01/state-regulation-of-pfas-in-consumer-products-continues-to-gain-momentum-in-2026) |
| **Vermont** (S.25 2024; H.238 2025) | **Jan 1, 2026:** cosmetics, menstrual products, and other categories. **Textiles:** "regulated PFAS" means **≥100 ppm TOF** from Jan 1, 2026, falling to **50 ppm on Jul 1, 2027**. **H.238 delays:** cleaning products and dental floss moved to **Jul 1, 2027**, cookware to **Jul 1, 2028**. Outdoor apparel for severe wet conditions: **Jul 1, 2028**. | Sources conflict. Some 2026 roundups still list Vermont's cookware and cleaning-product bans as starting Jan 1, 2026, which predates H.238. | [Specialty Fabrics Review](https://specialtyfabricsreview.com/2025/06/25/vermont/); [BV](https://www.cps.bureauveritas.com/newsroom/vermont-signs-pfas-legislation-law); [Eurofins 2026 overview](https://sustainabilityservices.eurofins.com/news/pfas-regulations-overview-2026-for-consumer-products/) |
| **Connecticut** (CGS §22a-903c, 2024) | **Jul 1, 2026:** advance **written notice to DEEP** (function, purpose and amount of PFAS, filed per product or per category on the DEEP "PFAS Reporting Form for Manufacturers") **plus labeling** with DEEP-approved wording and symbols. **Jan 1, 2028:** sales ban on covered categories, whether or not the product was labeled. | Covered categories: apparel, carpets/rugs, cleaning products, cookware, cosmetics, dental floss, fabric treatments, children's products, menstruation products, textile furnishings, ski wax, upholstered furniture. Disclosure for outdoor wet-weather apparel and turnout gear began Jan 1, 2026. **Cosmetics with "unavoidable trace" PFAS are not a violation.** Products manufactured before a prohibition took effect are exempt. | [Beveridge & Diamond](https://www.bdlaw.com/publications/connecticut-pfas-consumer-product-reporting-and-labeling-requirements-are-now-in-effect/); [CBIA](https://www.cbia.com/news/issues-policies/deep-pfas-product-labels); [Shipman & Goodwin](https://www.shipmangoodwin.com/insights/connecticut-provides-required-pfas-wording-for-product-labels-on-certain-consumer-goods.html); [Benesch](https://www.beneschlaw.com/insight/connecticuts-new-pfas-rules-what-businesses-need-to-know-about-the-regulations-and-covered-product-categories/pdf/) |
| **New York** (ECL §37-0121, apparel) | **Jan 1, 2025:** ban on new apparel with intentionally added PFAS. **By Jan 1, 2027:** DEC must set a numeric limit covering intentional and unintentional PFAS. **Jan 1, 2028:** the exemption for outdoor apparel for severe wet conditions ends. | Penalties up to **$1,000 per day** of violation and up to **$2,500** for a second violation. **Sellers may rely in good faith on a manufacturer's certificate of compliance.** One law firm reads the 2028 scope more broadly (household textiles, backpacks, handbags) than DEC's own page does. | [NY DEC](https://dec.ny.gov/environmental-protection/help-for-businesses/pfas-in-apparel-law); [Venable](https://www.venable.com/insights/publications/2024/10/fashion-industry-beware-pfas-bans-on-apparel); [Morgan Lewis 2024](https://morganlewis.com/pubs/2024/11/new-york-and-california-bans-on-pfas-in-textiles-and-apparel-begin-january-1-2025) |
| **New Mexico** (HB 212 PFAS Protection Act, 2025; 20.13.2 NMAC) | The final rule was published in the NM Register on **May 5, 2026**. A CDX notice says it takes effect **Jul 1, 2026**, but that notice's dates are internally inconsistent. **Jan 1, 2027:** cookware, food packaging, dental floss, juvenile products, firefighting foam. **Jan 1, 2028:** nine more categories, including carpets, cleaning products, cosmetics, textiles. **Jan 1, 2032:** nearly all non-exempt products unless CUU. | Applies to manufacturers, distributors and retailers. Manufacturers (including importers and first domestic distributors) must determine whether PFAS is intentionally added. **Detailed PFAS content reporting begins by 2027.** CUU applications are due 12 months before the relevant ban. Sources disagree on whether dental floss and foam fall in the 2027 group. | [NMED](https://www.env.nm.gov/pfas/pfas-protection-act-hb212/); [SGS May 2026](https://www.sgs.com/news/2026/05/safeguards-07526-new-mexico-issues-rules-for-pfas-in-consumer-products); [CDX](https://public.cdxsystem.com/web/cdx/w/revised-proposed-rule-on-pfas-in-consumer-products) |
| **Rhode Island** (Consumer PFAS Ban Act, 2024) | **Jan 1, 2027:** cookware, cosmetics and other categories. **Jan 1, 2029:** artificial turf and outdoor apparel for severe wet conditions. Secondhand sales are exempt. | **"Must prove PFAS-free within 30 days if suspected": PARTIALLY VERIFIED and needs rewording.** If the department suspects a violation, the director **may** direct the manufacturer, within **30 days**, to either (a) provide a **certificate attesting** that the product has no intentionally added PFAS, or (b) notify its sellers and distributors of the ban and report who was notified. The law asks for a certificate (an attestation), not lab proof. The 2025 (H 6059) and 2026 (H 7621) bills carry the same 30-day language; I could not confirm whether either was enacted. | [TÜV SÜD 2024](https://www.tuvsud.com/en-gb/e-ssentials-newsletter/consumer-products-and-retail-essentials/e-ssentials-5-2024/usa-rhode-island-enacted-law-on-pfas-ban); [SGS 2024](https://www.sgs.com/en/news/2024/07/safeguards-10624-rhode-island-usa-regulates-pfas-in-certain-consumer-goods); [RI H 7621 (2026)](https://webserver.rilegislature.gov/BillText26/HouseText26/H7621.htm); [RI H 6059 (2025)](https://webserver.rilegislature.gov/BillText25/HouseText25/H6059.htm); [QIMA Mar 2026](https://www.qima.com/regulatory-updates/03-26) |
| **New Jersey** (S1042 "Protecting Against Forever Chemicals Act") | Enacted **Jan 12, 2026**. **Jan 12, 2028:** bans cosmetics, carpets, fabric treatments and food packaging with intentionally added PFAS. | Cookware with intentionally added PFAS must carry **English and Spanish** disclosures. The law also **restricts misleading "PFAS-free" claims**. | [Bloomberg Law](https://news.bloomberglaw.com/litigation/expanding-state-pfas-regulations-prove-challenging-to-business); [Yordas](https://www.yordasgroup.com/pfas-updates-north-america); [BHFS](https://www.bhfs.com/insight/the-evolving-pfas-landscape-state-bans-federal-standards-and-legal-exposure/). The search extract did not say which of these supplied each detail. |
| **Illinois** | **HB 2516 (amended PFAS Reduction Act)**, signed **Aug 15, 2025**, **pushed the ban to Jan 1, 2032**. It covers cosmetics, dental floss, juvenile products, menstrual products and intimate apparel. Cookware and food packaging, which were in the introduced bill's 2026 list, **were dropped**. Separately, firefighting gear needs PFAS disclosure from 2026 and is banned from 2027. | Sources conflict. One says HB 3409 became **Public Act 104-0545 (Jul 10, 2026)** with cosmetics requirements from **Jul 1, 2028**. Another (Morgan Lewis) says Illinois banned cookware, cosmetics, children's products and textiles as of Jan 1, 2026. That reading looks like the introduced bill text, not the enacted law. | [Marine Fabricator](https://marinefabricatormag.com/2025/09/02/pfas-2-2/); [Specialty Fabrics Review](https://specialtyfabricsreview.com/2025/09/02/pfas-2/); [ILGA HB 2516 text](https://ilga.gov/ftp/legislation/104/HB/10400HB2516.htm) |
| **Maryland** | **SB 273 (2022)**, from **Jan 1, 2024:** Class B foam, food packaging, rugs and carpets. Broader bills were withdrawn (HB 1022). **SB 686 (2026)** would ban PFAS in many products and require product registration; its status is unknown. | No apparel ban found. | [Intertek](https://www.intertek.com/consumer/insight-bulletins/sb-273-maryland-bans-pfas-in-several-consumer-products/); [JD Supra](https://www.jdsupra.com/legalnews/maryland-pfas-bill-withdrawn-why-1471569/); [MD Chamber](https://www.mdchamber.org/?p=64701) |
| **Oregon** | Children's products, food packaging (**Jan 1, 2025**), and cosmetics/personal care (**from 2027**, per one summary). No new 2025–26 consumer-product law found. | — | [PPAI](https://www.ppai.org/media-hub/catch-up-on-current-state-laws-regulating-pfas-chemicals/); [BCLP food packaging](https://www.bclplaw.com/en-US/events-insights-news/pfas-in-food-packaging-state-by-state-regulations.html) |
| **Hawaii** | Food packaging ban (2022 law; timing given as Dec 31, 2024). A 2025 bill would add cosmetics and personal care from 2028; I could not confirm it was enacted. | — | [PPAI](https://www.ppai.org/media-hub/catch-up-on-current-state-laws-regulating-pfas-chemicals/); [BCLP](https://www.bclplaw.com/en-US/events-insights-news/pfas-in-food-packaging-state-by-state-regulations.html) |
| **Others named in 2026 roundups** | Adherent (a vendor blog) says Illinois, Maryland, New Jersey, New Mexico, Rhode Island, **Utah and Virginia** all enacted, amended or adopted PFAS product requirements in 2026. Safer States' summary does **not corroborate** this. | Unverified | [Adherent](https://www.adherent.com/blog/which-us-states-have-enacted-or-enforced-pfas-restrictions-in-2026/) |

**Federal developments (US)**
- **EPA TSCA §8(a)(7) PFAS reporting** has been delayed repeatedly.
  - A May 2025 interim rule moved the start of the submission period from Jan 11, 2026 to Oct 13, 2026 — [Faegre Drinker](https://www.faegredrinker.com/en/insights/publications/2025/5/epa-extends-tsca-8a7-pfas-reporting-to-october-2026).
  - A final rule published **Apr 13, 2026 (91 FR 18786)** moved the start again, to the **earlier of** 60 days after a future final rule revising the PFAS reporting rule takes effect, or **Jan 31, 2027** — [J.J. Keller](https://www.jjkeller.com/news/article/EPA-delays-TSCA-Section-8-a-7-PFAS-reporting-timeline-again_id-8463a3cb-c085-4ce5-d514-8ac6bec0ff00); [Eurofins](https://www.eurofins.com/textile-leather/media-centre/knowledge-e-news/tech-watch-epa-final-rule-tsca-section-8-a-7-pfas-reporting-submission-period-delayed/); [Farella Braun](https://www.fbm.com/sarah-peterman-bell/publications/epa-further-revises-reporting-period-for-pfas-reporting-requirements-under-tsca-section-8a7/).
  - A **November 2025 proposal** would add exemptions: de minimis below 0.1%, **imported articles**, byproducts, impurities, R&D, and non-isolated intermediates. Comments closed Dec 29, 2025. As of these sources, no final substantive rule had been confirmed — [Bureau Veritas](https://www.cps.bureauveritas.com/newsroom/us-federal-pfas-updates-postponement-and-proposal).
  - Certivo, a vendor, gives "July 31, 2027" as the TSCA deadline for most manufacturers. That conflicts with the dates above — [Certivo](https://www.certivo.com/pfas).
- **Federal bill:** The Forever Chemical Regulation and Accountability Act of 2026 (**S. 4153, Durbin; H.R. 8016, McCollum**) was reintroduced in Mar 2026.
  - It would ban non-essential PFAS uses in specified consumer products (carpets, food packaging, cosmetics, textiles) within 4 years of enactment.
  - It would presume all uses non-essential within 10 years, with manufacturers carrying the burden to show a use is essential.
  - Nothing shows it advancing past introduction, and I found **no analysis of whether it would preempt state laws** — [Arnold & Porter](https://www.arnoldporter.com/en/perspectives/blogs/environmental-edge/2026/03/congress-considers-broad-pfas-legislation); [JD Supra](https://www.jdsupra.com/legalnews/congress-advances-pfas-overhaul-the-2366494/).
- Bloomberg Law (Mar 2026): federal law "doesn't generally limit PFAS in consumer goods," and EPA "currently appears unlikely to act" — [Bloomberg Law](https://news.bloomberglaw.com/litigation/expanding-state-pfas-regulations-prove-challenging-to-business).
- Broader federal rollback context: in May 2026, EPA proposed extending the PFOA/PFOS drinking-water compliance deadline and rescinding limits for four other PFAS — [Federal Register, May 20, 2026](https://www.federalregister.gov/documents/2026/05/20/2026-10086/extending-the-compliance-deadline-for-the-pfoa-and-pfos-maximum-contaminant-levels).
- FDA's MoCRA-mandated PFAS-in-cosmetics review found data gaps on use levels and dermal absorption — [Global Cosmetics News](https://www.globalcosmeticsnews.com/?p=263797).

**Rollbacks and delays (evidence of regulatory volatility)**
- **Maine (2024):** removed broad reporting and moved to CUU-only reporting with a ≤100-employee exemption — [Kelley Drye](https://www.kelleydrye.com/viewpoints/blogs/kelley-green-law/maine-dramatically-revamps-and-delays-pfas-reporting-rules-and-consumer-product-bans).
- **Minnesota:** the reporting deadline slipped from Jan 1, 2026 to Jul 1, 2026 to Sep 15, 2026, and 2025 added exemptions for electronic and internal components — [BCLP](https://www.bclplaw.com/en-US/events-insights-news/minnesota-delays-pfas-reporting-deadline-six-months-to-july-1-2026.html); [B&D](https://www.bdlaw.com/publications/minnesota-extends-pfas-in-products-reporting-deadline-to-september-15-2026/); [SGS](https://www.sgs.com/en-us/news/2025/07/safeguards-10125-minnesota-usa-revises-law-on-pfas-ban-in-products-to-include-certain-exemptions).
- **Vermont H.238 (2025):** delayed cleaning products, floss and cookware — [Specialty Fabrics Review](https://specialtyfabricsreview.com/2025/06/25/vermont/).
- **Illinois HB 2516 (2025):** moved the start from 2026 to 2032 and dropped cookware and food packaging — [Marine Fabricator](https://marinefabricatormag.com/2025/09/02/pfas-2-2/).
- **California SB 682** veto (Oct 13, 2025), on affordability grounds — [Packaging Gateway](https://www.packaging-gateway.com/news/governor-vetoes-california-pfas-ban-bill-citing-affordability-issues/).
- **Washington** chose reporting rather than bans for cookware and some other categories, which advocates criticized as delay — [WA search extract via Specialty Fabrics Review](https://specialtyfabricsreview.com/2025/12/02/washington/).

### Inferences
- **Rules-engine complexity is real and growing.** The same SKU, such as a DWR-coated rain jacket, can be:
  - legal in most states;
  - legal but needing a label in CA (until 2028) and CT (2026–27);
  - banned in ME (2026), NY (2028), CO (2028) and VT (Jul 2028);
  - subject to a TOF threshold in CA and VT that drops from 100 to 50 ppm on different dates (CA Jan 1, 2027; VT Jul 1, 2027);
  - reportable in WA (Jan 31, 2027) and MN (Sep 15, 2026, if it has intentionally added PFAS).
  
  Effective-date rules also differ: "manufactured before" exemptions (WA, CT) versus "sold after" rules. This is a real data-modeling moat, but it needs continuous legal maintenance.
- **Reporting obligations are manufacturer-level and portal-specific** (MN PRISM, CT DEEP form, WA Ecology, NM from 2027, CA DTSC registration from 2029). The "test once, reuse" idea matches how the rules work: MN explicitly lets suppliers report for manufacturers and allows group reports. Each portal still needs its own filing.
- **States keep delaying**, so a rules engine must version dates and record the source citation for each rule. "Compliance calendar" alerts are themselves valuable.
- The **2032 "all products" phases** (ME, MN, NM, IL for listed categories) are the long-term demand driver. They pull in all consumer-goods categories, not just apparel and cookware.

### Gaps
- I could not confirm **New Hampshire, Virginia, Utah** or other 2025–26 enactments (Adherent's list is uncorroborated). I also could not get a definitive current count of states with consumer-product bans; the latest firm figure is "at least 16" as of late Feb 2026.
- Minnesota's 11 categories: the source said "11" but the list was cut off. From memory, and **unverified this session**: carpets/rugs, cleaning products, cookware, cosmetics, dental floss, fabric treatments, juvenile products, menstruation products, textile furnishings, ski wax, upholstered furniture.
- Maine's 2028/2029 dates for artificial turf and outdoor wet-weather apparel were not retrieved.
- Washington's earlier Cycle 1 PFAS restrictions (carpets/rugs, aftermarket stain treatments, etc.) were not retrieved.
- Whether RI H 7621 (2026) was enacted; Illinois HB 3409 (PA 104-0545) details; Maryland SB 686 outcome; Hawaii's 2025 cosmetics bill outcome.
- The New Mexico rule's effective date and final category lists (sources conflict).
- Whether CA AB 2771 (cosmetics) or AB 652 (juvenile products) require certificates of compliance. Only AB 1817 (textiles) was confirmed.
- The EU universal PFAS restriction (ECHA) was not researched (context only, per scope).

---

## Q2. What enforcement, litigation and retailer requirements exist?

### Takeaway
State agency enforcement of PFAS product bans is still thin and mostly not public. Activity runs mainly through:
- **consumer class actions over "PFAS-free" or "non-toxic" claims**, with settlements of about $2.5M–$5M;
- **state AG consumer-protection investigations**, including in Texas, which has no PFAS ban;
- **advocacy groups scanning websites** for banned items sold into Maine;
- **retailer and marketplace rules.** Walmart Marketplace already restricts PFAS products by state and requires a manufacturer certificate for "PFAS-free" claims.

Courts have held that TOF results alone do not prove PFAS presence. That cuts both ways for a "proof-of-absence" product.

### Cited Findings

**Class actions and settlements**
- **Thinx (period underwear):** settled in early 2023 for about **$5M**. Thinx must change its marketing and **take measures to ensure PFAS are not intentionally added** — [ConsumerNotice](https://www.consumernotice.org/news/pfas-thinx-lawsuit/). The WWD URL slug says "$4 million" and notes that Knix is fighting a similar suit, so the amount conflicts — [WWD/Sourcing Journal](https://wwd.com/sourcing-journal/sustainability/thinx-settles-class-action-lawsuit-pfas-4-million-knix-menstruation-underwear-1238809483/).
- **HexClad (cookware):** **$2.5M** settlement over "PFAS-Free / PFOA-Free / non-toxic" marketing. The class covers purchases from Feb 2022 to Mar 2024, and the claims deadline was Nov 14, 2025 — [ClassAction.org](https://www.classaction.org/news/2.5m-hexclad-settlement-reached-in-false-advertising-lawsuit-over-supposedly-non-toxic-cookware).
- **E. Mishan & Sons (Gotham Steel, Granite Stone, Bell & Howell cookware):** 2026 settlement over "healthy / non-toxic" claims. The class is CA and CO buyers from Sep 8, 2021 to Jul 6, 2026, paid **$6 per product, capped at 2 per household** — [Top Class Actions](https://topclassactions.com/lawsuit-settlements/open-lawsuit-settlements/bell-howell-pfas-cookware-class-action-settlement/).
- **REI:** a class action over private-label apparel allegedly containing long-chain PFAS. REI moved to dismiss for lack of harm and lack of PFAS identification — [Retail Dive](https://www.retaildive.com/news/rei-pfas-suppliers-sustainability-climate/643740/).
- **Band-Aid (J&J/Kenvue):** a 2024 class action prompted by Mamavation testing, which found PFAS indications in 26 of 40 bandages. It was **dismissed without prejudice for lack of standing**, and plaintiffs filed an amended complaint and briefs in Sep 2025. Current status unknown — [Bloomberg Law](https://news.bloomberglaw.com/litigation/johnson-johnson-faces-class-action-after-pfas-bandages-report); [MGKF blog](https://www.mgkflitigationblog.com/new-jersey-federal-court-dismisses-pfas-consumer-suit-on-standing-grounds); [Mealey's](https://www.mealeys.com/mealeys/articles/2386541).
- **Brita:** the Ninth Circuit reportedly affirmed dismissal of a California consumer-law class action. This comes from a listing only; the date is unconfirmed — [JD Supra topic page](https://jdsupra.com/topics/product-labels/pfas/).
- **Testing evidence in court:** a 2024 decision found **TOF insufficient to show PFAS**, noting "TOF may detect organofluorine chemicals that are not PFAS" — [Mintz/MGM Law](https://mgmlaw.com/news-insights/total-organic-fluorine-found-insufficient-to-demonstrate-pfas); [Farella Braun](https://www.fbm.com/publications/pfas-or-not-tof-analysis-poses-tough-challenges-for-identifying-pfas/); [ABA, Summer 2025](https://www.americanbar.org/groups/environment_energy_resources/resources/natural-resources-environment/2025-summer/limitations-pfas-testing-consumer-products-trying-test-rest).

**AG and agency enforcement**
- **Texas AG** issued a Civil Investigative Demand to **Lululemon on Apr 13, 2026** under deceptive-trade-practices law, over alleged PFAS in apparel. Lululemon says it phased PFAS out in 2023 and **requires vendors to test regularly through third-party agencies** — [Foley](https://www.foley.com/p/102mq7l/texas-attorney-general-investigates-lululemon-over-alleged-forever-chemicals-in/); [ESG Dive](https://www.esgdive.com/news/texas-ag-probes-lululemon-over-alleged-use-of-pfas-in-activewear/817720/). **No HydroFlask PFAS case was found.**
- **New York AG (Jul 2026)** sued PFAS manufacturers under environmental and consumer-protection law, seeking penalties and **orders requiring warnings on PFAS-containing products** — [Buchalter](https://www.buchalter.com/blogs/new-york-ag-targets-major-pfas-manufacturers-in-consumer-products-lawsuit/).
- **Maine (2026):** after the Jan 2026 bans took effect, a nonprofit **found websites and stores selling newly banned items and referred them to Maine DEP** for investigation. This is from a search summary; the organization and the outcome were not retrieved — [Alston & Bird Q1 2026](https://www.alston.com/en/insights/publications/2026/04/pfas-primer-quarterly-update-2026-q1); [Bloomberg Law](https://news.bloomberglaw.com/litigation/expanding-state-pfas-regulations-prove-challenging-to-business).
- **Industry challenge failed:** the Cookware Sustainability Alliance sued to block Minnesota's cookware ban. A preliminary injunction was **denied Feb 25, 2025**, and the case was **dismissed Aug 11, 2025**; the court held the law does not discriminate against interstate commerce. I found no appeal — [Packaging Law](https://www.packaginglaw.com/news/court-dismisses-cookware-alliances-lawsuit-challenging-mn-ban-cookware-containing-added-pfas); [Bergeson & Campbell](https://www.lawbc.com/federal-court-grants-minnesotas-motion-to-dismiss-challenge-to-its-pfas-ban-in-cookware/); [ArentFox Schiff](https://www.afslaw.com/perspectives/consumer-products-watch/bans-pfas-cookware-litigation-and-legislative-challenges).

**Retailer and marketplace policies**
- **Walmart Marketplace:** restricts sales of covered products containing intentionally added PFAS **in states that restrict them**. Sellers may claim "free of intentionally added PFAS" **only with a manufacturer certificate**. The guide was last updated Jan 7, 2025 — [Walmart Marketplace Learn](https://marketplacelearn.walmart.com/guides/prohibited-products-policy-pfas-chemicals).
- **REI:** required vendors to phase PFAS out of cookware and textiles. Products covered by California law had to be PFAS-free by 2024 and **all other textiles by 2026** — [Retail Dive](https://www.retaildive.com/news/rei-pfas-suppliers-sustainability-climate/643740/).
- **Dick's Sporting Goods:** added PFAS to its restricted-substance list for own-brand textiles, applying to all vendors — [Retail Dive](https://retaildive.com/news/dicks-bans-forever-chemicals-in-its-brand-textile-products/653766).
- **Target:** its safer-chemicals policy restricts some PFAS in certain textiles. **Amazon** is listed among retailers with PFAS phase-out policies for food packaging and/or products. In Toxic-Free Future testing, none of ten retailers, including Amazon and Costco, was fully PFAS-free — [Toxic-Free Future](https://toxicfreefuture.org/blog/major-retailers-phasing-out-worst-of-the-worst-chemicals/).

### Inferences
- **Walmart Marketplace's state-by-state restriction confirms the "geo-fenced catalog" concept.** Marketplaces are already doing it, so third-party sellers and DTC brands on Shopify and other platforms need a comparable control.
- **Proof-of-absence is directly valuable in litigation.** Every settlement above came from marketing claims ("PFAS-free", "non-toxic"). Documented, lot-linked test evidence protects against deceptive-marketing claims and AG CIDs, including in states with no PFAS ban (Texas). NJ S1042 also restricts misleading "PFAS-free" claims.
- **The Maine nonprofit web-scanning shows e-commerce listings are the enforcement surface.** A checkout block that stops banned SKUs from shipping to banned states reduces exposure.
- Courts' skepticism of TOF as proof of *presence* means a **TOF non-detect is strong evidence of *absence*.** But regulators in WA (above 50 ppm presumption) and CA/VT (100 then 50 ppm thresholds) use TOF for enforcement, so a positive TOF result creates a rebuttal burden on the brand.

### Gaps
- Current **Amazon, Costco, Target and Walmart (corporate) supplier PFAS certification requirements**: searches ran out before these were retrieved. Their documents should be checked directly.
- No public **state-agency notices of violation or penalties** under any PFAS product ban were found for ME, MN, CO, WA, CA or NY as of Oct 2026. This may reflect what is indexed rather than what has happened.
- I found no recall or retailer delisting tied specifically to a state PFAS ban, and no quantified cost of noncompliance per SKU.

---

## Q3. How big is the market and who are the buyers?

### Takeaway
I found no reliable count of affected brands or SKUs. The best proxy is Minnesota PRISM: about 500, then 700+ companies had registered before the Sept 15, 2026 deadline, but reporting only covers products that *contain* intentionally added PFAS. Brands that are PFAS-free file nothing, yet those are exactly the buyers of proof-of-absence.

Estimates of the PFAS testing market vary widely by scope: about $0.2B for US testing (2025) and about $0.5–1.0B globally for testing services (2025), growing roughly 10–15% a year. Broader "analysis workflow" definitions reach $3B+.

Per-sample costs set the economics of reusing one test across many brands:
- TOF screening: about €250–350 (roughly $270–380) per sample;
- targeted LC-MS/MS: $400–700 per sample.

### Cited Findings
**Proxies for the number of affected companies**
- Minnesota PRISM: "**over 700 companies have registered** … over 30 companies have successfully submitted reports months ahead of schedule." The MPCA release date is unclear, likely mid-2026 — [MPCA news](https://www.pca.state.mn.us/news-and-stories/groundbreaking-reports-on-pfas-in-products-are-due-three-months-from-today). An earlier count was "more than **500** companies registered … **18** manufacturers submitted" — [RV PRO](https://rv-pro.com/news/minnesota-pollution-control-agency-reaffirms-pfas-reporting-deadline/).
- Assent claims the following (vendor claims, unverified):
  - nearly **1 million PFAS declarations** gathered through its platform — [Assent](https://www.assent.com/?p=61638);
  - **695+ unique PFAS** found across supply chains, drawn from **4.5 million supplier declarations** (Sep 15, 2025) — [Supply Chain Dive press release](https://www.supplychaindive.com/press-release/20250915-assent-uncovers-over-695-unique-pfas-across-global-supply-chains-as-regulat).
- Sphera's **BOMcheck** handles data for **over 10 million parts** (vendor webinar claim) — [Sphera](https://sphera.com/resources/events/navigating-pfas-regulations-ensuring-supply-chain-compliance).

**PFAS testing market size (all paid-report summaries; scopes differ)**
- US PFAS testing market: **$199.16M in 2025**, 14.4% CAGR for 2026–2035 — [DataM Intelligence](https://www.datamintelligence.com/research-report/u-s-pfas-testing-market).
- Global: **$780.0M in 2025**, 9.8% CAGR for 2026–2036 — [Meticulous Research](https://www.meticulousresearch.com/product/pfas-testing-market-6901).
- Global: **$537.89M in 2025**, rising to $2,090.58M by 2035 at a 14.54% CAGR — [Towards Healthcare](https://www.towardshealthcare.com/insights/pfas-testing-market-sizing).
- Global: **$969.5M by 2030** at a 14.5% CAGR — [MarketsandMarkets via PR Newswire](https://prnewswire.co.uk/news-releases/pfas-testing-market-worth-us969-5-million-by-2030-with-14-5-cagr--marketsandmarkets-302392700.html).
- Broader definition: **$3.23B in 2025**, rising to $5.13B by 2029 at a 12.6% CAGR — [CB Insights (citing a market research firm)](https://www.cbinsights.com/company/enthalpy-analytical).
- Caveat: most of these totals are dominated by **water and environmental** testing, not consumer-product testing.

**Testing costs per sample (pricing benchmarks for the attestation layer)**
- Measurlabs, TOF in paper, polymers and textiles: **€250–350 per sample plus a €97 fee per order**. It needs 50 g of sample and has a 5 mg/kg limit of detection — [Measurlabs](https://measurlabs.com/products/total-organic-fluorine-tof-content-in-paper).
- Scion Research, TOF: about **NZ$1,100 for a single sample**, falling to about **NZ$295 per sample for 30+ samples**, with a 10 ppm detection limit for solids — [Scion](https://www.scionresearch.com/services/laboratory-services/pfas-testing-services).
- HQTS: PIGE and CIC screening cost "**a few hundred dollars**" per sample, and targeted **LC-MS/MS costs $400–700** per sample — [HQTS](https://www.hqts.com/?p=183995).
- Venture activity: PFAS *testing technology* startup **Biota raised a $3M seed** round (Jul 29, 2026, Burnt Island Ventures) — [VCA Online 2026 archive](https://www.vcaonline.com/news/archive/2026/).

**Buyer segments signalled by the laws**
- Apparel and textiles (CA, NY, ME, VT, CO 2028, WA 2027, CT 2028).
- Outdoor gear (wet-weather apparel; WA reporting covers "gear for recreation and travel" and "extreme and extended use apparel").
- Cookware (MN, ME, CO bans; WA reporting; NJ labeling; a CA ban vetoed).
- Cosmetics (CA, MN, ME, VT, NM 2028, NJ 2028, IL 2032).
- Children's and juvenile products, carpets and rugs, upholstered furniture, cleaning products, ski wax, dental floss, menstrual products.
- Sources: see the Q1 matrix — e.g., [B&D Connecticut](https://www.bdlaw.com/publications/connecticut-pfas-consumer-product-reporting-and-labeling-requirements-are-now-in-effect/); [WA Ecology](https://ecology.wa.gov/spwa-pfas).

### Inferences
- **Reuse economics.** With a TOF screen at about $300–400 and an LC-MS/MS confirmation at $400–700, one test of a shared component (for example, a mill's DWR-free fabric or a supplier's coating) costs a few hundred to about $1,100. Shared across 10+ brands, the per-brand cost falls below $100. This saving is real but small per test. The larger value is **avoiding repeat tests across hundreds of SKUs and many components**: a brand with 500 SKUs × 3 materials could otherwise face roughly $450k–$1M+ in testing. That figure is my own arithmetic, not a sourced estimate.
- The PFAS testing market (about $0.2B US) is mostly environmental. Consumer-product compliance software sits in a different budget (product compliance and regulatory affairs). Pure TAM sizing from lab-market reports would overstate or misstate the opportunity.
- The ~700 Minnesota registrants are **PFAS-*containing*** manufacturers, mostly industrial. The proof-of-absence buyer is the much larger group of **brands claiming or needing PFAS-free status** — DTC apparel, outdoor, cookware, beauty and kids' brands — and **retailers and marketplaces** that need certificates from sellers.

### Gaps
- No credible count of brands or SKUs in the target categories (US apparel brands, outdoor brands, cookware brands, cosmetics brands selling into regulated states). Trade associations (AAFA, OIA, Cookware Sustainability Alliance, PCPC) were not reached.
- No final Minnesota report count after Sept 15, 2026, and no MPCA rulemaking estimate (from the SONAR) of the number of affected manufacturers.
- No consumer-product-specific PFAS testing market size.
- No data on how often brands currently test (per style, per season, per lot).

---

## Q4. What does the competitive landscape look like?

### Takeaway
No direct competitor was found that combines (1) a **shared, reusable component-level PFAS test-certificate network** with (2) a **state-by-state SKU rules engine plugged into e-commerce checkout**. The space is split into four groups:
- **Enterprise supplier-declaration and regulatory-content platforms:** Assent, 3E, UL ULTRUS/WERCSmart, Enhesa, Sphera/BOMcheck, and the newer AI-native Certivo. These are custom-priced, enterprise-focused, and built mostly on declarations rather than lab tests.
- **Testing and certification bodies with PFAS-free marks:** Intertek (launched May 2025, TOF below 20 ppm) and SGS ("No PFAS Detected").
- **Industry data-sharing networks without a PFAS focus:** ZDHC Gateway (textiles), Novi (beauty).
- **Generic Shopify geo-restriction apps** at $10–50 a month, which enforce whatever rules the merchant types in and carry no PFAS legal content.

### Cited Findings

**Enterprise product-compliance and supply-chain data platforms**
- **Assent**
  - The PFAS solution surveys suppliers against **more than 7,000 PFAS** (Feb 2024) — [Supply Chain Dive press release](https://www.supplychaindive.com/press-release/20240207-assent-pfas-solution-now-surveys-against-more-than-7000-substances-enabli).
  - Scale claims: 4.5M supplier declarations and 695 unique PFAS (Sep 2025) — [press release](https://www.supplychaindive.com/press-release/20250915-assent-uncovers-over-695-unique-pfas-across-global-supply-chains-as-regulat).
  - Has published Minnesota reporting content — [Assent](https://www.assent.com/?p=104919).
  - **Pricing: custom quote only.** "Suppliers are never charged a fee to provide data" — [Assent pricing page](https://www.assent.com/?p=49947).
  - Target segment: complex manufacturers (industrial, electronics, machinery).
- **3E**
  - Added a **US PFAS Regulations library** to 3E Protect and 3E Exchange, with CAS-number filtering, update dates and jurisdiction alignment — [3E](https://www.3eco.com/article/streamlining-pfas-risk-management-embedded-u-s-pfas-regulations-library).
  - Tracks PFAS rules in 120+ countries, screens products against PFAS lists, and prepares regulatory reports — [3E PFAS coverage](https://www.3eco.com/3e-solutions/global-regulatory-coverage/pfas/).
  - Pricing not public.
- **UL Solutions (ULTRUS / WERCSmart)**
  - 2025 ULTRUS updates for PFAS tracking.
  - **WERCSmart identifies PFAS in retail products and collects documentation from manufacturers.** This is the retailer-facing data channel used by large US retailers.
  - Three-step workflow: portfolio screening, then automated supplier outreach for PFAS declarations, then targeted testing.
  - Sources: [UL](https://www.ul.com/services/proactive-pfas-management-products-across-your-supply-chain); [ESG Post](https://esgpost.com/ul-solutions-launches-new-tools-for-esg-pfas-and-wind-energy-planning/); [UL PFAS services](https://www.ul.com/services/pfas-identification-testing-and-management-services).
- **Enhesa**
  - "PFAS Tracker" for global PFAS rules within its product-compliance suite.
  - Acquired **TotalSDS** in Oct 2025.
  - Pricing per G2 (not retrieved in detail) — [G2](https://www.g2.com/products/enhesa/pricing); [Sagemount](https://www.sagemount.com/news/enhesa-expands-chemical-compliance-offering-with-acquisition-of-totalsds/).
- **Sphera:** Product Stewardship software plus **BOMcheck** supplier declarations (10M+ parts), with PFAS webinars — [Sphera](https://sphera.com/resources/events/navigating-pfas-regulations-ensuring-supply-chain-compliance).
- **Certivo** (AI-native challenger)
  - Says it covers multi-state PFAS reporting from **"a single PFAS dataset at product and component level, mapped to each state."**
  - Claims supplier declaration campaigns, PLM/ERP integration, coverage of 10,000–12,000+ PFAS, and "99.2% extraction accuracy." All are vendor claims and internally inconsistent.
  - It is the **closest in spirit to "reuse data across states,"** but no evidence was found of a cross-brand certificate network or a checkout integration.
  - Sources: [Certivo multi-state](https://www.certivo.com/blog-details/multi-state-pfas-reporting-reusing-data-across-minnesota-maine-and-more); [Certivo PFAS](https://www.certivo.com/pfas); [Certivo 12,000 substances](https://www.certivo.com/blog-details/how-certivo-manages-pfas-compliance-across-12-000-substances-and-multi-tier-supply-chains).
- **Inspectorio** (supply-chain quality platform) published a PFAS data-points guide for brands in 2025 — [Inspectorio](https://inspectorio.com/guide/pfas-in-focus-three-data-points-every-brand-must-track-in-2025).
- **Free and legal trackers** (substitutes for the rules-content layer):
  - Ballard Spahr PFAS Legislation Tracker (2024) — [Ballard Spahr](https://www.ballardspahr.com/insights/news/2024/06/new-pfas-tool-tracks-shifting-laws-and-regulations-around-forever-chemicals);
  - PFAS Project Lab Governance Tracker (federal and 50 states) — [PFAS Project](https://governance.pfasproject.com/static/aboutTool.html);
  - Safer States bill tracker — [Safer States](https://www.saferstates.org/resource/2026-analysis-of-state-policy-addressing-toxic-chemicals-and-plastics/laws-going-into-effect-in-2026/).

**Testing, inspection and certification (TIC) "PFAS-free" marks**
- **Intertek PFAS-Free Certification** (launched **May 2025**)
  - Based on TOF, with a **pass level below 20 ppm** (stricter than the 50/100 ppm regulatory thresholds).
  - Uses a formulation-data audit for metals, glass and stone.
  - Intertek markets against schemes that "rely solely on manufacturer affidavits."
  - Sources: [Intertek news](https://w3prep.intertek.com/news/2025/intertek-launches-pfas-free-certification-program); [Intertek PFAS-free](https://w3prep.intertek.com/sustainability/certification/pfas-free).
- **SGS Green Mark "No PFAS Detected"** (formerly "PFAS Screened")
  - Non-detection against a **selected list** of PFAS; **does not cover fluoropolymers**.
  - Has a "PFAS-assessed" route based on risk assessment of previous test data.
  - Sources: [SGS Green Mark](https://www.sgs.com/en/services/sgs-green-mark); [SGS TICmall](https://ticmall.sgs.com/en/blog_details/hl-technical-article-go-beyond-compliance-unlock-the-no-pfas-detected-advantage).
- **UL 746G** supports non-fluorine / non-PFAS ratings (from a Korean-language UL page, via search extract) — [UL](https://www.ul.com/services/pfas-identification-testing-and-management-services).

**Industry data-sharing networks (possible partners, or competitors if they add PFAS)**
- **ZDHC Gateway** (textile chemicals)
  - A shared repository for brands, formulators, suppliers and certifiers. **Suppliers control sharing per connection.**
  - The relaunched **Data Hub (Aug 2026)** includes only InCheck and ClearStream reports.
  - ZDHC planned a **PFAS communication for Oct 2026** alongside MRSL updates.
  - Sources: [ZDHC KB Data Hub](https://knowledge-base.roadmaptozero.com/hc/en-gb/articles/38314108808093-What-data-is-available-in-the-Data-Hub-at-launch-August-2026-Brands-Vendors); [ZDHC KB sharing](https://knowledge-base.roadmaptozero.com/hc/en-gb/articles/37973711903517-How-do-I-control-what-data-I-share-with-connected-organisations-Suppliers); [Just Style](https://www.just-style.com/news/zdhc-pfas-textile-manufacturing/).
- **Novi Connect** (beauty)
  - Supplier ingredient and packaging data checked against regulations and retailer standards (Target, Sephora).
  - Raised **$10.3M (Sep 2021)** and **$40M (Mar 2022)**. No PFAS-specific feature was found.
  - Sources: [CosmeticsDesign](https://www.cosmeticsdesign.com/Article/2022/03/09/novi-connect-gets-40-million-in-funding-to-expand-service); [Cosmetics & Toiletries](https://www.cosmeticsandtoiletries.com/home/news/21863257/novi-debuts-beauty-platform-for-ingredients-packaging).

**E-commerce geo-restriction tools (the checkout-blocking layer)**
- **Compliant Commerce AI** (Shopify): blocks specific products from being sold or shipped to restricted US states or ZIP codes, at storefront and checkout, while keeping products visible for SEO. **From $49.99 a month** — [Shopify App Store](https://apps.shopify.com/compliant-commerce).
- **ZIP Lock** (Shopify): state/ZIP rules by product or collection that block checkout. **From $9.99 a month; Shopify Plus only**; 2 ratings — [Shopify App Store](https://apps.shopify.com/zip-lock).
- **Ship Restrict** (Shopify): rules by product, variant or collection that block or allow states, cities or ZIPs. **$19.99 a month**; no reviews — [Shopify App Store](https://apps.shopify.com/ship-restrict).
- All three **enforce merchant-entered rules only**. None advertises PFAS legal content (from listing summaries).

**Startup and funding scan**
- No 2025–26 funding round for a **PFAS compliance-software** startup was found. PFAS venture money is going to destruction and testing technology, e.g. Claros ($55M Series B), Oxyle ($16M), Biota ($3M seed) — [VCA Online](https://www.vcaonline.com/news/archive/2026/); [Oxyle](https://oxyle.com/oxyle-raises-16m-to-lead-the-fight-against-the-forever-chemicals-contaminating-our-water).

### Inferences
- **White space:** no vendor was found doing **cross-brand reuse of lab-backed component PFAS certificates** combined with **legal-rule content pushed into checkout**.
  - Incumbents (Assent, 3E, UL, Enhesa, Sphera) sell to compliance teams at large manufacturers and retailers on custom enterprise pricing.
  - The Shopify apps are cheap but contain no rules content.
  - A "Compliant Commerce for PFAS" product, with rules maintained by the vendor and attestation-backed SKU flags, sits between them.
- **Main competitive threats:**
  - **UL WERCSmart** already sits between retailers and manufacturers collecting PFAS documentation, a natural network position.
  - **Intertek, SGS, BV, TÜV** could add certificate-sharing portals.
  - **ZDHC Gateway** already has supplier-controlled cross-brand sharing in textiles.
  - **Certivo and Assent** could add a checkout API.
  - Shopify apps could license a rules feed.
- **Partner path:** TIC labs (certificates as inputs), ZDHC and Novi (supplier data), and Shopify apps (checkout distribution) could be channel partners rather than competitors.

### Gaps
- Not researched because the search budget ran out:
  - Source Intelligence, Compliance & Risks (C2P), Toxnot, Chemical Watch/Enhesa news, GreenScreen Certified, Green Circle, OEKO-TEX and bluesign PFAS criteria, Higg/Cascale, Worldly, ChemFORWARD, Siemens Teamcenter compliance, Datamyne, Bureau Veritas and TÜV PFAS-free marks;
  - Avalara, Vertex, ShipStation and ShipperHQ product-restriction features;
  - IPC-1752 / IMDS-style declaration tools beyond BOMcheck.
- From memory, **unverified this session** — treat as leads only:
  - OEKO-TEX banned PFAS use in certified textiles from 2023;
  - bluesign has a PFAS restriction;
  - 3E was sold by Verisk to Warburg Pincus in 2022, so "3E (Verisk)" is likely outdated;
  - ShipperHQ supports product-group / destination shipping rules.
- **No pricing** found for Assent, 3E, UL, Enhesa, Sphera, Certivo, Intertek or SGS certifications.

---

## Q5. Is the business feasible: willingness to pay, legal acceptability of test-once-reuse, cold start, and risks?

### Takeaway
Feasibility is **mixed but plausible**. The case for it:
- the laws are multiplying and keep changing;
- penalties exist: WA up to $5k/$10k per violation, NY $1k per day;
- class-action exposure is real ($2.5M–$5M settlements);
- marketplaces (Walmart) already gate products by state and require manufacturer certificates;
- statutes in CA, NY and RI are built around **certificates of compliance**, and Minnesota explicitly allows **supplier and group reporting**.

These features support an attestation-sharing layer. The case against:
- obligations attach to the **finished product's manufacturer**, and TOF thresholds apply to the article, so a component test is evidence, not automatic compliance;
- definitions vary between states;
- enforcement is still light and states keep delaying rules;
- incumbents with large supplier networks, and generic checkout-blocking apps at $10–50 a month, cap pricing on the checkout piece.

### Cited Findings
**Evidence of willingness to pay (cost of noncompliance)**
- WA: up to **$5,000 per violation** for a first offense and **$10,000 per repeat** — [Exponent](https://www.exponent.com/article/washington-state-adopts-new-pfas-restrictions-and-reporting).
- NY apparel: up to **$1,000 per day** of violation and **$2,500** for a second violation — [Venable](https://www.venable.com/insights/publications/2024/10/fashion-industry-beware-pfas-bans-on-apparel).
- CA AB 347: DTSC gets authority from **Jul 1, 2030** to test products, issue violation notices, impose administrative penalties and seek injunctions — [BV](https://cps.bureauveritas.com/newsroom/california-adds-enforcement-body-and-registration-certain-pfas-laws).
- Settlements: Thinx about $5M; HexClad $2.5M; Gotham Steel/Bell & Howell 2026 — [ConsumerNotice](https://www.consumernotice.org/news/pfas-thinx-lawsuit/); [ClassAction.org](https://www.classaction.org/news/2.5m-hexclad-settlement-reached-in-false-advertising-lawsuit-over-supposedly-non-toxic-cookware); [Top Class Actions](https://topclassactions.com/lawsuit-settlements/open-lawsuit-settlements/bell-howell-pfas-cookware-class-action-settlement/).
- Texas AG investigation of Lululemon (Apr 2026), even though Texas has no PFAS ban — [Foley](https://www.foley.com/p/102mq7l/texas-attorney-general-investigates-lululemon-over-alleged-forever-chemicals-in/).
- Direct regulatory fees and burden: MN **$800 one-time fee** plus annual updates — [RVIA](https://www.rvia.org/news-insights/minnesota-adopts-final-rules-pfas-reporting-and-fees); CA AB 347 registration fee (not yet set) — [BCLP](https://www.bclplaw.com/en-US/events-insights-news/pfas-update-california-enacts-new-pfas-enforcement-and-registration-law.html).
- Law-firm advice is to "negotiate supplier certifications, manage inventory, and decide whether to reformulate, discontinue, or redesign covered products for the Connecticut market" — [B&D Connecticut](https://www.bdlaw.com/publications/connecticut-pfas-consumer-product-reporting-and-labeling-requirements-are-now-in-effect/).

**Is test-once-reuse-many legally acceptable?**
- **Supports reuse:**
  - CA AB 1817: manufacturers give certificates to sellers, which may be electronic, and **sellers relying in good faith are protected** — [Bureau Veritas](https://www.cps.bureauveritas.com/newsroom/california-signs-pfas-textile-articles-bill-ab-1817).
  - NY: sellers may rely in good faith on a manufacturer's certificate of compliance — [Venable](https://www.venable.com/insights/publications/2024/10/fashion-industry-beware-pfas-bans-on-apparel).
  - RI: on request, a manufacturer **certificate attesting** no intentionally added PFAS satisfies the 30-day demand — [TÜV SÜD](https://www.tuvsud.com/en-gb/e-ssentials-newsletter/consumer-products-and-retail-essentials/e-ssentials-5-2024/usa-rhode-island-enacted-law-on-pfas-ban).
  - MN: **suppliers may report on a manufacturer's behalf under agreement**; groups of manufacturers and authorized representatives may report together; similar products can be grouped and concentration ranges used — [MPCA via B&D](https://www.bdlaw.com/publications/minnesota-extends-pfas-in-products-reporting-deadline-to-september-15-2026/); [Pillsbury](https://www.pillsburylaw.com/en/news-and-insights/minnesota-extends-initial-pfas-deadline-september-15-2026.html).
  - MN: reports may rest on the **best available information**, with continued supplier outreach documented — [Greenberg Traurig](https://www.gtlaw.com/es/insights/2026/6/schools-out-for-summer-but-minnesotas-amaras-law).
  - Walmart Marketplace accepts "free of intentionally added PFAS" claims backed by a **manufacturer certificate** — [Walmart](https://marketplacelearn.walmart.com/guides/prohibited-products-policy-pfas-chemicals).
- **Limits reuse:**
  - Obligations sit with the "manufacturer," which in NM includes importers and first domestic distributors, and the duty is to determine intentional addition — [SGS NM](https://www.sgs.com/news/2026/05/safeguards-07526-new-mexico-issues-rules-for-pfas-in-consumer-products).
  - TOF thresholds (CA, VT) and the WA 50 ppm presumption apply to the **product or article**.
  - DTSC will set **accepted test methods and lab accreditations** by Jan 1, 2029 — [BCLP](https://www.bclplaw.com/en-US/events-insights-news/pfas-update-california-enacts-new-pfas-enforcement-and-registration-law.html). A shared certificate may need to match state-specified methods and labs.
  - Intertek markets against affidavit-only schemes — [Intertek](https://w3prep.intertek.com/news/2025/intertek-launches-pfas-free-certification-program).
  - TOF methods are not standardized, so lab method matters for comparability — [HQTS](https://www.hqts.com/?p=183995).
- **Public data seed:** MN PRISM reports are public after review, except trade secrets, and anyone can read them without an account — [RV PRO / MPCA](https://rv-pro.com/news/minnesota-pollution-control-agency-reaffirms-pfas-reporting-deadline/).
- **No interoperability across states:** "no shared technical standard linking state reporting systems." The data each state asks for is largely the same, which makes reuse possible — [Certivo, vendor](https://www.certivo.com/blog-details/multi-state-pfas-reporting-reusing-data-across-minnesota-maine-and-more).

**Risks**
- **Definitional differences:**
  - "intentionally added" (most states) versus TOF thresholds (CA and VT, 100 then 50 ppm) versus WA's 50 ppm presumption versus NY's numeric limit due 2027;
  - CT's trace exemption for cosmetics;
  - SGS's mark uses a targeted list and excludes fluoropolymers, while Intertek's uses TOF below 20 ppm;
  - Sources: [Q1 matrix]; [SGS](https://www.sgs.com/en/services/sgs-green-mark); [Intertek](https://w3prep.intertek.com/sustainability/certification/pfas-free).
- **State delays and rollbacks:** ME 2024, MN three deadline moves, VT H.238, IL to 2032, CA SB 682 veto — see the Q1 rollback list.
- **Federal preemption:**
  - No federal preemption bill was found. The main federal bill (S. 4153 / H.R. 8016) would be **more** restrictive, and nothing shows it moving — [Arnold & Porter](https://www.arnoldporter.com/en/perspectives/blogs/environmental-edge/2026/03/congress-considers-broad-pfas-legislation).
  - EPA is easing PFAS obligations: TSCA 8(a)(7) delays, a proposed exemption for imported articles, and drinking-water rollbacks — [BV](https://www.cps.bureauveritas.com/newsroom/us-federal-pfas-updates-postponement-and-proposal); [Federal Register](https://www.federalregister.gov/documents/2026/05/20/2026-10086/extending-the-compliance-deadline-for-the-pfoa-and-pfos-maximum-contaminant-levels).
  - Courts have **upheld** a state ban against a dormant Commerce Clause challenge (MN cookware, Aug 2025) — [Packaging Law](https://www.packaginglaw.com/news/court-dismisses-cookware-alliances-lawsuit-challenging-mn-ban-cookware-containing-added-pfas).
- **Litigation and evidence risk:** TOF alone was found insufficient to prove PFAS presence — [Mintz](https://mgmlaw.com/news-insights/total-organic-fluorine-found-insufficient-to-demonstrate-pfas). A positive result needs a targeted LC-MS/MS follow-up at $400–700 — [HQTS](https://www.hqts.com/?p=183995).
- **Incumbent network effects:** Assent (4.5M declarations; free for suppliers), BOMcheck (10M+ parts), UL WERCSmart (retailer channel) and ZDHC Gateway (textile supplier sharing) already have supplier networks — sources in Q4.

### Inferences
- **Willingness to pay is strongest for:**
  1. mid-market DTC brands in apparel, outdoor, cookware, beauty and kids' products that sell nationally online and cannot afford Assent or 3E;
  2. marketplaces and retailers that must collect certificates from thousands of sellers, following Walmart's model.
  
  Pricing anchors:
  - the low end is Shopify geo-blocking apps at **$10–$50 a month**;
  - a single TOF test is about **$300–400**, and a targeted test **$400–700**;
  - the high end is enterprise compliance suites on custom quotes (amounts not public).
  
  A plausible structure: SaaS tiers per SKU count for the rules engine and checkout block, plus **per-certificate listing or access fees** paid by suppliers or labs, or a revenue share with labs. This is an inference; no direct WTP survey was found.
- **The cold start is the main business risk.** Mitigations suggested by the evidence:
  - **seed the network with public MN PRISM data**, as negative signal for PFAS-containing products, plus state rules content;
  - **partner with TIC labs** (Intertek, SGS) so certificates flow in automatically;
  - **target concentrated component suppliers** (textile mills, DWR-free finish makers, cookware coating suppliers), where one certificate covers many brands;
  - **sell the rules engine and checkout block first** as a standalone tool that works with zero network data, then upsell attestations.
- **Legal design point:** position certificates as **evidence supporting the manufacturer's own certificate of compliance or report** (CA, NY, RI, MN), not as a replacement for it. Link each certificate to a material spec, lot or date range, test method, lab accreditation and threshold, so the rules engine can check "does this evidence meet state X's definition on date Y?"
- **Regulatory volatility helps a rules-content business** (constant updates justify a subscription) **but hurts urgency.** Delays such as MN's three moves, IL to 2032 and the SB 682 veto let buyers defer purchases. The firmest near-term deadlines in this research:
  - CA 50 ppm TOF: Jan 1, 2027
  - WA restrictions: Jan 1, 2027
  - WA first reports: Jan 31, 2027
  - NM bans: Jan 1, 2027 and Jan 1, 2028
  - VT 50 ppm TOF: Jul 1, 2027
  - RI bans: Jan 1, 2027
  - CT ban: Jan 1, 2028
  - NJ ban: Jan 12, 2028
  - NY outdoor apparel: Jan 1, 2028
  - CO textiles: Jan 1, 2028
  - CA DTSC registration: Jul 1, 2029
  - ME, MN and NM near-universal bans: 2032

### Gaps
- No direct evidence (surveys, interviews, public statements) of brands' willingness to pay for PFAS compliance software, and no published price points for enterprise competitors.
- No regulator guidance found that explicitly accepts or rejects **component-level third-party test reports shared across brands** as the basis for a finished-product certificate. Regulators' positions on this need direct confirmation (DTSC rulemaking by 2029; MPCA guidance on supplier reporting).
- No data on how often retailers delist products, or what recalls cost, over PFAS state bans.
- Shopify, BigCommerce and Amazon policies on state-based shipping restrictions for PFAS were not retrieved, beyond Walmart's.
