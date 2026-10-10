# Validation of K02 (CARS Act 3-Day Log, California used-car dealers) and K03 (IFTA Close, small fleets and owner-operators)

Method note: research date **2026-10-10**. I ran 35 web searches (the full budget). Direct page fetches failed: dmv.ca.gov and cbtnews.com returned DNS errors through WebFetch, and leginfo.legislature.ca.gov, data.transportation.gov, ai.fmcsa.dot.gov and iftach.org returned proxy 403s through curl. GitHub search was also refused (the session is scoped to its own repository). **Every finding below therefore comes from search-engine summaries of the linked pages, not from reading the pages.** Treat exact figures, especially statutory numbers, as "reported by the linked source, not confirmed against primary text." "[Corpus]" marks claims carried over from the corpus files (written Sep 24 2026 and never fact-checked).

---

## Key question 1: Trigger check. Is the CARS Act (SB 766) in force as described, and what are the IFTA deadlines, record rules and 2026 changes?

### Takeaway
**K02:** The trigger is real and live. SB 766 was chaptered Oct 6 2025 and took effect **Thu Oct 1 2026**. A DMV industry memo from Sep 2026 confirms the date, and I found no delay, cleanup amendment or litigation. The corpus's 3-day-return numbers ($50k cap, 400 miles, 1.5% restocking fee bounded at $200–$600, 48-hour refund) match several secondary sources. Those sources add a **mileage charge of $1 per mile over 250 miles, capped at $150**, plus trade-in return rules. The corpus's retention claim needs correcting: the Act's own retention period is **2 years** for ads, price communications, add-on consents and cancellation documents. **K03:** The IFTA schedule is unchanged and I found no 2026 rule change. The next realistic launch deadline is effectively **Mon Feb 1 2027**, because Jan 31 2027 is a Sunday. Records must be kept 4 years.

### Cited Findings
**K02: status and dates**
- SB 766 was chaptered by the Secretary of State on **2025-10-06** as Chapter 354, Statutes of 2025 — [CalMatters Digital Democracy](https://calmatters.digitaldemocracy.org/bills/ca_202520260sb766); [PolicyRisk tracker](https://policyrisk.com/state-bill/CA-SB766-20252026)
- Gov. Newsom signed it Oct 6 2025, and it became operative Oct 1 2026 — [CarPro, "coming soon"](https://www.carpro.com/blog/california-cars-act-coming-soon-will-other-states-follow). A CarPro post dated early Oct 2026 says the Act "became operative Oct. 1" — [CarPro, "The new CARS Act has started"](https://www.carpro.com/blog/the-new-cars-act-has-started)
- A California DMV industry memo (file "26olin10", September 2026 per search summaries) confirms the Oct 1 2026 start — [DMV memo 26olin10](https://www.dmv.ca.gov/portal/file/26olin10-pdf/). The DMV also has a consumer page on the CARS Act — [DMV CARS Act page](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/)
- Dealership Guy says the rules "kick in Thursday, Oct. 1" — [Dealership Guy](https://news.dealershipguy.com/p/on-top-of-ftc-rules-california-dealers-rush-to-comply-with-cars-act)
- **Delays, amendments, litigation:** a targeted search found no 2026 delay, cleanup bill or lawsuit — [search over NCLC, Sen. Allen's office, ComplyAuto and others](https://sd24.senate.ca.gov/news/press-release/senator-allen-delivers-needed-transparency-and-consumer-protections-car-shoppers). That is absence of evidence, not confirmation.
- Some pages (SecureClose; an older NIADA post) still say the bill is "heading to the Governor". They are stale — [SecureClose](https://secureclose.net/tag/sb766/); [NIADA](https://niada.com/blog/california-passes-cars-act/)

**K02: coverage**
- The Act covers licensed California dealers selling or leasing light-duty vehicles (under 10,000 lb), new and used. Exempt: wholesale, fleet sales (5+ units), auction sales, and commercial buyers purchasing 5+ vehicles a year — [DMV CARS Act page](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/); [ComplyAuto summary](https://complyauto.com/california-enacts-the-cars-act-overhauling-vehicle-sales-and-leasing-rules/)
- Motorcycles and vehicles over 10,000 lb are excluded — [PolicyRisk](https://policyrisk.com/state-bill/CA-SB766-20252026)

**K02: the 3-day cancellation right (the wedge)**
- **Scope:** the right is automatic on used vehicles priced **$50,000 or less**. It does not cover new vehicles, lease buy-outs, auctions, fleet sales or used vehicles over $50k — [SecureClose summary](https://secureclose.net/tag/sb766/); [ComplyAuto](https://complyauto.com/california-enacts-the-cars-act-overhauling-vehicle-sales-and-leasing-rules/)
- An Assembly committee analysis used a **$48,000** threshold. That was an earlier version; the enacted figure reported elsewhere is $50,000 — [Assembly analysis](https://apcp.assembly.ca.gov/media/1007)
- **What it replaces:** the old optional, paid 2-day contract cancellation option (Car Buyer's Bill of Rights, used cars under $40,000) — [DMV memo 26olin10](https://www.dmv.ca.gov/portal/file/26olin10-pdf/); [CarPro](https://www.carpro.com/blog/the-new-cars-act-has-started)
- **Clock:** the window starts the calendar day after signing and runs 3 calendar days. The buyer must return the car in person during business hours — [SlashGear](https://www.slashgear.com/2004828/california-2026-new-car-buying-law/); [CarPro](https://www.carpro.com/blog/the-new-cars-act-has-started)
- **Mileage and condition:** the right ends once the car has been driven more than **400 miles**. The car must come back in the same condition, with no new damage beyond normal wear — [DMV CARS Act page](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/); [Jalopnik](https://jalopnik.com/2005998/california-cars-act-protects-used-car-buyers)
- **Fees:** a restocking fee of **1.5% of the sale price, minimum $200, maximum $600**, plus **$1 per mile over 250 miles, capped at $150** — [CBT News](https://www.cbtnews.com/?p=252530); [SlashGear](https://www.slashgear.com/2004828/california-2026-new-car-buying-law/)
  - **Not confirmed against the statute.** The codified section (reported as Civil Code §1784.43) surfaced only subdivisions (h)–(j) — [FindLaw §1784.43](https://codes.findlaw.com/ca/civil-code/civ-sect-1784-43/)
  - One law-firm summary words the fee as "not to exceed 1.5%... maximum $600" without the $200 floor — [Ginsburg Law Group](https://ginsburglawgroup.com/?p=17652)
- **Refund timing:** 48 hours per [CBT News](https://www.cbtnews.com/?p=252530). One tracker gives "48 hours, or two business days after your payment is verified" — [PolicyRisk](https://policyrisk.com/state-bill/CA-SB766-20252026). These differ; check the statute.
- **Trade-ins:** the dealer must return the trade-in, or pay the highest of the agreed value, the dealer's resale price or fair market value, minus any payoff — [PolicyRisk](https://policyrisk.com/state-bill/CA-SB766-20252026)
  - Because reselling a trade-in during the window can raise what the dealer owes, ComplyAuto suggests some dealers will hold trade-ins for the full 3 days — [ComplyAuto](https://complyauto.com/california-enacts-the-cars-act-overhauling-vehicle-sales-and-leasing-rules/)
- **Required disclosures:**
  - a 36-point in-store notice, a notice on the first page of the contract, and a separate "3-Day Right to Cancel" form — [PolicyRisk](https://policyrisk.com/state-bill/CA-SB766-20252026)
  - updated "No Cooling Off" signage — [Ginsburg Law Group](https://ginsburglawgroup.com/?p=17652); [LexBlog](https://www.lexblog.com/?p=3343833)
  - Disclosures may be satisfied by adding them to the existing California Pre-Contract Disclosure form — [Ginsburg Law Group](https://ginsburglawgroup.com/?p=17652)

**K02: other duties**
- **Total price:** dealers must show it in advertising and in the first written communication about a vehicle or its financing (email, text, document, form). It must include mandatory fees and dealer charges, with government taxes and fees shown separately — [DMV CARS Act page](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/); [CNCDA/ComplyAuto event page](https://www.cncda.org/events/carsact_complyauto/)
- **"Valueless" add-ons are banned** — [NIADA](https://niada.com/blog/california-passes-cars-act/)
- **Record retention:** dealers must keep **2 years** of records showing compliance: ads, pricing communications, add-on disclosures and consents, and cancellation documents — [DMV memo 26olin10](https://www.dmv.ca.gov/portal/file/26olin10-pdf/); [ComplyAuto](https://complyauto.com/california-enacts-the-cars-act-overhauling-vehicle-sales-and-leasing-rules/)
  - The corpus's "7+ years finance rules" figure was not checked in this pass — [Corpus K02]
- **Enforcement:** the Act sets no fixed per-violation fines. It is enforced through the Unfair Competition Law, False Advertising Law and Consumer Legal Remedies Act, with the DMV and BAR named as agencies. Possible penalties include license suspension or revocation and administrative fines — [DMV CARS Act page](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/) (search summary; also [CA Lawyers Association](https://calawyers.org/business-law/california-combating-auto-retail-scams-cars-act-signed-into-law/))
- **Federal backdrop:** a search summary says the FTC sent warning letters to "over 90" dealers in 2026 about pricing transparency. I could not pin the figure to a specific source; the likely one is [AutoSuccess](https://www.autosuccessonline.com/ftc-warning-letters-dealership-pricing-transparency/). Unverified.

**K03: IFTA dates and rules**
- **Quarters and due dates:** Q1 (Jan–Mar) is due Apr 30, Q2 Jul 31, Q3 Oct 31 and Q4 Jan 31. If a due date falls on a weekend or legal holiday, the next business day is the due date — [Colorado DOR](https://tax.colorado.gov/IFTA-filing-information)
- Georgia lists the **Q3 2026 due date as 11/02/2026** and **Q4 2026 as 2/01/2027** — [Georgia DOR](https://dor.georgia.gov/ifta-due-dates). Utah's calendar also shows Feb 1 2027 — [Utah Tax Commission](https://tax.utah.gov/?p=5348)
  - My calendar check: Oct 31 2026 is a Saturday, Jan 31 2027 a Sunday, Apr 30 2027 a Friday and Jul 31 2027 a Saturday.
- One guide warns that weekend rules vary by base jurisdiction — [O Trucking](https://otrucking.com/resources/guides/ifta-quarterly-due-dates/)
- **No 2026 rule change found.** The only item found: Colorado will keep paper forms through the 2027 tax returns for filers who still qualify — [Colorado DOR](https://tax.colorado.gov/IFTA-filing-information)
- **Jurisdictions:** IFTA has 58 member jurisdictions (48 US states and 10 Canadian provinces). New Jersey alone has about 12,000 IFTA accounts covering about 63,000 vehicles — [NJ MVC](https://www.nj.gov/mvc/business/ifta.htm)
- **Records:** keep them 4 years from the return's due date or filing date, whichever is later. The period extends if records are not produced at audit — [Minnesota DPS](https://dps.mn.gov/divisions/dvs/business/irp-and-ifta/irp-and-ifta-audit/irp-and-ifta-audit-record-keeping-requirements); [Kentucky Audit Assistance Manual 2026](https://transportation.ky.gov/Audits/Documents/Audit%20Assistance%20Manual%202026.pdf)
- **Tracking-system data:** since Jan 1 2024, vehicle-tracking records must be captured at least every 10 minutes while the engine is on, with date, time, location and odometer — [Minnesota DPS](https://dps.mn.gov/divisions/dvs/business/irp-and-ifta/irp-and-ifta-audit/irp-and-ifta-audit-record-keeping-requirements)
- **Summaries alone don't count.** Auditors want source documents such as individual vehicle mileage records (IVMRs) — [J.J. Keller on IVMRs](https://jjkellercompliancenetwork.com/regsense/individual-vehicle-mileage-report-ivmr); [Kentucky manual](https://transportation.ky.gov/Audits/Documents/Audit%20Assistance%20Manual%202026.pdf)
- **IRP retention is longer** (Minnesota: 5½ years) — [Minnesota DPS](https://dps.mn.gov/divisions/dvs/business/irp-and-ifta/irp-and-ifta-audit/irp-and-ifta-audit-record-keeping-requirements)
- **Audit rate:** jurisdictions must randomly audit about 3% of licensees a year — [Keller Encompass](https://eld.kellerencompass.com/resource/blog/what-is-ifta) (secondary)
- **Late penalty:** $50 or 10% of net tax, whichever is greater, plus 1% a month interest — [Beancount guide, Jul 10 2026](https://beancount.io/blog/2026/07/10/ifta-fuel-tax-quarterly-filing-owner-operator-guide) (secondary)

### Inferences
- **K02:** the trigger is now a **"first 90 days of live compliance"** sale, not a pre-deadline sale. Every used retail deal at nearly every California independent lot is in scope, because almost all independent inventory is under $50k.
- **K02:** the most operationally risky pieces are the time-bound ones: the 3-day window, the 48-hour refund and the trade-in hold. Paper forms do these badly, and they are the ones a small tool can own.
- **K02:** the 2-year retention period is shorter than the corpus implied. "7-year storage" is not a selling point; sell "2-year CARS Act binder" and keep everything by default.
- **K03:** the next real selling deadline is **Feb 1 2027** (Q4 2026), then Apr 30 2027. Q3 2026 (due Nov 2 2026) is too close for a new build.

### Gaps
- I could not read the SB 766 chaptered text. The restocking-fee floor ($200), the mileage charge ($1/mile over 250, cap $150) and refund timing (48 hours versus two business days after payment verification) must be confirmed on leginfo before any calculator ships.
- I found no California Attorney General guidance and no report of enforcement or returns since Oct 1.
- I found no IFTA, Inc. ballot or 2026 agreement amendment. The IFTA, Inc. site was unreachable.

---

## Key question 2: Competitor sweep. Who already sells this, at what price, and what did the corpus miss?

### Takeaway
**K02:** No independent-dealer DMS (DealerCenter, Frazer, Wayne Reaves, ProMax) has a public CARS Act workflow announcement that surfaced in search as of Oct 10 2026. The compliance field is aimed at franchise dealers and quote-priced: ComplyAuto, KPA, Tekion, Reynolds forms through CNCDA. The adjacent point tools are SecureClose (e-sign and e-vault) and SnapInspect (condition inspection), both marketing SB 766. The gap the corpus assumed still looks open at the independent end, but it is unconfirmed; vendor release notes are not public. **K03:** The space is crowded and cheap, and the corpus under-counted it. Prices run from **$9/mo** (FleetCollect, launched Feb 2026, receipt photos) through $19.95/mo or **$19.95–$24.95 per report** (ExpressIFTA, Geotab, TruckLogics) to free (calculators; AscendTMS through DAT and factoring partners). A new AI receipt-scanning IFTA app (SureMile, Apr 2026) also exists. Motive and Samsara already produce jurisdiction-mileage IFTA reports with fuel CSV import; they just don't file the return.

### Cited Findings
**K02: compliance vendors and association kits**
- **ComplyAuto** runs a CARS Act resource center and co-hosted the CNCDA webinar "Countdown to the CARS Act". The webinar cost **$99 for CNCDA members**, registration closed Aug 24 2026, and it walked through ComplyAuto's **Guardian** AI tool — [CNCDA event](https://www.cncda.org/events/carsact_complyauto/)
  - Guardian is an AI/ML engine for sales, F&I and advertising compliance — [AutoSuccess](https://www.autosuccessonline.com/?p=21067)
  - **No public price found.** ComplyAuto has separate pricing pages for single rooftops and groups, but the figures did not surface — [search, Oct 10 2026](https://www.autosuccessonline.com/?p=21067)
- **CNCDA and Reynolds & Reynolds** built new and updated CARS Act forms, with a recorded webinar "Complying with the CARS Act: New Forms and Dealer Obligations" — [CNCDA](https://www.cncda.org/events/carsact_newformswebinar/)
  - CNCDA also has a "Compliance Guidance for Dealers" event (recorded Mar 10 2026) — [CNCDA](https://www.cncda.org/events/california-cars-act)
  - CNCDA's guidance includes checklists, FAQs and an **80-page compliance guide** — [Dealership Guy](https://news.dealershipguy.com/p/on-top-of-ftc-rules-california-dealers-rush-to-comply-with-cars-act)
  - CNCDA is the **franchise** (new-car) association.
- **KPA** runs a CA CARS webinar series, including "Episode 2: 3-day cancellation, payment transparency, deal disclosures" — [KPA webinar](https://kpa.io/webinar/ca-cars-episode-2-3-day-cancellation-payment-transparency-deal-disclosures/). It offers a free compliance checklist — [KPA](https://info.kpa.io/cdg2) — and a blog post titled "The $3 million warning: state-level enforcement replaces FTC's CARS Rule" — [KPA blog](https://hs.kpa.io/blog/the-3-million-warning-state-level-enforcement-replaces-ftcs-cars-rule). No price found.
- **Tekion** (franchise DMS) says its platform is being updated for CARS Act requirements, and that dealers remain responsible for their own compliance — [Tekion](https://tekion.com/blog/preparing-for-cars-act-and-ftc-pricing-compliance-what-dealers-need-to-know)
- **Fullpath** (AI shopper agent) lets dealers configure a CARS Act rule set: explain the 3-day right only on request, and never approve a cancellation — [Fullpath help center](https://help.fullpath.com/hc/en-us/articles/53305019188500-Compliant-Agent-Onboarding-California-CARS-Act)
- **SecureClose** markets ID verification, e-signature and e-vault storage, with SB 766 and BHPH-tagged content — [SecureClose SB766 tag](https://secureclose.net/tag/sb766/); [SecureClose BHPH tag](https://secureclose.net/tag/bhph/). Price not found.
- **SnapInspect** (vehicle inspection software) markets condition documentation for the 3-day return: "how does a dealership show what condition it was actually in when it left?" — [SnapInspect blog](https://blog.snapinspect.com/california-sb-766/). A syndicated press release pushes the same angle — [KDH News press release](https://kdhnews.com/online_features/press_releases/californias-new-3-day-used-car-return-law-puts-vehicle-condition-documentation-in-the-spotlight/article_645ad4a1-01c5-567b-894a-6039e8f99064.html). Price not found.
- **Independent-dealer DMS and forms vendors:** targeted searches for DealerCenter, Frazer, ProMax, Wayne Reaves, RouteOne and Dealertrack plus "CARS Act" returned **no vendor announcements** — [search summaries, Oct 10 2026, results pointed only to general CARS Act pages such as the DMV memo](https://www.dmv.ca.gov/portal/file/26olin10-pdf/). Absence in search is weak evidence; these vendors publish release notes behind logins.
- **DMS prices (corpus, Sep 2026, not re-checked):** DealerCenter $99/mo; Frazer $129/mo desktop or $199/mo hosted — [Corpus K02, citing Frazer pricing](https://www.frazer.com/frazer-pricing)
- **CIADA caution:** the "CIADA" search results were for the **Carolinas** Independent Automobile Dealers Association (theciada.com), which has no CARS Act content — [theciada.com](https://theciada.com/). I could not confirm a California independent-dealer association running a CARS Act kit. NIADA covered the law's passage — [NIADA](https://niada.com/blog/california-passes-cars-act/)

**K03: ELDs**
- **Motive:** distance per IFTA jurisdiction, recorded daily from GPS and odometer. Fuel comes in from the Motive Card automatically, from driver-app receipt uploads, or from bulk CSV import from fuel vendors. Reports > IFTA Trip Reports exports by quarter. Motive's FAQ says it **"doesn't yet automate IFTA fuel tax filing"** — [Motive IFTA product page](https://gomotive.com/products/fleet-compliance/ifta-fuel-tax-reporting/); [Motive help: Trip Reports](https://helpcenter.gomotive.com/hc/en-us/articles/30897108333213-Trip-Reports); [Motive blog: fuel purchase reports](https://gomotive.com/blog/ifta-fuel-purchase-reports)
- **Samsara:** an IFTA Mileage report under Fuel & Energy, using ECU distance with GPS as fallback. It runs monthly or quarterly and is available on the 2nd day after the period ends. Fuel comes in by CSV import or WEX/Fleetcor card integration — [Samsara KB](https://kb.samsara.com/hc/articles/360046354291)
  - Third parties pull Samsara data: [TruckLogics import](https://support.trucklogics.com/art/14754/how-to-import-distance-and-fuel-data-from-samsara-for-ifta-reporting); [DataTruck Samsara IFTA export, by state and by truck](https://support.datatruck.io/hc/en-us/articles/50522581636243-How-to-Generate-a-Samsara-IFTA-Report)
- **Roadeazy** (ELD) shipped an "IFTA Report (Beta)" on Jan 4 2026 — [Roadeazy release notes](https://kb.roadeazy.com/hc/en-us/articles/45682353407131-Cloud-Release-Notes-January-4-2026)

**K03: back-office and IFTA tools**
- **TruckLogics:**
  - Owner-operator plan (1–2 trucks): $35.96/mo billed annually or $39.95/mo monthly. Small fleet (3–7 trucks): $71.96 or $79.95 — [Empwr review](https://www.empwrtrucking.com/freight-technology/trucklogics-tms-review-for-small-fleets-simplify-dispatch-and-compliance/)
  - IFTA-only reports at about $19.95–$24.95 per report — [rfp.wiki citing TruckLogics pricing](https://www.rfp.wiki/supply-chain-logistics-transportation/transportation-logistics/trucking-erp-software/trucklogics/truckbase). $24.95 per report per quarter — [TruckLogics blog](https://blog.trucklogics.com/start-generating-your-3rd-quarter-ifta-report-with-trucklogics-now-the-deadline-is-october-31st/)
  - NerdWallet (labeled 2024) lists TruckLogics from $10/mo — [NerdWallet](https://www.nerdwallet.com/best/small-business/trucking-accounting-software). These sources conflict and dates vary.
- **ExpressIFTA:** from $19.95/mo — [Guideflow](https://www.guideflow.com/blog/ifta-reporting-software). Also a free calculator app needing no account — [App Store](https://apps.apple.com/app/id977647302)
- **Geotab standalone IFTA:** $24.95 per report for business owners, $19.95 for service providers, 7-day free trial — [Guideflow](https://www.guideflow.com/blog/ifta-reporting-software)
- **LoadManager:** owner-operator tier $50/mo, IFTA automation $5 per truck — [G2](https://www.g2.com/products/loadmaster/pricing)
- **TruckingOffice** $20/mo (tiers $30–$110) and **Rigbooks** $19/mo, each with a 30-day trial — [NerdWallet (2024; may be stale)](https://www.nerdwallet.com/best/small-business/trucking-accounting-software)
- **AscendTMS:**
  - Free IFTA reporting with state-rate calculation and EFS/Fleet One fuel-card import. The 2016 release tied it to the premium tier — [DC Velocity](https://dcvelocity.com/articles/40909-ascendtms-provides-free-ifta-tax-reporting-to-subscribers-of-their-premium-tms-software)
  - Free to DAT carrier users, with IFTA and fuel-card import listed — [Overdrive](https://overdriveonline.com/business/article/14892605/ascendtms-software-free-to-dat-carrier-users)
  - Free to Love's factoring customers — [FreightWaves](https://freightwaves.com/news/loves-offers-ascendtms-free-to-its-factoring-customers)
  - Free version limited to 2 users — [SoftwareConnect](https://softwareconnect.com/transportation-management/ascendtms/). The corpus says 3 or fewer users, so the sources conflict.
- **New in 2026 (missed by the corpus):**
  - **FleetCollect** launched IFTA tracking software on Feb 16 2026: fuel-stop logging with receipt photo capture and location detection, **plans from $9/mo with no contract**, and an ELD planned — [24-7 Press Release](https://www.24-7pressrelease.com/press-release/531872/fleetcollect-launches-ifta-tracking-software-and-fleet-dqf-platform-to-automate-compliance-for-trucking-companies)
  - **SureMile** (iPhone, first released Apr 29 2026): miles by state, fuel capture, quarterly reports, and an AI document scanner for crumpled receipts — [mwm.ai listing](https://mwm.ai/apps/suremile/6759183086)
  - **Bubba.ai:** driver receipts via SMS or WhatsApp, with tax data extracted — [Bubba.ai](https://bubba.ai/solutions/fleet-compliance-software)
  - **Omnitracs Tax Manager:** AI-assisted multi-jurisdiction fuel-tax filing (enterprise) — [SDCExec](https://www.sdcexec.com/transportation/press-release/21117146/www.sdcexec.com/omnitracs)
- **Spreadsheets:** a $27 Excel/Google Sheets owner-operator tracker with IFTA quarters — [Payhip](https://payhip.com/b/zQl2s). A 48-state mileage and fuel tracker — [Payhip](https://payhip.com/b/92H4J). Etsy equivalents — [Etsy](https://www.etsy.com/listing/4533491676/)
- **Filing services:** Simplex Group advertises owner-operator IFTA filing without a public price — [Simplex](https://simplexgroup.net/ifta-filing-service/). A 2026 "cost guide" puts professional filing at $200–$350 a quarter, but the site looks unreliable — [risingsunartscentre.org](https://new.risingsunartscentre.org/news/ifta-quarterly-cost-guide-for-us-truckers-2026.html)
- **Forum anecdotes:** one owner-operator says the most he ever paid for a quarter was about $60. Another reports first quarters costing about $200 and $300, the second including a late penalty — [TruckersReport thread (date not confirmed, likely old)](https://www.thetruckersreport.com/truckingindustryforum/posts/2294530)

### Inferences
- **K02:** the competitive picture splits in two. Franchise-grade compliance suites (ComplyAuto, KPA, Reynolds forms, Tekion) are quote-priced and sold to franchise groups. Point tools (SecureClose, SnapInspect) each cover one slice: e-sign and storage, or photos.
  - Nothing I found combines a **3-day clock, mileage and fee calculator, 48-hour refund timer, trade-in hold alert, condition photos with buyer e-sign, and a 2-year binder**, priced by card for a 20-car independent lot. That gap is plausible but unconfirmed.
  - The real threat is forms vendors and DMSs adding a "3-day cancellation" form plus a checkbox. That covers the paperwork but probably not the clock, the photos or the refund workflow.
- **K03:** the corpus's "Gap" score of 2 was, if anything, generous.
  - The core calculation is a commodity: $0 calculators, $9–$20/mo apps, and $20–$25 per-report tools.
  - The ELDs already output the hardest input (jurisdiction miles).
  - AI receipt OCR, the corpus's intended differentiator, shipped in at least two 2026 products.
  - The remaining gaps are actual e-filing on each base state's portal, receipt-to-card reconciliation, and audit defense. All three are service-heavy.

### Gaps
- I have no live prices for ComplyAuto, KPA, SecureClose, SnapInspect, DealerCenter or Frazer (beyond the corpus's Sep 2026 figures), Wayne Reaves or ProMax.
- I could not see whether DealerCenter or Frazer added CARS Act forms or workflows; release notes are behind logins. **This is the single most important unknown for K02.** Ask 5 dealers on discovery calls.
- I have no current ExpressIFTA pricing page, no confirmed AscendTMS free-tier IFTA scope, and no current Rigbooks or TruckingOffice pricing.
- Factoring-company bundles (OTR, RTS, TAFS apps) were not checked, beyond Love's/AscendTMS.

---

## Key question 3: Buyers and reachability. How many buyers are there, and can one person reach them?

### Takeaway
**K02:** California had **7,926 licensed used-vehicle dealers** (plus 2,333 new-vehicle dealers) as of Jan 1 2024. That is a small but concentrated universe, which caps K02 at roughly $40–60k MRR even at high share. The DMV does not offer a free bulk download, but county dealer lists can be ordered ($39–$117 per county per a DMV fee page, to verify), and the online lookup is public. The lists carry no emails, so outreach is phone, walk-in or mail first. **K03:** buyers number in the hundreds of thousands and are listable through the daily FMCSA Company Census on data.transportation.gov. Email coverage is partial (about 55% via the SMS census, per a vendor), and paid daily-lead feeds exist from about $20 per 1,000 leads. Reach is high; the problem is willingness to pay, not reach.

### Cited Findings
**K02: buyer count**
- California DMV facts: **New Vehicle Dealers 2,333 and Used Vehicle Dealers 7,926** (as of Jan 1 2024) — [DMV Top Ten Facts](https://www.dmv.ca.gov/portal/file/top-ten-california-dmv-facts-pdf)
- The 2020 version listed 1,517 new and **8,307 used** — [DMV EXEC 66 (2020)](https://www.dmv.ca.gov/portal/uploads/2020/10/EXEC-66-R6-2020-AS-WWW.pdf)
- I found no newer count — [search summary](https://www.dmv.ca.gov/portal/file/top-ten-california-dmv-facts-pdf)
- Don't confuse these with BAR repair-dealer counts (35,431 at Mar 31 2026) — [BAR](https://www.bar.ca.gov/arsc/newsletters/newsletter/spring-2026/licensing-data)

**K02: getting the list**
- The DMV's Occupational License Lookup shows dealer license status, ownership and disciplinary history — [DMV](https://www.dmv.ca.gov/portal/?p=1647)
- Printouts not in the lookup need form **OL 100** plus a $5 fee (form dated 9/2015) — [OL 100](https://dmv.ca.gov/portal/file/request-for-occupational-licensing-information-ol-100-pdf)
- A DMV fee schedule lists **dealer lists by county: Los Angeles $117, Orange $78, all other counties $39**. This is from a Spanish-language portal page; verify — [DMV (es)](https://qr.dmv.ca.gov/portal/es/?p=1560)
- Other records go through Public Records Act requests. Residence addresses and SSNs are not released — [DMV records request](https://www.dmv.ca.gov/portal/customer-service/records-request/); [DMV FFDMV-4](https://www.dmv.ca.gov/portal/driver-education-and-safety/educational-materials/fast-facts/public-information-request-ffdmv-4/)
- No bulk statewide download was found — [search summary](https://www.dmv.ca.gov/portal/customer-service/records-request/)

**K02: communities and channels**
- **CNCDA** (franchise dealers) is active on CARS Act education with ComplyAuto and Reynolds — [CNCDA](https://www.cncda.org/events/carsact_complyauto/)
- **NIADA** covers the law — [NIADA](https://niada.com/blog/california-passes-cars-act/)
- A California independent-dealer association running CARS Act events **did not surface**. Search hits for "CIADA" were the Carolinas association — [theciada.com](https://theciada.com/)
- Searches returned no r/askcarsales threads on the CARS Act — [search summary](https://consumerlaw.berkeley.edu/news/cars-act-sb766-brings-best-nation-protections-california-car-buyers)

**K03: buyer count and lists**
- The **USDOT Company Census File** is public on data.transportation.gov (dataset az4n-8mr2) and updated daily. Filtering on add_date finds new registrations — [OpenNetZero dataset mirror](https://opennetzero.org/us-department-of-transportation/company-census-file); [O Trucking guide](https://otrucking.com/resources/guides/fmcsa-new-carrier-list/)
- There is "no official one-click New Carrier List" — [O Trucking](https://otrucking.com/resources/guides/fmcsa-new-carrier-list/)
- **Email coverage:** a vendor feed pulls email from the separate SMS Census (kjg3-diqy) and claims about **55% coverage**. New carriers appear about 2–3 days after registration. A new USDOT registration is not yet operating authority; the feed catches a roughly 21-day pre-authority window — [Apify FMCSA new-authority actor](https://apify.com/foo121/fmcsa-new-authority)
- **Paid lead feeds** sell daily new-carrier leads with email from about **$20 per 1,000 leads** — [Apify listing](https://apify.com/transparent_meteorite/fmcsa-new-carrier-leads); [other Apify feeds](https://apify.com/jobito/fmcsa-new-authority-feed). Data-use terms are unverified.
- **Market trend:** the for-hire carrier population was roughly flat in 2025, with revocations offsetting new grants. FTR's Avery Vise says there are still about **86,000 more for-hire firms than before the pandemic (+33%)** — [Trucking Dive](https://www.truckingdive.com/news/fmcsa-grants-reinstatements-revocations-operating-authority-2025-data/808968/)
- For-hire carriers with **1–6 power units declined steadily through 2025** — [Datawrapper chart](https://datawrapper.dwcdn.net/7Adxc/1/)
- FMCSA's Registration Statistics page has a Feb 27 2026 snapshot, but I could not read its figures — [FMCSA A&I](https://ai.fmcsa.dot.gov/registrationstatistics)
- A third-party aggregator counts **322,646 active FMCSA-registered motor carriers in California** (Mar 9 2026), including non-freight entities — [usdotscore.com](https://usdotscore.com/state/california)
- New Jersey has about 12,000 IFTA accounts — [NJ MVC](https://www.nj.gov/mvc/business/ifta.htm)

### Inferences
- **K02 ceiling:** at about 7,900 used dealers, $10k MRR at $69/mo needs about 145 rooftops (1.8% of dealers). $5k needs about 72 (0.9%). Both are feasible shares, but the total ceiling is low: even 10% share at $69 is about $55k MRR.
  - Many of the 7,926 are tiny wholesale-only or home-office licensees with few retail deals. The real retail target is probably smaller (judgment).
- **K02 outreach:** buying LA, Orange, Riverside, San Bernardino and Central Valley county lists costs a few hundred dollars. The lists will have business addresses and phones, not emails. A solo founder would rely on phone calls, walk-ins (lots cluster on auto rows), direct mail and enrichment from Google Maps or Yelp listings. That is slower than email but has high response from owner-operators (judgment).
- **K03:** reach is not the constraint. New-authority carriers can be listed daily for almost nothing.
  - Brand-new carriers are the most price-sensitive and have the highest failure rate (the 1–6 truck segment is shrinking).
  - They are also already pitched by ELD vendors, factoring companies and free TMS bundles in their first weeks (judgment).
- **K03 TAM:** if New Jersey alone has about 12,000 IFTA accounts, the national IFTA licensee base is plausibly in the low hundreds of thousands. Even 0.2% share is about 500 customers (extrapolation, unverified).

### Gaps
- I have no current (2025–2026) DMV used-dealer count, and no split of retail lots versus wholesale-only licensees.
- I have no confirmed national count of IFTA licensees or of for-hire carriers by fleet size; the FMCSA and IFTA pages were unreachable.
- I could not verify which California Facebook groups exist for independent dealers, or their size.

---

## Key question 4: Demand signals. Is there 2025–2026 evidence of dealer confusion over the CARS Act or trucker pain over IFTA?

### Takeaway
**K02:** Trade-press and association signals are strong. "Dealers rush to comply", confusion between the FTC's approach and SB 766, an 80-page CNCDA guide, and $99 webinars all point the same way. Consumer press coverage is heavy (NBC, SlashGear, Jalopnik, SF Chronicle, Berkeley Law), which means buyers know about the 3-day right and dealers will see cancellations. I found no Reddit or forum threads, so first-person independent-dealer pain is **unverified**. **K03:** pain evidence is old or vendor-written: a 2011-era forum post about owing about $1,200 for lost receipts, and spreadsheet templates on Payhip and Etsy. There is clear evidence that people pay small amounts ($27 templates, $20–25 reports), but no 2025–2026 evidence of unmet demand.

### Cited Findings
**K02**
- "California dealers rush to comply with CARS Act" on top of FTC rules — [Dealership Guy](https://news.dealershipguy.com/p/on-top-of-ftc-rules-california-dealers-rush-to-comply-with-cars-act)
  - The main confusion is that FTC implementation guidance conflicts with SB 766 on what goes into "total price". CNCDA advised following the FTC approach. The association warns that confusion "becomes a serious liability for dealers without the staff or resources".
  - CNCDA's president said dealers making an honest effort "should have time to adjust" (same source).
- **Trade and legal coverage:** Auto Remarketing ran an Nov 2025 feature and a podcast on "Regulation like vacated CARS Rule rises in California" — [Auto Remarketing Nov 2025](https://digital.autoremarketing.com/november-2025/page-52); [Auto Remarketing podcast](https://www.autoremarketing.com/?p=80108). CBT News has a CARS Act hub — [CBT News](https://www.cbtnews.com/california-cars-act/). The used-car dealer magazine UCD covered advocacy in July 2025 — [UCD Magazine](https://digitaleditions.walsworth.com/article/Advocacy/5007171/849270/article.html)
- **Consumer awareness:**
  - [NBC Bay Area](https://nbcbayarea.com/news/local/car-dealer-new-law-price-consumer/4151010)
  - [NBC San Diego](https://www.nbcsandiego.com/news/local/car-dealer-new-law-price-consumer/4080735/)
  - [SlashGear, Oct 2026](https://www.slashgear.com/2276764/new-california-car-buying-laws-october-2026-cars-act/)
  - [Jalopnik](https://jalopnik.com/2005998/california-cars-act-protects-used-car-buyers)
  - [SF Chronicle](https://preview-prod.w.sfchronicle.com/personal-finance/article/buy-car-law-california-21090698.php)
  - [Berkeley Center for Consumer Law](https://consumerlaw.berkeley.edu/news/cars-act-sb766-brings-best-nation-protections-california-car-buyers)
- **Vendor demand-creation:** KPA's webinar series — [KPA](https://kpa.io/webinar/ca-cars-episode-2-3-day-cancellation-payment-transparency-deal-disclosures/); SnapInspect's blog — [SnapInspect](https://blog.snapinspect.com/california-sb-766/); the condition-documentation press release — [KDH News](https://kdhnews.com/online_features/press_releases/californias-new-3-day-used-car-return-law-puts-vehicle-condition-documentation-in-the-spotlight/article_645ad4a1-01c5-567b-894a-6039e8f99064.html)
- Searches returned no r/askcarsales threads — [search, Oct 10 2026](https://www.carpro.com/blog/the-new-cars-act-has-started)
- I found no reporting on first-week return volumes or enforcement — [search, Oct 10 2026](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/)

**K03**
- **Receipts:** a TruckersReport thread has owner-operators discussing per-quarter IFTA cost. One owed about $1,200 for a quarter after missing receipts (an old, about 2011 thread) — [TruckersReport](https://www.thetruckersreport.com/truckingindustryforum/posts/2294530)
- **Card statements aren't enough:** vendor guides say a card statement without the individual receipt (date, jurisdiction, gallons, vehicle) can get tax-paid credit rejected, and that mileage estimated from maps is an audit red flag — [Oxmaint guide](https://oxmaint.com/industries/fleet-management/ifta-fuel-tax-documentation-fleet-compliance-guide-2026); [Heavy Vehicle Inspection guide](https://heavyvehicleinspection.com/blog/post/ifta-fuel-tax-reporting-guide-2026-fleets). Vendor content; I could not tell which guide made each claim.
- **Spreadsheet market:** Payhip and Etsy sellers offer IFTA trackers at about $27 — [Payhip](https://payhip.com/b/zQl2s); [Etsy](https://www.etsy.com/listing/4533491676/)
- Searches returned no Reddit (r/Truckers or r/OwnerOperators) threads — [search, Oct 10 2026](https://greenlane.ai/blog-posts/complete-guide-to-ifta-reporting)

### Inferences
- **K02:** the demand signal is "institutional anxiety", visible in association guides, webinars and vendor marketing. Independent dealers are the least resourced to absorb it, which fits the wedge.
  - Because consumers are widely told about the 3-day right, cancellations will actually happen. That makes the refund clock and condition proof an operational problem, not just a paperwork one.
  - Direct dealer quotes are still missing. **Do 10 discovery calls before writing code.**
- **K03:** the pain is real but well served. The evidence shows that owner-operators pay $20–$60 a quarter or use spreadsheets, not that they are searching for a new tool.

### Gaps
- I have no first-person 2026 posts from California independent dealers (Facebook groups were not searchable here).
- I have no keyword-volume data ("CARS Act 3 day return form", "IFTA calculator"), because no SEO tool was available.
- I have no 2025–2026 Reddit evidence for IFTA pain.

---

## Key question 5: Build feasibility and liability. Can one developer with Claude build it in 4–6 weeks, and what are the legal exposures?

### Takeaway
Both are buildable as mobile web apps in 4–6 weeks. **K02:** CRUD, timers, photo capture, e-sign and PDFs. Liability is moderate: the product encodes one state's rules, so a wrong fee or deadline creates dealer exposure. Mitigations are a statute-checked rules table, attorney-reviewed templates, a "dealer remains responsible" disclaimer (Tekion uses the same framing) and E&O insurance. Buyer ID and deal documents also bring FTC Safeguards Rule (GLBA) expectations, which were not researched. **K03:** inputs are easy: Motive and Samsara expose jurisdiction mileage and fuel CSVs, and fuel cards export CSV. Tax math needs IFTA's quarterly rate matrix. Liability is a tax-calculation error, but the carrier signs and files, as the corpus noted.

### Cited Findings
**K02**
- **What the law needs captured:**
  - 3-calendar-day window starting the day after signing [SlashGear](https://www.slashgear.com/2004828/california-2026-new-car-buying-law/)
  - 400-mile cap and $1/mile fee over 250 miles [CBT News](https://www.cbtnews.com/?p=252530)
  - condition at delivery [Jalopnik](https://jalopnik.com/2005998/california-cars-act-protects-used-car-buyers)
  - separate 3-day cancellation disclosure plus contract first-page notice [PolicyRisk](https://policyrisk.com/state-bill/CA-SB766-20252026)
  - trade-in return or highest-value payout [PolicyRisk](https://policyrisk.com/state-bill/CA-SB766-20252026)
  - 2-year retention of price communications and cancellation documents [DMV memo](https://www.dmv.ca.gov/portal/file/26olin10-pdf/)
- **Disclaimer pattern:** Tekion tells dealers they "remain fully responsible for their own compliance" — [Tekion](https://tekion.com/blog/preparing-for-cars-act-and-ftc-pricing-compliance-what-dealers-need-to-know). Fullpath's agent "never approves a cancellation itself" — [Fullpath](https://help.fullpath.com/hc/en-us/articles/53305019188500-Compliant-Agent-Onboarding-California-CARS-Act)
- **Forms:** CARS Act disclosures may be added to the existing California Pre-Contract Disclosure form, so the forms already come from forms vendors and need not come from us — [Ginsburg Law Group](https://ginsburglawgroup.com/?p=17652). CNCDA/Reynolds forms exist for franchise dealers — [CNCDA](https://www.cncda.org/events/carsact_newformswebinar/)
- **Integration:** DMS exports (DealerCenter/Frazer CSV) are assumed by the corpus but were not verified — [Corpus K02]

**K03**
- **Motive:** IFTA Trip Reports export by quarter. Fuel comes from the Motive Card, receipt uploads or vendor CSV import — [Motive help](https://helpcenter.gomotive.com/hc/en-us/articles/30897108333213-Trip-Reports); [Motive IFTA](https://gomotive.com/products/fleet-compliance/ifta-fuel-tax-reporting/)
- **Samsara:** IFTA Mileage report (ECU distance with GPS fallback), fuel CSV import, WEX/Fleetcor integration. A native CSV export of state mileage is **not confirmed** in Samsara's own article; third parties show "By State/By Truck" exports — [Samsara KB](https://kb.samsara.com/hc/articles/360046354291); [DataTruck](https://support.datatruck.io/hc/en-us/articles/50522581636243-How-to-Generate-a-Samsara-IFTA-Report)
- **Audit binder contents:** auditors want IVMRs or trip sheets, GPS data at 10-minute intervals, individual fuel receipts and bulk fuel logs, kept 4 years — [Minnesota DPS](https://dps.mn.gov/divisions/dvs/business/irp-and-ifta/irp-and-ifta-audit/irp-and-ifta-audit-record-keeping-requirements); [J.J. Keller](https://jjkellercompliancenetwork.com/regsense/individual-vehicle-mileage-report-ivmr)
- **Rate tables:** IFTA rates change quarterly. ExpressTruckTax blogs on Q3 rate changes — [ExpressTruckTax](https://blog.expresstrucktax.com/what-you-need-to-know-about-3rd-quarter-ifta-rate-changes/)

### Inferences
- **K02 build, 4–5 weeks:**
  - VIN deal record (NHTSA decode)
  - eligibility check (used, $50k or less, not exempt)
  - countdown to end of day 3, with SMS/email alerts
  - odometer out/in with the 400-mile cutoff and the 250-mile fee
  - restocking-fee calculator
  - 48-hour refund timer
  - trade-in "do not wholesale until [date]" hold flag
  - guided 12–20 photo walk-around plus odometer photo, buyer e-sign on a phone, PDF certificate
  - 2-year (default 4+ year) archive
  - Liability control: every computed number shows the rule and a statute citation, and the dealer confirms it.
- **K03 build, 4–6 weeks:**
  - CSV parsers (Motive, Samsara, generic)
  - fuel-card CSV and Claude-vision receipts
  - rate table
  - per-jurisdiction worksheet
  - binder PDF
  - The hard part is not the build. It is maintaining parsers across many ELDs and handling edge cases (bulk fuel, reefer fuel, Canadian provinces, surcharges such as Kentucky/Indiana), with peak support load in the week before each deadline (judgment).

### Gaps
- I have no confirmed DealerCenter or Frazer export formats.
- I did not research whether FTC Safeguards Rule vendor obligations apply to a tool storing buyer IDs.
- E&O insurance cost was not researched.
- IFTA, Inc. rate-matrix access and terms were not confirmed (site unreachable).

---

## Key question 6: Verdicts, refined wedges, prices, first-30-day sales plans and revenue paths

### Takeaway
- **K02: BUILD-IF.** Build it if, by about Oct 24 2026, (a) at least 5 of 10 California independent dealers say their DMS or forms vendor gives them no 3-day clock, condition proof or refund workflow and they would pay about $49–69/mo, and (b) the SB 766 fee and refund numbers are confirmed against the chaptered text, with a dealer attorney agreeing to review templates.
  - The trigger is live, the build is small, there is no direct cheap competitor I could find, and the buyer pays by card.
  - The ceiling is about 7,900 dealers in one state, and DMS vendors are the main threat.
  - Realistic path: **$5k MRR in about 6–9 months, $10k MRR in about 12–18 months.**
- **K03: DON'T BUILD as a standalone SaaS.** The calculation is commoditized ($0–$25), new AI receipt apps launched in 2026 (FleetCollect at $9/mo, SureMile), and the ELDs already produce jurisdiction mileage. ARPU near $20–30 means 170–530 customers for $5–10k MRR, with seasonal churn.
  - Only a materially different angle is worth a 2-week smoke test: a done-for-you "IFTA close and audit binder" productized service, or a white-label for a factoring company.

### Cited Findings
- **K02 price context:**
  - DMS: DealerCenter $99/mo and Frazer $129–$199/mo (corpus, Sep 2026) — [Frazer pricing](https://www.frazer.com/frazer-pricing)
  - Association webinar: $99 for CNCDA members — [CNCDA](https://www.cncda.org/events/carsact_complyauto/)
  - The maximum restocking fee a dealer can recover is $600 plus a $150 mileage charge — [CBT News](https://www.cbtnews.com/?p=252530)
  - Violations run through UCL/CLRA and possible license action — [DMV CARS Act page](https://www.dmv.ca.gov/portal/vehicle-registration/new-registration/registering-a-vehicle-purchased-from-a-dealer/california-combating-auto-retail-scams-act/)
- **K02 buyer count:** 7,926 used dealers (Jan 1 2024) — [DMV](https://www.dmv.ca.gov/portal/file/top-ten-california-dmv-facts-pdf)
- **K02 list cost:** LA $117, Orange $78, other counties $39 (to verify) — [DMV (es)](https://qr.dmv.ca.gov/portal/es/?p=1560)
- **K03 price context:**
  - FleetCollect from $9/mo — [24-7 Press Release](https://www.24-7pressrelease.com/press-release/531872/fleetcollect-launches-ifta-tracking-software-and-fleet-dqf-platform-to-automate-compliance-for-trucking-companies)
  - ExpressIFTA from $19.95/mo; Geotab $19.95–$24.95 per report — [Guideflow](https://www.guideflow.com/blog/ifta-reporting-software)
  - TruckLogics $24.95 per report, or $35.96/mo full TMS — [TruckLogics blog](https://blog.trucklogics.com/start-generating-your-3rd-quarter-ifta-report-with-trucklogics-now-the-deadline-is-october-31st/); [Empwr](https://www.empwrtrucking.com/freight-technology/trucklogics-tms-review-for-small-fleets-simplify-dispatch-and-compliance/)
  - AscendTMS free through partners — [FreightWaves](https://freightwaves.com/news/loves-offers-ascendtms-free-to-its-factoring-customers)
- **K03 deadlines:** Q4 2026 due Feb 1 2027 — [Georgia DOR](https://dor.georgia.gov/ifta-due-dates)
- **K03 audit rate:** about 3% a year — [Keller Encompass](https://eld.kellerencompass.com/resource/blog/what-is-ifta)

### Inferences

All of the following is judgment built on the findings above.

#### K02 "CARS Act 3-Day Log": verdict BUILD-IF

**Refined wedge.** The pitch is "Prove the car's condition, never miss the 3-day or 48-hour clock, and keep the 2-year file." It sits beside the DMS and the forms vendor, and drafts no contracts.
1. **Delivery Kit (phone, about 3 minutes):**
   - VIN scan or decode.
   - Odometer photo.
   - A guided 12–20 photo walk-around with timestamps and GPS.
   - The buyer e-signs "condition and odometer acknowledged" plus receipt of the 3-day cancellation form, which is uploaded or photographed from the dealer's forms vendor.
   - A PDF certificate is texted or emailed to the buyer.
2. **3-Day Board:**
   - Every open cancellation window, with a countdown to the end of day 3.
   - Trade-in "hold, don't wholesale" flags.
   - Alerts to the owner or GM.
3. **Return desk:**
   - Odometer in, set against the 400-mile cutoff.
   - Side-by-side condition photo comparison.
   - Restocking and mileage fee calculator showing the statute cite.
   - A **48-hour refund timer** with escalation.
   - Trade-in disposition record.
   - A signed return receipt.
4. **2-year binder:** a per-deal PDF and a search-by-VIN or buyer export for DMV or attorney requests.
5. **Later, not v1:** a "first written price quote" log for the total-price rule (needs email/SMS capture), DMS CSV import, and a Spanish-language buyer screens toggle.

**Price.**
- **$59/mo per rooftop**, unlimited deals, 14-day free trial, card only. Or **$590/yr**.
- A **$29/mo "Lite" tier for lots doing fewer than 15 retail deals a month** keeps tiny lots from churning to paper.
- A **$149 one-time "CARS Act setup"** includes a signage pack, staff checklist and template review notes. Use this only after an attorney has reviewed them.
- Rationale: below the $99–$199 DMS bill, and roughly equal to one restocking fee every 10 months.

**First 30 days (Oct 10 to Nov 9 2026):**
- **Days 1–3:**
  - Confirm the SB 766 text on leginfo (fees, refund timing, trade-in formula).
  - Order the DMV county dealer lists for LA, Orange, Riverside, San Bernardino and Fresno/Kern (about $39–$117 each), or scrape the public lookup.
  - Line up one California dealer attorney as reviewer and possible co-marketer.
- **Days 3–10:**
  - Ship a free "CARS Act 3-Day Return Calculator" page: eligibility, end-of-window date, 400/250-mile logic, fee math, trade-in hold date. It works as an SEO and lead magnet.
  - Run 10–15 discovery calls or walk-ins on one auto row (for example in the Inland Empire). Ask what their DMS or forms vendor already provides, how many cancellations they have had since Oct 1, and how they prove condition today.
- **Days 10–24:**
  - Build the Delivery Kit, 3-Day Board and Return desk.
  - Run 3–5 design-partner lots free for 30 days in exchange for feedback and a testimonial.
- **Days 24–30:**
  - Convert design partners at a "founding" $39/mo locked for 12 months.
  - Start a cadence of about 50 dials a day plus a postcard (QR code to the calculator) to about 1,000 lots.
  - Pitch dealer-licensing schools (e.g., CA Dealer Academy, per the corpus) and forms vendors on a referral fee.
- **Target:** 5 paying rooftops by day 45.

**Revenue path.**

| Price | Customers for $5k MRR | Customers for $10k MRR | Share of 7,926 used dealers |
|---|---|---|---|
| $49 | 102 | 204 | 1.3% / 2.6% |
| $59 | 85 | 169 | 1.1% / 2.1% |
| $69 | 72 | 145 | 0.9% / 1.8% |
| $79 | 63 | 127 | 0.8% / 1.6% |

- Realistic pace for one founder doing phone and walk-in sales: 8–15 new rooftops a month after month 2, with low churn because the binder accumulates.
- At $59 that gives **$5k MRR in about 6–9 months (around Apr–Jul 2027)** and **$10k MRR in about 12–18 months (around Q4 2027–Q1 2028)**.
- Upside: a forms-vendor or DMS referral partner doubles the pace.
- Downside: DealerCenter or Frazer ships a free 3-day module, which caps growth at whoever values the photo proof.
- **Kill if:** discovery calls show the DMS or forms vendor already provides a 3-day tracker plus condition photos, or dealers report almost no cancellations by mid-November.

#### K03 "IFTA Close": verdict DON'T BUILD (standalone SaaS)

**Why.**
- Competitors at $0–$25:
  - free calculators (ExpressIFTA app)
  - $9/mo FleetCollect with receipt photos (Feb 2026)
  - an AI receipt app (SureMile, Apr 2026)
  - $19.95–$24.95 per-report tools (TruckLogics, Geotab)
  - $35.96/mo TMS with IFTA (TruckLogics)
  - free AscendTMS through DAT and Love's
- ELDs (Motive, Samsara, even small ones like Roadeazy) already output the jurisdiction mileage that is the hard input.
- The quarterly cadence drives 3-of-4-month disuse and churn.
- At a market-clearing $19–29/mo, $5k MRR needs 172–263 customers and $10k needs 345–526. Combined with seasonal churn, that is likely **18–30+ months to $10k MRR** for a solo founder.

**If the founder still wants trucking, two "build-if" alternatives (each with a 2-week smoke test before any build):**
1. **"IFTA Close and Audit Binder" as a productized service**, at about $79–$129 per quarter per carrier (1–5 trucks).
   - The customer forwards an ELD export and a fuel-card CSV and snaps missing receipts.
   - Claude-assisted reconciliation produces a filing-ready worksheet. The carrier files, or uses the founder's portal walkthrough.
   - Includes a 4-year binder and missing-receipt chase texts.
   - The anchor is filing services reportedly in the low hundreds per quarter (unverified).
   - Customers needed: $5k MRR is about 150–190 carriers at about $26–$33/mo equivalent ($79–$99 a quarter), so the math is no better than SaaS and support spikes at each deadline. **Only build if** a smoke test in December 2026 for the Feb 1 2027 deadline gets 20+ prepaid quarters.
2. **"IFTA Audit Defense Pack"** (one-time $299–$499) for carriers who received an audit letter.
   - It rebuilds IVMR-style records from ELD and fuel data and organizes the 4-year binder.
   - Audits cover about 3% of licensees a year, which is plausibly thousands nationally, but this is one-shot revenue, not MRR.
   - **Build-if** a CPA or IFTA filing firm agrees to refer cases.

**First 30 days (if testing only):**
- Publish an "IFTA Q4 2026 due Feb 1 2027" checklist and a Motive/Samsara export walkthrough.
- Run a landing page with a prepaid $79 "we close your Q4" offer.
- Email 1,000–2,000 new-registration carriers from the FMCSA census or SMS census (where email exists).
- Pitch 3 small factoring companies on white-label.
- **Kill if** fewer than 10 prepay by Dec 15 2026.

### Gaps
- None of these verdicts rests on customer interviews; K02's BUILD-IF conditions are designed to supply them in the first 2 weeks.
- The monthly sales pace (8–15 rooftops a month) and the 6–9 and 12–18 month timelines are judgment. There is no benchmark for solo founders selling to California independent dealers.
- K02's price-tolerance evidence is indirect: DMS prices and $99 webinars. I found no direct comparison with a $29–$79 CARS Act point tool because none surfaced.
- K03's filing-service price anchor ("low hundreds per quarter") comes from weak sources and needs quotes from 3–5 real services.
