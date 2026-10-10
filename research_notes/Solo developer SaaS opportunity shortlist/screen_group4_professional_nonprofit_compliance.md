# Solo-developer screen, group 4: professional services (G01–G07), nonprofit/community (I01–I07) and compliance (J01–J07)

Scope and method. All 21 assigned idea files were read in full, along with INDEX.md sections 1–5 and 8, `_scoreboard.csv`, `_states_summary.csv` and the state files' rankings. Each idea was scored against `_solo_dev_rubric.md` (8 criteria, 1–5 each, /40), with kill flags. **No web search or fetch was done in this pass, by design.** Every external link below was fetched by the corpus authors on Sep 24–25 2026 and was not re-checked here. "(via G03)" means the claim and its link come from that corpus file. Corpus root: `/tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/`. Rubric scores, competitor names the corpus does not mention, and wedge designs are **my judgment**, and they appear only under Inferences or Gaps. Today is 2026-10-10.

---

## Q1. What are the 8 rubric scores and kill flags for each assigned idea, and why?

### Takeaway
Only 3 of the 21 ideas clear the solo-developer screen without a disqualifying flag: **I03 DuesDesk (28/40), G03 SeasonDesk (28/40) and J06 LicenseLedger (26/40)**. G06 AdvisorVault (26) and J03 PostedUp (26) are worth pursuing only as narrowed, validate-first wedges. The other 16 fail on at least one of these flags: a feature-parity product (practice management, accounting, payroll, AMS, ATS, ChMS, camp/club suites), core payment handling (I02, I04, I05), 50-state legal-rule liability (J01, J02, J04, J05, G04), a committee or government buyer (I07, J07), or a market full of free and cheap tools (G02, I01, I02, I04, I07, J02).

### Cited Findings

**G01 LawLedger (Clio/MyCase alternative with IOLTA trust accounting)**
- Clio shows Starter "from $49/user/mo", with Core, Signature and Elite at "pricing upon request". The early-2026 ladder was $49/$89/$149 per user ([Clio pricing via G01](https://www.clio.com/pricing/); [CounselStack via G01](https://www.counselstack.io/blog/legal-practice-management-software-pricing)).
- A Trustpilot reviewer reports a 34% per-user hike explained as the cost of AI (Aug 17 2026), plus complaints about forced AI enrollment ([Trustpilot via G01](https://www.trustpilot.com/review/clio.com)).
- The MVP list covers imports from 4 systems, matters, a conflict check, IOLTA ledgers, three-way reconciliation, time and billing, LEDES, Stripe trust/operating separation and intake. The file's own risk line says "Trust accounting errors are career-ending for lawyers", with E&O insurance and SOC 2 within 6–9 months as the mitigation ([corpus G01](ideas/G01-small-law-practice-trust-clio-mycase-alternative.md)).
- The corpus lists a "Crowded category" of MyCase $49–$89, PracticePanther $59–$99, Smokeball, CosmoLex $99, Actionstep and Lawcus ([CounselStack via G01](https://www.counselstack.io/blog/legal-practice-management-software-pricing)).

**G02 PlainLedger (QuickBooks Online/Xero alternative)**
- QBO list prices from Aug 1 2026: Essentials $85, Plus $140, Advanced $340. Plus is up 56% and Advanced up 70% in three years ([SWK via G02](https://www.swktech.com/2026-quickbooks-price-increases-what-they-mean-for-your-renewal/); [NerdWallet via G02](https://www.nerdwallet.com/article/small-business/quickbooks-pricing)).
- Xero US rose on Oct 1 2026: Early $25→$27, Growing $55→$59, Established $90→$97 ([Booksla via G02](https://www.booksla.com/xero-price-increase/)).
- The file itself says "Build ease is moderate, not easy… Expect a 6–8 week MVP" for a GL, bank feeds, reconciliation and reports. Buyers usually choose "on the advice of their outside bookkeeper or CPA" ([corpus G02](ideas/G02-smb-accounting-quickbooks-online-xero-alternative.md)).

**G03 SeasonDesk (TaxDome/Karbon/Canopy alternative for 1–15 person tax firms)**
- TaxDome's per-seat yearly prices are Essentials $800 (solo only), Pro $1,000 and Business $1,200. A Business seasonal seat costs $500 per 4-month term and auto-renews ([taxdome.com/pricing via G03](https://taxdome.com/pricing)).
- TaxDome was $600/yr before Feb 13 2023. On a 1-year term the Pro tier is now $1,000, about +67% ([TaxDome blog via G03](https://taxdome.com/blog/everything-you-need-to-know-about-taxdomes-first-ever-price-change)).
- Capterra complaints: pressure to prepay 3 years, months of configuration, no phone support, and document saves lagging near deadlines ([Capterra via G03](https://www.capterra.com/p/186749/TaxDome/reviews/)).
- The MVP is a magic-link portal, an AI organizer and document chaser, engagement e-sign, a kanban board, Stripe invoicing and a WISP generator. Buyers are owners of 1–15 person firms who buy in the Oct–Dec pre-season window ([corpus G03](ideas/G03-cpa-tax-practice-portal-taxdome-karbon-alternative.md)).
- Karbon, Canopy, Financial Cents and Liscio prices are "not verified this pass" ([corpus G03](ideas/G03-cpa-tax-practice-portal-taxdome-karbon-alternative.md)).

**G04 StatePay (Gusto/ADP alternative, starting as a state-compliance copilot)**
- Gusto Simple rose from $40 to $49/mo in March 2026 (+22%). Plus is $80 + $12/person ([HRPayPick via G04](https://hrpaypick.com/gusto-pricing/); [Gusto pricing via G04](https://gusto.com/product/pricing)).
- Maryland paid-leave contributions start Jan 1 2027. Minnesota, Delaware and Maine programs are live ([OnPay via G04](https://onpay.com/insights/paid-family-leave-by-state/)).
- Phase 1 includes a "paid-leave and sick-leave engine" with per-state and per-city accrual rules. Phase 2 is payroll on an embedded payroll partner, whose fees are "unknown". The file lists "Liability for compliance advice" as a risk ([corpus G04](ideas/G04-payroll-state-compliance-gusto-adp-alternative.md)).
- Corpus state files rank G04 in the top 3 for DE and MD ([_states_summary.csv](_states_summary.csv)).

**G05 AgencyLite (EZLynx/Applied Epic alternative for small P&C agencies)**
- QuoteSweep, a vendor blog, lists Applied Epic at about $500/mo plus $10K–$100K+ implementation, QQCatalyst at $129/user and NowCerts at $169/mo. EZLynx users report a 50% hike in 2023 ([QuoteSweep via G05](https://www.quotesweep.com/blog/ams-comparison-2026)).
- The file itself says "Carrier download (IVANS) and comparative raters are the real moat. Without them, AgencyLite is a CRM" ([corpus G05](ideas/G05-insurance-agency-ams-applied-epic-ezlynx-alternative.md)).

**G06 AdvisorVault (Redtail/Wealthbox CRM plus a compliance kit for small RIAs)**
- Redtail costs $39–$65/user/mo and Wealthbox $59–$99/user/mo. Wealthbox's AI notetaker is a $49/user/mo add-on ([Redtail pricing via G06](https://redtailtechnology.com/pricing/); [Wealthbox pricing via G06](https://www.wealthbox.com/pricing/)).
- The Reg S-P amendments, adopted May 2024, require an incident-response program, customer notice within 30 days and service-provider oversight ([SEC 2024-58 via G06](https://www.sec.gov/newsroom/press-releases/2024-58)). The small-entity date of about Jun 3 2026 is marked "verify" in the corpus.
- The file is flagged "**Evidence status: THIN**". No 2025–2026 complaints were collected ([corpus G06](ideas/G06-ria-crm-compliance-reg-sp-redtail-smarsh-alternative.md)).

**G07 BenchBoard (Bullhorn alternative for small staffing agencies)**
- Bullhorn complaints include auto-renewal despite cancellation (Aug 2026), "bullhorn jail" over excess licenses (Jun 2026) and failure to deliver a full data export ([Trustpilot via G07](https://www.trustpilot.com/review/bullhorn.com)).
- Bullhorn and JobDiva prices are unverified (quote-based). The MVP includes "Two-way SMS (10DLC registered)" and auto-texting of applicants, and temp back office and VMS come in V2 ([corpus G07](ideas/G07-staffing-ats-crm-bullhorn-alternative.md)).

**I01 GiftLedger (Raiser's Edge NXT/Bloomerang/Givebutter alternative)**
- Bloomerang's CRM starts at $125/mo and the Giving Platform at $242/mo, all billed annually. "Every plan includes unlimited users" ([Bloomerang pricing via I01](https://bloomerang.com/pricing/)).
- Givebutter adds a 15% default tip, and a class action was filed in April 2026 ([TINA.org via I01](https://truthinadvertising.org/articles/givebutters-hidden-fees/)).
- A competitor estimates RE NXT at $4k–$15k/yr plus $5k–$25k implementation ([AlignMint via I01](https://www.getalignmint.org/blog/blackbaud-pricing)).
- The file's own risk section says "Free competitors (Zeffy, Givebutter) set a '$0' anchor". Its timing note reads "switch before Giving Tuesday (Dec 1 2026) or wait until January" ([corpus I01](ideas/I01-nonprofit-donor-crm-blackbaud-bloomerang-givebutter-alternative.md)).

**I02 TitheBox (Pushpay/ChurchStaq alternative)**
- Pushpay sells 1–3 year contracts with no published prices, and early cancellation means paying the contract balance ([Pushpay pricing via I02](https://pushpay.com/product/pricing/)).
- Planning Center is modular with free tiers. Giving costs 2.15% + $0.30, with no contracts. The file concedes "Planning Center is liked and cheap" ([Planning Center via I02](https://www.planningcenter.com/pricing)).
- The MVP includes giving and text-to-give, plus kids' check-in with printed security tags that "must be rock-solid offline". Donors must re-enter cards unless a PCI token export is obtained ([corpus I02](ideas/I02-church-giving-chms-pushpay-alternative.md)).

**I03 DuesDesk (WildApricot/MemberClicks/GrowthZone alternative)**
- WildApricot costs $66/mo monthly for 100 contacts ([WildApricot pricing via I03](https://www.wildapricot.com/pricing)). A competitor reports April 2026 annual prices of $886 (250 contacts), $1,663 (500) and $5,238 (5,000), and a 20% surcharge for using an outside payment processor ([Groupable via I03](https://www.groupable.com/blog/wild-apricot-pricing-hidden-fees)).
- WildApricot is rated 1.3/5 on Trustpilot across 159 reviews. Complaints include a 27% renewal jump ($640→$810), a 9-month failed launch and an email editor and site builder that keep breaking (2026) ([Trustpilot via I03](https://www.trustpilot.com/review/wildapricot.com)).
- Momentive Software (owned by TA Associates) acquired Personify on Jan 6 2026. Analysts warn of "product rationalization and pricing optimization within 18–36 months" ([SmartThoughts via I03](https://www.smartthoughts.net/post/momentive-personify-acquisition-association-impact)).
- Users have long asked for a ~$25/mo plan on WildApricot's own wishlist forum ([WildApricot forums via I03](https://forums.wildapricot.com/forums/308932-wishlist/suggestions/13335057-low-level-pricing-plans-e-g-25)).
- The file names cheap competitors MembershipWorks, Groupable and Memberplanet. Clubs buy by card, and chambers "move quickly at renewal" ([corpus I03](ideas/I03-membership-associations-chambers-wild-apricot-alternative.md)).
- DC ranks I03 #1 ([DC state file](states/DC-district-of-columbia.md)).

**I04 DoorList (Eventbrite alternative)**
- Eventbrite charges 3.7% + $1.79 per ticket plus 2.9% processing ([Eventbrite pricing via I04](https://www.eventbrite.com/organizer/pricing/)).
- Bending Spoons closed its purchase on Mar 10 2026 and made layoffs. The file's own verification note says the trigger "rests on uncertainty and staff cuts, not an actual fee hike" ([Equaticket via I04](https://equaticket.com/blog/eventbrite-bending-spoons-what-organizers-need-to-know); [IQ Magazine via I04](https://www.iqmagazine.com/2026/04/eventbrite-makes-layoffs-following-bending-spoons-acquisition/)).
- The file lists "Crowded field: Ticket Tailor, Humanitix, SimpleTix and TicketSpice". Payouts run through Stripe Connect, and chargebacks and fraud are listed as risks ([corpus I04](ideas/I04-event-ticketing-small-organizers-eventbrite-alternative.md)).

**I05 ClubHouse (TeamSnap ONE/SportsEngine alternative)**
- TeamSnap is rated 1.1/5 across 692 reviews. One admin says the forced move to TeamSnap ONE took their admin work from 2 hours a week to 2 hours a day (Mar 2026) ([Trustpilot via I05](https://www.trustpilot.com/review/teamsnap.com)).
- The buyer is a club board ("the board signs"). The MVP includes dues installments, payments, SMS blasts and storing minors' birth certificates ([corpus I05](ideas/I05-youth-sports-clubs-leagues-teamsnap-sportsengine-alternative.md)).

**I06 CampFile (CampMinder alternative)**
- The ACA counts 14,000+ camps ([ACA via I06](https://www.acacamps.org/press-room/aca-facts-trends)).
- No 2025–26 price hike was found, and the only window is seasonal (Sep–Dec, before registration opens Nov–Jan). The MVP includes a daily medication-administration log and a staff app ([corpus I06](ideas/I06-summer-camps-after-school-campminder-ultracamp-alternative.md)).

**I07 SchoolPing (ParentSquare/Remind alternative for private and charter schools)**
- ParentSquare is quote-based. A reviewer says "any feature will cost you thousands per year" ([Software Advice via I07](https://www.softwareadvice.com/school-administration/parentsquare-profile/reviews/)).
- The MVP includes SMS, a Twilio voice fallback and A2P 10DLC registration "for each school". Student-data privacy agreements are needed state by state ([corpus I07](ideas/I07-k12-parent-communication-private-charter-parentsquare-alternative.md)).

**J01 NexusBook (TaxJar/Avalara alternative)**
- TaxJar month-to-month customers move to new pricing on Oct 1 2026. Professional annual prices rise 110–128% at 2.5K–25K orders, and AutoFile goes from $35 to $55 ([TaxCloud via J01](https://taxcloud.com/blog/taxjar-price-increase-2026/); [TaxJar support via J01](https://support.taxjar.com/article/139-how-much-does-taxjar-cost)).
- The file names VC-backed challengers Zamp, Numeral, Kintsugi, TaxCloud, Taxwire and Galvix, and lists "Rate accuracy liability" as a risk. The MVP must integrate with 5+ commerce platforms and cover all 46 taxing jurisdictions ([corpus J01](ideas/J01-sales-tax-nexus-filing-avalara-taxjar-alternative.md)).
- KY and NH rank J01 in their top 3 ([_states_summary.csv](_states_summary.csv)).

**J02 SiteShield (Termly/Osano alternative plus accessibility scanning)**
- Termly costs $10–$15/mo, CookieYes $10–$55, and Osano jumps from free to $199/mo ([Consently via J02](https://consently.net/blog/consent-management-platform-pricing)).
- There were 3,117 federal ADA web suits in 2025 ([Seyfarth via J02](https://www.adatitleiii.com/2026/03/federal-court-website-accessibility-lawsuit-filings-bounce-back-in-2025/)), and 1,300+ suits hit sites running overlays ([UsableNet via J02](https://blog.usablenet.com/ada-web-lawsuit-trends-2026)).
- The file itself says "Crowded, cheap category" and "Against Termly alone, our price is roughly at parity". Its risks include "Unauthorized practice of law" ([corpus J02](ideas/J02-smb-privacy-cookie-accessibility-compliance-termly-osano-alternative.md)).

**J03 PostedUp (Poster Guard/GovDocs/Mineral alternative)**
- Poster Guard's e-service costs $15.95 per remote employee per year, and it lists five mandatory poster changes in Sep 2026 alone ([posterguard.com via J03](https://www.posterguard.com/)).
- Pay-transparency rules differ by state: NJ from Jun 1 2025, VT Jul 1 2025, MA Oct 29 2025 (25+ employees), WA's 5-day cure, CA's Jan 1 2026 amendment, and DE from Sep 26 2027 ([Hunton via J03](https://www.hunton.com/hunton-retail-law-resource/several-states-enact-pay-transparency-laws-what-employers-need-to-know-in-2026)).
- Scam mailers demand $114 for posters that are free ([KSL via J03](https://www.ksl.com/article/news/features/ksl-investigates/small-business-owner-warns-of-letters-threatening-fines-for-noncompliance-over-workplace-posters/51572864)).
- The proposed price is $9/mo per location. The file says "Content accuracy is the product. We would need a small legal-ops team", and notes that no direct user reviews were captured ([corpus J03](ideas/J03-smb-employment-law-posters-pay-transparency-poster-guard-mineral-alternative.md)).
- CT and MA rank J03 #1 ([CT state file](states/CT-connecticut.md); [MA state file](states/MA-massachusetts.md)).

**J04 TagTrue (cannabis/hemp compliance alongside Metrc)**
- H.R. 5371, signed Nov 12 2025, caps hemp at 0.4 mg THC per container. The effective date of about Nov 12 2026 is marked "not verified" ([Wikipedia via J04](https://en.wikipedia.org/wiki/2025_United_States_federal_government_shutdown)).
- Metrc API access "requires each state's integrator approval". The file notes that hemp demand "may collapse" ([corpus J04](ideas/J04-cannabis-hemp-compliance-metrc-reconciliation-dutchie-alternative.md)).

**J05 CellarPermit (ShipCompliant alternative for alcohol direct-to-consumer shipping)**
- ShipCompliant is used by "more than 2,000" producers, and its pricing is unpublished ([Sovos via J05](https://www.sovos.com/shipcompliant/)).
- The file itself says "We have no hard dated switching event. This is a weakness". The product depends on a state-by-state rules matrix, and "a compliance miss risks the permit" ([corpus J05](ideas/J05-winery-brewery-distillery-dtc-shipping-compliance-shipcompliant-alternative.md)).

**J06 LicenseLedger (CE Broker/Harbor Compliance/LegalZoom alternative)**
- CE Broker is rated 1.5/5 on 37 reviews, 94% of them 1-star. Reviewers say they must upgrade to see their own transcript, and that credits show "Not completed" ([Trustpilot via J06](https://www.trustpilot.com/review/cebroker.com)).
- FinCEN's final rule (Aug 11 2026) exempts US companies from BOI reporting ([FinCEN via J06](https://www.fincen.gov/boi)).
- Proposed pricing is Individual $29/yr and Team $4 per staff member per month. The file notes "Low individual willingness to pay" ([corpus J06](ideas/J06-professional-license-ce-tracking-entity-compliance-cebroker-legalzoom-alternative.md)).
- In Florida, CE records are checked through CE Broker at renewal for "200+ license types in more than 40 health care professions" ([FL HealthSource via FL state file](https://www.flhealthsource.gov/)).
- Delaware corporate franchise tax and the annual report are due Mar 1, and the LLC tax is $400, due Jun 1 ([DE Corporations via DE state file](https://corp.delaware.gov/frtax/)).
- DE and WY rank J06 in their top 3, and FL ranks it #4 ([_states_summary.csv](_states_summary.csv); [FL state file](states/FL-florida.md)).

**J07 StationLog (NERIS reporting for volunteer fire departments)**
- NFIRS was retired on Jan 31 2026. 20,945 departments filed 2025 data ([USFA via J07](https://www.usfa.fema.gov/nfirs/)).
- Whether a free government NERIS entry path exists "was not verified". "Sales speed is honestly slow… board or council approval". No user complaints were captured ([corpus J07](ideas/J07-small-government-volunteer-fire-neris-reporting-tyler-civicplus-eso-alternative.md)).

### Inferences

#### Score table (solo-developer rubric, 1–5 each, /40; my judgment)
Column key: Build = solo build scope · Reg = regulatory/liability · Self = self-serve sale · Dist = solo-reachable distribution · WTP = willingness to pay/ARPU · Gap = gap versus cheap indie tools · Urg = urgency Oct 2026–Apr 2027 · Supp = support load and retention.

| ID | Product (replaces) | Build | Reg | Self | Dist | WTP | Gap | Urg | Supp | **/40** | Kill flags | Verdict |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| I03 | DuesDesk (WildApricot) | 3 | 4 | 4 | 4 | 3 | 2 | 4 | 4 | **28** | Crowded-cheap (partial) | **Shortlist #1** |
| G03 | SeasonDesk (TaxDome) | 3 | 3 | 4 | 4 | 5 | 2 | 4 | 3 | **28** | None hard; crowded portal space (partial) | **Shortlist #2** |
| J06 | LicenseLedger (CE Broker / LegalZoom) | 3 | 3 | 5 | 4 | 2 | 3 | 3 | 3 | **26** | 50-state rules (partial, low stakes) | **Shortlist #3** (team-plan wedge) |
| G06 | AdvisorVault (Redtail + compliance) | 3 | 2 | 4 | 3 | 5 | 2 | 3 | 4 | **26** | None hard; thin evidence | **Conditional #4** |
| J03 | PostedUp (Poster Guard / Mineral) | 3 | 2 | 5 | 4 | 2 | 2 | 5 | 3 | **26** | 50-state + city legal rules | **Conditional #5** (narrowed) |
| J01 | NexusBook (TaxJar / Avalara) | 2 | 1 | 4 | 4 | 5 | 2 | 4 | 3 | 25 | 50-state tax rules; feature parity (5+ connectors, 46 jurisdictions); crowded (VC-backed) | Out |
| I01 | GiftLedger (RE NXT / Bloomerang) | 3 | 3 | 4 | 4 | 3 | 1 | 3 | 3 | 24 | Crowded with free tools; payments-adjacent | Out |
| J02 | SiteShield (Termly / Osano) | 3 | 2 | 5 | 5 | 2 | 1 | 3 | 3 | 24 | Crowded-cheap; 20-state legal content | Out |
| G05 | AgencyLite (EZLynx / Epic) | 2 | 3 | 3 | 2 | 5 | 3 | 2 | 3 | 23 | Feature parity (IVANS, raters) | Out |
| G07 | BenchBoard (Bullhorn) | 2 | 3 | 3 | 3 | 5 | 2 | 2 | 3 | 23 | SMS/10DLC core; crowded-cheap ATS; parity for temp | Out |
| I04 | DoorList (Eventbrite) | 3 | 2 | 5 | 4 | 3 | 1 | 3 | 2 | 23 | Payment processing core; crowded-cheap | Out |
| I06 | CampFile (CampMinder) | 2 | 2 | 3 | 3 | 5 | 3 | 3 | 2 | 23 | Feature parity; health-data-adjacent; payments | Out |
| J04 | TagTrue (Metrc / Dutchie) | 2 | 2 | 3 | 2 | 5 | 3 | 4 | 2 | 23 | 50-state cannabis rules; gated state API access | Out |
| J05 | CellarPermit (ShipCompliant) | 2 | 1 | 4 | 3 | 5 | 4 | 1 | 3 | 23 | 50-state alcohol rules (permit risk) | Out |
| G01 | LawLedger (Clio / MyCase) | 1 | 2 | 3 | 3 | 5 | 2 | 3 | 3 | 22 | Feature parity; trust-accounting liability | Out |
| G04 | StatePay (Gusto / ADP) | 2 | 2 | 4 | 3 | 3 | 2 | 4 | 2 | 22 | 50-state/city leave rules; payroll money movement (Phase 2); parity | Out |
| I05 | ClubHouse (TeamSnap ONE) | 2 | 2 | 2 | 3 | 5 | 2 | 4 | 2 | 22 | Payments core; committee buyer; parity; SMS | Out |
| J07 | StationLog (ESO / Tyler) | 3 | 3 | 2 | 3 | 3 | 3 | 2 | 3 | 22 | Government/committee buyer; NERIS access unknown | Out |
| G02 | PlainLedger (QBO / Xero) | 1 | 2 | 2 | 3 | 4 | 1 | 4 | 2 | 19 | Feature parity (accounting); crowded-cheap | Out |
| I02 | TitheBox (Pushpay) | 2 | 2 | 2 | 3 | 4 | 1 | 3 | 2 | 19 | Payments core; hardware/offline check-in; committee; crowded; SMS | Out |
| I07 | SchoolPing (ParentSquare) | 2 | 2 | 2 | 3 | 5 | 1 | 2 | 2 | 19 | SMS/voice/10DLC core; committee; crowded-free | Out |

Note on the totals: WTP rewards high-priced B2B verticals, so several killed ideas (G05, J04, J05, I06) still total 23. **Use the kill flags, not the total, to rule ideas in or out.**

#### Scoring rationale (one line per idea)
- **I03:** The CRUD core (members, renewals, events, directory) is easy. The website builder pulls Build down to 3. Liability is low because dues flow through the org's own processor. The buyers (club treasurers, small-association EDs) are card buyers, and Jan 1 dues season plus WildApricot hikes and the Momentive sale give urgency. ARPU is modest ($19–$149). Many cheap rivals exist, so Gap is only 2.
- **G03:** Portal, document requests, e-sign and a kanban board are textbook CRUD and documents. The tax-season window (Oct–Dec) is live now. ARPU is high ($39–$199 per firm vs TaxDome's $800–$1,200 per seat). Gap is weak: the corpus never priced Karbon, Canopy or Financial Cents. In my judgment, pro tax software also bundles client portals (see Gaps). The firm holds SSN-bearing documents, so Reg is 3 and security expectations are high.
- **J06:** Easy CRUD plus AI extraction from certificates. The CE-rules content is the work, but this is a tracker, not a filing, so stakes are lower than in J01 or J05. Individuals buy alone (Self 5), but $29/yr fails WTP, which is why the wedge pivots to team plans.
- **G06:** A compliance kit is document generation plus logs (easy), and ARPU is high ($79–$199). Reg is 2 because marketing-rule AI flags are regulatory judgments and RIAs will send vendor due-diligence questionnaires under Reg S-P's service-provider oversight rule (my inference). The evidence is THIN per the corpus.
- **J03:** The Jan 1 2027 wage, leave and poster changes are a hard date (Urg 5). But $9/location makes WTP 2, and accurate poster and ordinance content across states, counties and cities is ongoing legal-ops labor carrying liability.
- **J01:** High ARPU and a real price shock. But it gives tax determinations (rates, taxability, nexus, return prep) where an error costs customers money, and it needs 5+ commerce connectors. The rivals are VC-funded challengers the corpus itself lists.
- **I01:** Free anchors (Zeffy, Givebutter) and many cheap donor CRMs make Gap 1. Donation forms pull payments into the core. Q4 is when nonprofits are least likely to migrate donor data.
- **J02:** The best distribution in the group (Shopify and WordPress marketplaces). But the file admits price parity with Termly in a cheap, crowded category, and it generates state-specific privacy policies, which carries unauthorized-practice-of-law risk.
- **G05, G07, G01, G02, I06, I05, I02:** Customers won't switch until the incumbent's core is replicated: IVANS carrier downloads (G05), pay/bill and VMS (G07), trust accounting plus billing (G01), the general ledger (G02), health center plus staff app (I06), payments plus rostering (I05), payments plus check-in hardware (I02).
- **I04:** The organizer is a perfect card buyer, but the money flow, chargebacks, refunds and event-day support are core. Ticket Tailor, Humanitix and others are already cheaper than or equal to $0.99/ticket (judgment: Ticket Tailor's per-ticket fee is below $0.99; verify).
- **I07, J07:** The buyer is a school board, diocese or town council. I07 also depends on SMS and voice.
- **J04, J05:** State-by-state rules where an error risks a license or permit. J05 has no dated trigger. J04's hemp buyers may be exiting the market rather than buying software.
- **G04:** Phase 1 is buildable, but it encodes state and city leave-accrual rules. Its end state (payroll) is money movement on a partner whose economics are unknown.

#### Kill-flag watch items the assignment named
- **J-series 50-state legal rules:** J01 (sales-tax rates, taxability, nexus), J04 (cannabis and hemp), J05 (alcohol DtC) and J02 (privacy policies for 20 states) all trip this flag hard. J03 trips it through poster and wage content. J06 trips it only lightly, because a CE tracker that shows citations and leaves reporting to the board carries lower stakes.
- **G-series trust/financial liability:** G01 (IOLTA trust ledgers, "career-ending" per the file) and G02 (general ledger, bank feeds) trip it hard. G04 trips it through tax notices and, later, payroll. G03 and G06 are documentation and workflow tools, so the trust/financial flag does not apply to them.
- **I-series payment handling:** I02, I04 and I05 depend on payment processing at their core (giving, ticketing, dues installments), each with chargeback exposure. I01 and I03 can route money through the org's own Stripe or PayPal account (Connect Standard/OAuth), which avoids holding funds. The flag is partial for them.

### Gaps
- Several "Gap vs cheap indie" scores rest on competitor names that come from my training knowledge, not the corpus, and they need verification: Wave and Zoho Books (G02); Manatal, Loxo and Zoho Recruit (G07); Spond and TeamLinkt (I05); ClassDojo and TalkingPoints (I07); Complianz (J02); Mosey (G04); Luma for free events (I04).
- Only I01, I04 and J06 among these 21 files carry a corpus "Verification (Sep 24 2026)" section. The other 18 rely on unverified first-pass data, including the G03 price tables and the I03 competitor-reported surcharge.
- No market-size figure in the G, I or J files is verified. Most are labeled "Estimate".

---

## Q2. Where does the corpus score (/25) disagree with the solo-developer view, and why?

### Takeaway
The corpus rewards pain, price gap and market size. The solo rubric rewards build scope, low liability, self-serve, reachable channels and room against cheap tools. **The biggest downgrades are I01, I04 and J06**, which the corpus ranks #9, #10 and #5 overall at 20/25: I01 and I04 hit crowded or free competitors and payment handling, and J06's individual price is too low. **The biggest upgrades are G06 and G03.** G06 is on the corpus's "put off" list, but a document and compliance kit sold to owner-operators at $79+/mo fits a solo founder. G03 is a CRUD product with high ARPU and a live window. The corpus's "quick-cash compliance add-ons" (J01, J03, J06) are only partly right: J01 fails the solo screen on liability and competition, and its Oct 1 trigger has already passed.

### Cited Findings
- The corpus scores Pain, Price gap, Build ease, Sales speed and Market size, each 1–5 out of 25. Priority adds 0.1 for each state ranking an idea in its top 3 ([INDEX.md](INDEX.md)).
- INDEX's top 15 includes J06 (#5, 20), I01 (#9, 20) and I04 (#10, 20) ([INDEX.md §1](INDEX.md)).
- INDEX recommends "Quick-cash compliance add-ons, sold on a date": J01 (TaxJar Oct 1 2026), J06 (Delaware Mar 1) and J03 (poster and pay-transparency changes) ([INDEX.md §2](INDEX.md)).
- INDEX's "Ideas to put off (14/25 or below)" includes G05, G06, J04, J05, J07 and I06 ([INDEX.md §5](INDEX.md)).
- INDEX's own pattern note: "The best buyers own the business and pay by card… small nonprofits. Avoid segments that buy through RFPs, like local government (J07)" ([INDEX.md §5](INDEX.md)).
- The corpus's own risk notes support the solo downgrades: I01 says "Free competitors (Zeffy, Givebutter) set a '$0' anchor" ([corpus I01](ideas/I01-nonprofit-donor-crm-blackbaud-bloomerang-givebutter-alternative.md)). I04 says "Crowded field: Ticket Tailor, Humanitix, SimpleTix and TicketSpice" ([corpus I04](ideas/I04-event-ticketing-small-organizers-eventbrite-alternative.md)). J06 says "Low individual willingness to pay" ([corpus J06](ideas/J06-professional-license-ce-tracking-entity-compliance-cebroker-legalzoom-alternative.md)). J01 says "Crowded category (Zamp, Numeral, Kintsugi, TaxCloud and others)" ([corpus J01](ideas/J01-sales-tax-nexus-filing-avalara-taxjar-alternative.md)).
- G06's corpus Pain score of 2 is provisional because of thin evidence. Its Market size of 2 rests on an estimated ~20k small firms ([corpus G06](ideas/G06-ria-crm-compliance-reg-sp-redtail-smarsh-alternative.md)).
- G02's corpus Build ease is 2 and its Market size 5. G01's Build ease is 3 ([_scoreboard.csv](_scoreboard.csv); [corpus G01](ideas/G01-small-law-practice-trust-clio-mycase-alternative.md); [corpus G02](ideas/G02-smb-accounting-quickbooks-online-xero-alternative.md)).

### Inferences

| ID | Corpus /25 (%) | Solo /40 (%) | Direction | Main reason for the gap |
|---|---|---|---|---|
| I01 | 20 (80%) | 24 (60%) | **Solo much lower** | The corpus gives Market size 5 and Build ease 4. The solo screen penalizes free and cheap rivals (Gap 1), payments in the core, and Q4 timing that discourages migration. |
| I04 | 20 (80%) | 23 (58%) | **Solo much lower** | No criterion in the corpus for indie competition or payment-handling burden. Per the file's own verification, the trigger is uncertainty, not a fee hike. |
| J06 | 20 (80%) | 26 (65%) | Solo lower, still shortlisted | Market size 5 counts tens of millions of licensees, but they pay $29/yr. Only a team/agency plan reaches $49+/mo. |
| G01 | 19 (76%) | 22 (55%) | Solo much lower | Corpus Build ease 3 understates feature parity and trust-ledger liability. Solo distribution through state-bar benefit programs is partnership-gated. |
| G02 | 18 (72%) | 19 (48%) | **Solo much lower** | Market size 5 drives the corpus score. For a solo founder, accounting is the textbook parity monster and the low end is full of free or cheap tools (judgment). |
| J01 | 18 (72%) | 25 (63%) | Solo lower and killed | The corpus rewards Pain 4 and Sales speed 4. The solo flags are 50-state tax determinations, connector breadth and VC-funded rivals. The headline Oct 1 date has passed. |
| G04 | 17 (68%) | 22 (55%) | Solo lower and killed | DE and MD rank it top 3 for state hooks, but it carries per-state/city leave rules plus a payroll end state. |
| J02 | 17 (68%) | 24 (60%) | Similar %, but killed | The best channel fit in the group. The corpus itself says it is at price parity in a crowded, cheap category. |
| I05 | 18 (72%) | 22 (55%) | Solo lower | Corpus "Sales speed 4" ignores the board buyer and the payments and minors-data load. |
| I03 | 19 (76%) | 28 (70%) | Agree (top of group) | Both views like card buyers, a dated renewal season and a hated incumbent. The solo view adds low liability. |
| G03 | 18 (72%) | 28 (70%) | Solo relatively higher | The corpus caps Pain at 3 because TaxDome is well rated. For a solo founder, the CRUD build, $39–$199 ARPU and the live Oct–Dec window matter more. |
| G06 | 14 (56%) | 26 (65%) | **Solo higher** | The corpus penalizes thin evidence and a small market (~20k firms). A solo founder needs only ~125 customers at $79/mo for $10k MRR, and the kit is documents plus logs. Validate before building. |
| J03 | 18 (72%) | 26 (65%) | Roughly agree | Both like the dated legal churn. The solo view penalizes $9/location ARPU and content liability. |
| G05, J04, J05, J07, I06 | 14 (56%) | 22–23 (55–58%) | Agree: put off | The solo scores look middling only because WTP is high. The kill flags agree with the corpus's "put off". |
| G07 | 17 (68%) | 23 (58%) | Solo lower | Corpus Build ease 4 understates SMS/10DLC and the ATS parity needs. Cheap ATS rivals were not checked (judgment). |
| I02, I07 | 17 / 15 | 19 / 19 | Solo lower | Several kill flags each: payments, hardware and SMS (I02); SMS/voice and committee buyer (I07). |

- **Structural reason for the disagreements (judgment):** the corpus has no criterion for (a) liability from encoding rules, (b) cheap indie competition, or (c) support load. Its "Market size" criterion also rewards huge but low-ARPU or hard-to-reach pools. For a solo founder, ARPU times reachable customers matters more than total addressable market.
- State "Priority" boosts G04, J01, J02, J03 and J06 through state hooks. For a product sold online nationally, state rankings matter mainly as content and SEO angles, not launch geography.

### Gaps
- The corpus scored only once, and only 3 of these 21 files were fact-checked. Corpus sub-scores for unverified files (G03, G06, I03, J03) could move once prices are checked.
- No conversion, CAC or search-volume data exists in the corpus for any of these ideas, so the "Dist" scores are judgment.

---

## Q3. For the best 3–5, what is the narrowest sellable wedge, and which claims most need fresh verification?

### Takeaway
**Build in this order: (1) I03, a "WildApricot escape" for small associations, chambers and clubs; (2) G03, a document-collection portal plus WISP generator for solo and small tax firms, which must be live by about Nov 15 to catch the 2027 season; (3) J06, a staff license and CE expiry tracker sold to small Florida healthcare employers, not to individuals.** G06 (a Reg S-P incident-response and vendor-oversight kit for small RIAs) and J03 (a pay-transparency job-ad checker for recruiters and staffing agencies) are validate-first options. Before any build, the most important things to verify are: WildApricot's current pricing and surcharge plus the cheap membership tools; whether pro tax software already bundles free client portals; CE Broker's paid prices and free alternatives such as Nursys e-Notify; and the Reg S-P small-entity date.

### Cited Findings
- I03's corpus pricing: $19/mo (≤250 members), $39 (≤1,000), $79 (≤5,000), $149 unlimited. The corpus example has a 500-contact club moving from ~$1,663/yr to $468/yr ([corpus I03](ideas/I03-membership-associations-chambers-wild-apricot-alternative.md)).
- WildApricot's risks per the corpus: many orgs run their public site on it, so the import must cover pages and menus, and autopay tokens must be re-collected at first renewal ([corpus I03](ideas/I03-membership-associations-chambers-wild-apricot-alternative.md)).
- I03's corpus timing: "Oct–Nov before Jan 1 renewals; July for fiscal-year associations" ([corpus I03](ideas/I03-membership-associations-chambers-wild-apricot-alternative.md)).
- G03's corpus pricing: Solo $39/mo, Firm $99/mo (≤5 users), Plus $199/mo (≤15), with seasonal users free. The corpus example has a 4-person TaxDome Pro firm at $4,500/yr moving to $1,188/yr ([corpus G03](ideas/G03-cpa-tax-practice-portal-taxdome-karbon-alternative.md)).
- G03's corpus timing: "Nobody switches Feb–Apr… sell Oct–Dec and May–Jul", with a "Live before Jan 15" onboarding push and a free WISP generator as the lead magnet ([corpus G03](ideas/G03-cpa-tax-practice-portal-taxdome-karbon-alternative.md)).
- G03's channels: r/taxpros, TaxProTalk, EA and tax-practice Facebook groups, NAEA, NATP and state CPA societies ([corpus G03](ideas/G03-cpa-tax-practice-portal-taxdome-karbon-alternative.md)).
- J06's corpus team plan is $4 per licensed staff member per month, aimed at "clinics, agencies and brokerages", and it overlaps with the E07 (home care) buyer list ([corpus J06](ideas/J06-professional-license-ce-tracking-entity-compliance-cebroker-legalzoom-alternative.md)).
- CE Broker's paid-tier prices are unverified because cebroker.com/pricing returned 404 on Sep 24 2026 ([corpus J06 Verification](ideas/J06-professional-license-ce-tracking-entity-compliance-cebroker-legalzoom-alternative.md)).
- Florida checks CE through CE Broker at renewal for 200+ health license types ([FL HealthSource via FL state file](https://www.flhealthsource.gov/)).
- G06's corpus pricing is Solo $79/mo and Team $199/mo. The corpus recommends "Validate demand with 15 RIA interviews before building" ([corpus G06](ideas/G06-ria-crm-compliance-reg-sp-redtail-smarsh-alternative.md)).
- J03's corpus MVP includes a "pay-transparency job-ad checker" (paste box or Chrome extension) covering CA, CO, WA, NY, NJ, IL, MN, MA, VT, MD and DE. Its go-to-market includes "cold email to recruiters posting non-compliant ads in MA, NJ and VT (the ads are public)" ([corpus J03](ideas/J03-smb-employment-law-posters-pay-transparency-poster-guard-mineral-alternative.md)).
- Corpus "(verify)" markers relevant to the shortlist:
  - G03: Karbon, Canopy, Financial Cents and Liscio prices; the WISP requirement ("background, verify").
  - G06: the Reg S-P small-entity date (about Jun 3 2026).
  - J03: CT sick leave reaching 1+ employee on Jan 1 2027; local pay-transparency ordinances.
  - J06: the date of the Delaware LLC tax increase.
  - I03: the 20% surcharge, which is competitor-reported.
  - ([corpus files as above](ideas/); [INDEX §3](INDEX.md))

### Inferences

#### Shortlist #1: I03 DuesDesk, narrowed to a "WildApricot escape kit" (judgment)
- **Ships in 4–6 weeks:**
  - A WildApricot importer (CSV export, plus the WildApricot API if it is available) covering contacts, membership levels, renewal dates and event history.
  - A member database with levels and custom fields.
  - Automated dues-renewal reminders with payment links and autopay through **the org's own Stripe account** (Connect Standard), plus "mark paid by check".
  - Member self-service profiles.
  - An **embeddable** public member and business directory and an events widget for the org's existing WordPress or Squarespace site.
  - Simple event registration with member and non-member prices.
  - Segment email sent through a transactional provider.
- **Explicitly excluded:**
  - The website builder (the biggest scope risk in the corpus MVP).
  - The newsletter block editor.
  - The chamber sponsorship pack and multi-chapter mode.
  - SMS (no 10DLC).
- **Buyer:** volunteer presidents and treasurers of clubs and alumni groups, and EDs of 1–5 staff associations, currently on WildApricot with 100–2,000 contacts. Chambers come second, because they need the business directory and board sign-off.
- **Price:** I would set it slightly above the corpus: $29/mo (≤250), $49 (≤1,000) and $99 (≤5,000), month to month. That is still well below the competitor-reported WildApricot prices of ~$74/mo for 250 contacts and ~$139/mo for 500. At a blended ~$45 ARPU, about 220 customers give $10k MRR.
- **Channel:**
  - "WildApricot alternative / price increase / surcharge" SEO pages.
  - Replies on the WildApricot wishlist forum thread asking for a ~$25 plan.
  - Club-admin Facebook groups (running, pickleball) and r/nonprofit.
  - Lead magnet: "upload your WildApricot export, see your dashboard in 5 minutes".
- **Window:** Oct–Nov 2026 for Jan 1 renewals. The second window is May–Jun for Jul 1 fiscal-year associations.
- **Wedge re-score:** Build 4, Reg 4, Self 4, Dist 4, WTP 3, Gap 2, Urg 4, Supp 4 = **29/40**. The partial crowded flag remains: the wedge must win on import quality and the no-surcharge message, not on features.

#### Shortlist #2: G03 SeasonDesk, narrowed to a document-collection portal plus WISP generator (judgment)
- **Ships in 4–6 weeks:**
  - A magic-link client portal with phone photo-to-PDF upload.
  - Per-client document checklists, created from a CSV of last year's list or manually.
  - AI that labels uploads and ticks off checklist items.
  - Automated **email** chasers. SMS is deferred to avoid 10DLC.
  - Engagement letters with simple e-sign and an audit trail.
  - A status board.
  - A free **WISP generator** as the lead magnet.
- **Explicitly excluded:** 8879/KBA signatures, CRM, time tracking, integrations with QBO or the tax software, and Stripe pay-before-release (that is V1.5).
- **Data-custody option to cut liability:** let uploads land in the firm's own Google Drive, Dropbox or OneDrive folder, so the product doesn't become a long-term store of SSN-bearing documents.
- **Buyer:** owners of solo to 5-person EA, CPA and preparer shops that today use email and Dropbox, or that find TaxDome Essentials ($800/yr) or Pro ($1,000/seat/yr) too expensive.
- **Price:** the corpus's $39/mo solo and $99/mo for up to 5 users, with seasonal staff free and an annual option. At a ~$60 blend, about 170 customers give $10k MRR.
- **Channel:** r/taxpros, TaxProTalk, EA and NATP Facebook groups, NAEA chapter webinars, and SEO for the free WISP template.
- **Hard timing constraint:** launch by about Nov 15 2026 so firms can onboard clients before mid-January. Miss it, and the next window is May–Jul 2027.
- **Wedge re-score:** Build 5, Reg 3, Self 4, Dist 4, WTP 4, Gap 2, Urg 4, Supp 3 = **29/40**.

#### Shortlist #3: J06 LicenseLedger, narrowed to a staff license and CE expiry tracker for small Florida healthcare employers (judgment)
- **Ships in 4–6 weeks:**
  - A license wallet per staff member (state, board, number, expiry).
  - AI certificate capture by email forward or photo.
  - CE-hours tracking for 3–5 high-volume Florida professions (e.g. RN/LPN, PT/PTA, dental hygienist), with each board rule cited.
  - A manager dashboard showing who expires in 120/60/30 days.
  - Reminders to staff and managers.
  - A one-click audit export (PDF plus the certificate bundle).
  - A free individual tier with an unlimited transcript export, as the funnel (the anti-CE-Broker hook).
- **Explicitly excluded:** automated board lookups, submission to CE Broker, entity filing and registered-agent services.
- **Buyer:** administrators, compliance coordinators or directors of nursing at Florida home-health agencies, nurse-staffing agencies, and therapy or dental group practices.
- **Price:** $49/mo up to 25 licensees and $99/mo up to 100. That replaces the corpus's $4/staff and the unviable $29/yr individual plan.
- **Channel:**
  - Cold email to licensed-facility lists (whether Florida publishes such lists is unverified).
  - The free individual tier promoted in r/nursing and r/TravelNursing.
  - "CE Broker alternative / transcript without upgrade" SEO.
- **Optional add-on (same build, different buyer):** a free entity due-date calendar for bookkeepers and CPAs covering DE Mar 1, CA Apr 15 and FL May 1. It doubles as a cross-sell to G03's tax-firm buyers.
- **Wedge re-score:** Build 4, Reg 3, Self 4, Dist 3, WTP 4, Gap 3, Urg 3, Supp 4 = **28/40**.
- **Caveat:** the paid team buyer is my inference. The corpus evidence (CE Broker anger) comes from individual licensees. Validate with about 10 calls to Florida agency administrators before building.

#### Conditional #4: G06 AdvisorVault, narrowed to a Reg S-P incident-response and vendor-oversight kit (validate first)
- **Ships in about 4 weeks:**
  - A questionnaire that produces a firm-specific written incident-response program.
  - A service-provider inventory with an annual attestation log.
  - A breach triage workflow with a 30-day notice clock and notice templates.
  - An annual-review checklist with evidence uploads and a CCO sign-off PDF.
- **Excluded:** CRM, archiving, AI marketing-rule review and custodian integrations.
- **Buyer:** founder/CCOs of 1–10 person RIAs. **Price:** $79/mo or $790/yr.
- **Channel:** XYPN, Kitces community, r/CFP, NAPFA, and SEO for "Reg S-P incident response plan template RIA".
- **Wedge re-score:** about 28/40.
- **Gate:** run the corpus's 15 interviews first, and confirm the small-entity compliance date and current competitors.

#### Conditional #5: J03 PostedUp, narrowed to a pay-transparency job-ad checker (validate first)
- **Ships in 3–4 weeks:**
  - A paste box and Chrome extension for Indeed, LinkedIn and ZipRecruiter posting screens.
  - A rule set limited to the ~11 states in the corpus plus a few named cities, each rule cited.
  - Flags for a missing range, missing benefits language and remote-role triggers.
  - A suggested compliant rewrite.
  - A timestamped check log to keep as evidence.
- **Excluded:** posters, wage calendars and the scam-letter checker. These carry the unbounded content liability.
- **Buyer:** staffing-agency owners and multi-state in-house recruiters. **Price:** $29/mo per recruiter or $99/mo per agency.
- **Channel:** Chrome Web Store, r/recruiting, LinkedIn recruiter groups, and the corpus's idea of cold-emailing public non-compliant ads.
- **Wedge re-score:** about 27/40, with urgency only 2 because no pay-transparency deadline falls between Oct 2026 and Apr 2027 (DE is Sep 26 2027).

#### Why I03 ranks above G03 (judgment)
I03's timing is more forgiving: it has two renewal seasons a year, continuing WildApricot hikes and a recent PE sale, and a slip of a few weeks still catches Jan 1 renewals. G03 has better ARPU but a hard Nov–Dec launch deadline and, probably, denser competition. If the founder can ship in under 5 weeks, G03 could go first for faster cash.

#### Verification asks for the later web round, by shortlist item
1. **I03:**
   - WildApricot's current tier prices, any 2027 change, and whether the "20% surcharge" for outside processors is real and current (it is competitor-sourced).
   - What the WildApricot API and export allow.
   - The Momentive/Personify roadmap for WildApricot.
   - Re-check the 1.3/5 Trustpilot rating.
   - Search volume for "WildApricot alternative".
   - **Cheap-competitor sweep** (names from my judgment, the corpus lists only the first three): MembershipWorks, Groupable, Memberplanet, ClubExpress, Join It, Zeffy memberships, Membership Toolkit, Raklet, Glue Up, Novi AMS and Wix/Squarespace member areas.
2. **G03:**
   - TaxDome's 2026–27 prices.
   - Karbon, Canopy, Financial Cents, Liscio, Content Snare and SmartVault prices (a corpus gap).
   - **Whether Drake, ProSeries/Lacerte and UltraTax bundle client portals** (e.g., Drake Portals, Intuit Link, TaxCaddy; judgment). That would be the biggest threat to the wedge.
   - The IRS/FTC Safeguards WISP requirement, whether the IRS's free WISP template (I believe IRS Publication 5708) undercuts the lead magnet, and whether PTIN renewal asks about a WISP (judgment; verify).
   - The 2027 filing-season opening date.
   - r/taxpros rules on vendor posts.
3. **J06:**
   - CE Broker's paid-tier prices (the page 404'd).
   - The Florida professions and renewal cohorts that fall due Oct 2026–Apr 2027, to time campaigns.
   - **Nursys e-Notify** (I believe it gives nurses and employers free license-expiry alerts; judgment), ExpirationReminder-style generic trackers, and healthcare credentialing tools (Credentially, Kamana, Medallion, Verifiable) with their pricing.
   - Whether Florida publishes home-health and agency licensee lists suitable for cold email.
   - Delaware's $400 LLC tax and Mar 1 2027 franchise-tax details.
4. **G06:**
   - The Reg S-P small-entity compliance date and any SEC delay.
   - Competitors and prices (judgment names: COMPLY, formerly RIA in a Box; Hadrius; Saifr; MarketCounsel).
   - 2025–26 complaint evidence for Redtail and Wealthbox.
   - XYPN's size and vendor terms.
5. **J03:**
   - The current list of pay-transparency states and cities with effective dates (city ordinances are marked "not verified" in the corpus).
   - Existing free or cheap job-ad checkers and ATS features that already flag missing ranges.
   - The Jan 1 2027 changes (CT sick leave at 1+ employees, MI $15 minimum wage, MA PFML).
   - Whether WA's 5-day cure has reduced lawsuit fear.

### Gaps
- None of the shortlisted wedges has direct evidence of willingness to pay for the narrowed scope. The corpus prices are for the broader MVPs.
- The corpus does not say whether the WildApricot API allows bulk export, whether NERIS has a free portal (J07, not shortlisted), or whether Florida licensee data is accessible.
- G03's competitor density is the largest unknown. The corpus says outright that the Karbon, Canopy and pro-tax-software price checks are a gap.
- Search-volume, CPC and marketplace-install data were not collected for any idea.

---

## Q4. Which switching-window dates have already passed as of Oct 10 2026, and which are still ahead?

### Takeaway
**TaxJar's Oct 1 2026 month-to-month repricing and Xero's Oct 1 2026 hike have both passed.** J01 can now chase only annual TaxJar renewals, which run through late Feb 2027. Several other headline triggers are also history: FL's Sunbiz dissolution (Sep 25), FinCEN's BOI final rule (Aug 11), the Reg S-P small-entity date (about Jun 3), NFIRS retirement (Jan 31), IN/KY/RI privacy laws (Jan 1), Eventbrite's sale (Mar 10) and Personify's sale (Jan 6). **Live windows for the shortlist:** the tax pre-season (now through about mid-Jan 2027, G03), Jan 1 dues renewals (I03), the Jan 1 2027 employment-law changes (J03), Delaware's franchise tax on Mar 1 2027 (J06) and California's franchise tax on Apr 15 2027 (J06). Year-end giving (Oct–Dec, Giving Tuesday Dec 1 2026) is still running, but it argues against nonprofits migrating donor systems until January.

### Cited Findings
- TaxJar month-to-month customers moved on **Oct 1 2026**. Annual customers move at renewal "from mid-2026 through late February 2027" ([TaxCloud via J01](https://taxcloud.com/blog/taxjar-price-increase-2026/)).
- The Illinois Remote Retailer Tax Amnesty ends Oct 31 2026, and Minnesota Paid Leave premiums are due then too ([INDEX §3](INDEX.md)).
- Xero US rose on Oct 1 2026, and the QBO list increase took effect Aug 1 2026 at renewal ([Booksla via G02](https://www.booksla.com/xero-price-increase/); [SWK via G02](https://www.swktech.com/2026-quickbooks-price-increases-what-they-mean-for-your-renewal/)).
- Florida's Sunbiz dissolved unfiled entities on Sep 25 2026, and the next annual report is due May 1 2027 ([FL state file](states/FL-florida.md); [FL Division of Corporations via FL state file](https://dos.fl.gov/sunbiz/manage-business/efile/annual-report/)).
- FinCEN's BOI final rule came on Aug 11 2026, effective Aug 14 2026 ([FinCEN via J06](https://www.fincen.gov/boi)).
- The Reg S-P smaller-entity compliance date is about Jun 3 2026 ("verify") ([corpus G06](ideas/G06-ria-crm-compliance-reg-sp-redtail-smarsh-alternative.md)).
- NFIRS's final date was Jan 31 2026 ([USFA via J07](https://www.usfa.fema.gov/nfirs/)).
- Indiana, Kentucky and Rhode Island privacy laws took effect Jan 1 2026 ([MultiState via J02](https://www.multistate.us/insider/2026/2/4/all-of-the-comprehensive-privacy-laws-that-take-effect-in-2026)).
- Kentucky dropped its 200-transaction test on Aug 1 2026 and Illinois on Jan 1 2026 ([Avalara blog via J01](https://www.avalara.com/blog/en/north-america/2025/06/states-eliminating-economic-nexus-transaction-thresholds.html)).
- The Eventbrite sale closed Mar 10 2026 ([Equaticket via I04](https://equaticket.com/blog/eventbrite-bending-spoons-what-organizers-need-to-know)), and Momentive acquired Personify on Jan 6 2026 ([SmartThoughts via I03](https://www.smartthoughts.net/post/momentive-personify-acquisition-association-impact)).
- Gusto's hike took effect Mar 2026 ([HRPayPick via G04](https://hrpaypick.com/gusto-pricing/)), and the Givebutter class action was filed Apr 2026 ([TINA.org via I01](https://truthinadvertising.org/articles/givebutters-hidden-fees/)).
- Poster Guard lists five mandatory poster changes in Sep 2026 ([posterguard.com via J03](https://www.posterguard.com/)).
- Still ahead:
  - The federal hemp cap, about Nov 12 2026 (verify) ([corpus J04](ideas/J04-cannabis-hemp-compliance-metrc-reconciliation-dutchie-alternative.md)).
  - Giving Tuesday, Dec 1 2026 ([corpus I01](ideas/I01-nonprofit-donor-crm-blackbaud-bloomerang-givebutter-alternative.md)).
  - Jan 1 2027: the payroll switch date, Maryland FAMLI contributions, Michigan's $15 minimum wage, the Massachusetts PFML change and Connecticut sick leave at 1+ employees (verify) ([INDEX §3](INDEX.md)).
  - Delaware franchise tax and annual report, Mar 1 2027 ([DE state file](states/DE-delaware.md)).
  - California's $800 minimum franchise tax, Apr 15 (verify) ([CA state file](states/CA-california.md)).
  - Spring youth-sports registration opens Nov–Jan ([corpus I05](ideas/I05-youth-sports-clubs-leagues-teamsnap-sportsengine-alternative.md)).
  - The camp window, Sep–Dec ([corpus I06](ideas/I06-summer-camps-after-school-campminder-ultracamp-alternative.md)).
  - Delaware pay transparency, Sep 26 2027, outside the 6-month window ([Hunton via J03](https://www.hunton.com/hunton-retail-law-resource/several-states-enact-pay-transparency-laws-what-employers-need-to-know-in-2026)).

### Inferences

| Trigger | Date | Ideas | Status on 2026-10-10 | Implication for a solo founder |
|---|---|---|---|---|
| TaxJar month-to-month repricing | Oct 1 2026 | J01 | **Passed** (9 days ago) | Month-to-month churners have already decided. Only annual renewals through Feb 2027 remain. |
| Xero US hike | Oct 1 2026 | G02 | **Passed** | Small hike with sweeteners. The corpus already calls Xero users a weak target. |
| QBO renewal hike | Aug 1 2026 (at renewal) | G02 | Rolling | Not actionable for a solo founder (G02 is killed). |
| Sunbiz administrative dissolution | Sep 25 2026 | J06 | **Passed** | Possible "reinstatement rescue" content. Next hard date: May 1 2027. |
| FinCEN BOI domestic exemption | Aug 11 2026 | J06 | **Passed** | A content hook ("stop paying for BOI"), not a buying deadline. |
| Reg S-P small-entity compliance | ~Jun 3 2026 (verify) | G06 | **Passed** | The pitch becomes "you're exposed in exams now", which works but is weaker than a deadline. |
| NFIRS retired | Jan 31 2026 | J07 | **Passed** | Departments have probably chosen a NERIS path already, which weakens J07 further. |
| IN/KY/RI privacy laws | Jan 1 2026 | J02 | **Passed** | Watch for newly enacted laws with 2027 dates (corpus: AL, LA, OK, VT, unverified). |
| KY drops 200-transaction test | Aug 1 2026 | J01 | **Passed** | An explainer-content hook only. |
| Eventbrite and Personify sales | Mar 10 / Jan 6 2026 | I04 / I03 | **Passed** | Post-deal repricing risk continues. For I03, the corpus cites an 18–36 month rationalization horizon. |
| IL Remote Retailer Amnesty ends | Oct 31 2026 | J01 | 21 days left | Too soon for a new product to ship. |
| Federal hemp cap | ~Nov 12 2026 (verify) | J04 | About a month left | Too soon. The buyers may be exiting the market. |
| Tax pre-season | Oct–mid-Jan | G03 | **Live, closing** | Ship by about Nov 15 or wait until May. |
| Year-end giving / Giving Tuesday | Oct–Dec; Dec 1 2026 | I01, I02 | Live | Peak-season risk: nonprofits and churches avoid migrating mid-campaign. The realistic switch is January (statements pain). |
| Jan 1 dues renewal | Jan 1 2027 (sell Oct–Nov) | I03 | **Live** | The best-fitting live window for the #1 pick. |
| Jan 1 2027 employment-law changes | Jan 1 2027 | J03, G04 | Live | A strong date for poster and wage alerts, but those carry content liability. The job-ad checker doesn't depend on it. |
| Spring youth registration; camp window | Nov–Jan; Sep–Dec | I05, I06 | Live and partly elapsed | Both ideas are killed anyway. |
| Delaware franchise tax; CA franchise tax | Mar 1 2027; Apr 15 2027 | J06 | Ahead | Good timing for the J06 entity-calendar add-on campaigns (Jan–Apr). |

### Gaps
- The hemp effective date, CT sick-leave expansion, MI minimum-wage step, Reg S-P small-entity date and CA franchise-tax due date are all corpus "(verify)" items. None was checked in this pass.
- Whether TaxJar, WildApricot, TaxDome or CE Broker announced further price changes after Sep 25 2026 is unknown, because no web access was allowed in this pass.
