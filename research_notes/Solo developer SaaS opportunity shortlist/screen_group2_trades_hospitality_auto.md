# Screen group 2: trades, hospitality and auto/fleet ideas (C01–C07, D01–D09, K01–K06) re-scored for a solo, Claude-assisted developer

Scope and method. I read all 22 assigned idea files in full, plus INDEX.md sections 1–5 and 8, the corpus scoring rubric, `_scoreboard.csv`, `_states_summary.csv` and the state files that rank these ideas. The corpus was written Sep 24–25 2026, and today is Oct 10 2026. I did no web searches. Every score below is my judgment, made by applying the solo-developer rubric ([RUBRIC]) to the evidence in the corpus. Links are reference-style, and the definitions are at the end of the file. Most point to corpus files, and those files cite the original URLs (I give the original URL where it carries weight). Statements marked "(judgment)" come from my own reasoning or general knowledge and are not backed by the corpus.

## Key question 1: What are the 8 rubric scores (/40) and kill flags for each idea, and what evidence supports them?

### Takeaway
As the corpus wrote them, only two ideas reach 29/40: **K02 DealJacket** (California CARS Act deal compliance) and **K03 HaulDesk** (small-fleet back office plus IFTA). K02 is the only idea in the group with no full kill flag. Ten of the 22 carry two or more full kill flags. None of the nine hospitality ideas (D01–D09) survives: each is a payments-core, hardware, real-time or feature-parity product, or sits in a crowded cheap market. C05 (CoConstruct exodus), C03 (NY pesticide reporting) and C07 (restoration supplements) are viable only when cut down to a narrow wedge (see Key question 3).

### Cited Findings
**C01 FlatRate (HVAC/plumbing/electrical field service)**
- Third-party estimates put ServiceTitan at about $245–$500 per tech per month, with $5k–$15k onboarding and contracts of at least 12 months. Reviewers describe early-exit bills of about $22k and $37k (Trustpilot, Jun–Jul 2026) — [C01]
- Housecall Pro runs from Basic at $79/mo to Max at $329/mo. Jobber Core is $49/mo month to month. One HCP bill went from $351 to $681 without notice (Trustpilot, Sep 15 2026) — [C01] (prices checked Sep 24 2026 at https://www.housecallpro.com/pricing/ and https://www.getjobber.com/pricing/)
- The corpus's own MVP list is a full field-service suite. It includes a "mobile tech app that works offline", a dispatch board, Stripe payments, membership auto-billing, two-way QuickBooks Online sync and importers from three systems. The file concedes: "Crowded category. FieldEdge, Workiz and many cheap FSMs already exist" — [C01]
- Corpus score 19/25 (Pain 5, Build ease 2, Market 5). It ranks in the top 3 in 5 states (ME, ND, OH, TX, WI) — [C01], [STATES]

**C02 StormDesk (roofing/storm CRM)**
- AccuLynx is estimated at $350–$450/mo for 1–3 users and $900–$1,400/mo for 5–10 users. JobNimbus is quote-only. Roofr offers a free Starter plan, then $109, $249 and $349/mo, with no per-seat fees — [C02]
- The corpus admits "Roofr already has flat pricing, cheap reports and a free tier" — [C02]
- The trigger is storm events plus the Oct–Feb off-season. There is no dated deadline — [C02]. Colorado roofing contract rules (C.R.S. 6-22) are marked "verify" — [CO]
- Corpus score 17/25. It ranks in the top 3 in KS, LA, NE and OK — [STATES]

**C03 SprayLog (pest/lawn route software plus NY pesticide reporting)**
- New York commercial applicators file an annual pesticide report. Each record needs the EPA registration number, product, quantity, date and full address with a 5-digit ZIP (NYSDEC OGC 3) — [C03]. The NY state file marks the **Feb 1** due date "(verify)" because the DEC page does not state it. It also confirms against DEC that the Birds and Bees Act neonic ban expands to imidacloprid, thiamethoxam and acetamiprid from **Dec 31 2026** — [NY]
- A pest operator on Jobber complains that it has no chemical tracking (Trustpilot, Aug 25 2026). GorillaDesk costs $49, $99 or $149/mo. A FieldRoutes customer had to pay out a full 3-year agreement — [C03]
- The MVP as written is a full route field-service product: offline mobile tickets, route optimization, autopay, five importers and QuickBooks sync — [C03]
- Corpus score 18/25. The NY state file ranks it #7 in New York — [NY]

**C04 RouteBook (pool and cleaning routes)**
- Skimmer charges $1 per location (minimum $49) or $2 per location (minimum $98). Pool Brain is $50 plus $65 per tech. ZenMaid is $19–$49 plus $4–$24 per cleaner — [C04]
- The corpus says "Complaints in this segment are milder and mostly secondhand; the incumbents are already cheap", calls the urgency "Weak", and names "Many cheap competitors" as the main customer-acquisition risk — [C04]
- Corpus score 16/25 (Pain 2, Build ease 5) — [C04]

**C05 FlatBuild (remodeler/small-GC project management; CoConstruct exodus)**
- CoConstruct: "Projects can still be added through March 31, 2027", and historical data stays viewable. The corpus verified this on Sep 24 2026 — [C05] (https://www.coconstruct.com/migration)
- Buildertrend runs from the mid-$300s to $1,000+/mo, priced by revenue bracket. JobTread is $199/mo plus $20 per internal user. Both were verified — [C05]
- "Competitors are already running the same play. JobTread and Projul target CoConstruct users", and they are "already ranking" for CoConstruct search terms. Also: "CoConstruct exports are limited, so part of the import is manual" — [C05]
- The MVP is a full project-management suite: importer, estimate-to-proposal-to-invoice flow, selections, change orders, client portal, Gantt schedule, job costing with QuickBooks Online sync, and full export — [C05]
- Corpus score 20/25, #4 by Priority. It ranks in the top 3 in CA and ID — [INDEX], [STATES]. The California file pairs it with the LA fire-rebuild deposit cap ($1,000 or 10%) — [CA]

**C06 LienClock (lien deadlines, notices, waivers)**
- Levelset's SendNotice is $59 per recipient. A competitor lists notices at $19 after 3 free, a notice of intent at $49 and a lien filing at $349 — [C06]
- Levelset is rated 4.3/5 on 3,839 Trustpilot reviews, so the file calls the pain "moderate" — [C06]
- The corpus's own Sep 24 fact-check found **four errors in its 8-state rules table**: Texas enforcement, the NY preliminary notice, Colorado notice-of-intent timing and the Colorado enforcement trigger. The FL, CA, WA and GA rows were left unchecked — [C06]
- Its own risk section: "Wrong deadlines create liability... E&O insurance... Unauthorized practice of law" — [C06]

**C07 ClaimKit (restoration documentation plus AI supplements)**
- Xactimate Pro costs $350 for 1 month up to $2,690 for 12 months (Fervor Studio, verified Aug 7 2026). CompanyCam is Core $63/mo, Crew $129/mo for 3 users, plus $29 per extra user — [C07]
- The figure that carriers decline O&P "about 85% of the time" comes from **one** Software Advice reviewer and is not a market statistic — [C07]
- "Several states restrict contractors from acting as public adjusters... supplement-writing must stay documentation, not negotiation" — [C07]. Louisiana's Fortify Homes Program rules ban public adjusting — [LA]
- Corpus score 17/25. It is #1 in Louisiana — [LA]

**D01 FlatTab POS (counter-service restaurants)**
- Toast plans are $0 or $69/mo plus 2.49–3.69% processing, and hardware costs $409–$1,899. Clover equipment runs on 36-month terms at $179–$354/mo — [D01]
- The corpus says "Square is cheap and good... Our edge over Square... is weak". Offline mode is deferred to V2, even though "Restaurants cannot go down on a Friday night" — [D01]

**D02 DirectPlate (direct online ordering)**
- Owner.com is $249/mo plus 5%, or $499/mo flat. ChowNow is $119–$328/mo plus 2.95% + $0.29 per order — [D02]
- The file names eight competitors (Owner, ChowNow, Sauce, Menufy, BentoBox, Slice, Square Online, Toast Online Ordering) and says "The moat is weak". Its complaint evidence is "mostly from competitor comparison pages" — [D02]
- The main trigger, the NYC fee-cap settlement, dates from June 2025 — [D02]

**D03 TableKeep (reservations/waitlist)**
- OpenTable charges $149/mo plus $1.50 per network cover (or $49 flat), $299 for Core and $499 for Pro. A 2% fee on deposits started in Jan 2026. The Resy–Tock merger is dated "summer 2026" by Eat App, and its timeline is unconfirmed — [D03]
- The MVP depends on an SMS waitlist, an iPad host stand and Stripe deposits and no-show fees. OpenTable's diner network is a moat. No first-hand Reddit or Trustpilot threads were pulled — [D03]

**D04 ShiftTip (scheduling plus tip pooling)**
- 7shifts has a free Comp plan (up to 15 employees), then $44.99, $89.99 and $149.99. Homebase has a free Basic plan, then $30, $70 and $120. ShiftTip is priced at $39 per location — [D04]
- "No tax on tips" employer reporting is "Not re-verified via web in this pass". The file names "Wage-and-hour liability" as a risk — [D04]
- It ranks in the top 3 in CT, DC, HI, IL and MI — [STATES]

**D05 InnDesk (independent hotel PMS)**
- Cloudbeds is about $15 per room per month. Little Hotelier is $39/mo plus a 1% booking fee. The file says "Channel manager certification... is the hardest part" and lists "Overbooking liability" as a risk — [D05]
- The INDEX lists it under "ideas to put off" — [INDEX]

**D06 SiteLoop (campgrounds/RV parks)**
- Campspot charges a subscription plus a booking fee paid by the guest, and the amounts are not public. It is rated 4.5/5 on 90 Capterra reviews — [D06]
- The MVP includes map booking, seasonal and metered-electric billing, a front desk, Stripe payments and a camp-store POS. On rural connectivity it says "Offline-tolerant PWA (V2)" — [D06]

**D07 BookTrail (tours and activities)**
- FareHarbor adds a 6% fee to the guest's checkout and charges the operator nothing. Peek has no base fee, Rezdy starts at $99/mo, and Roverd charges 5% — [D07]
- The corpus says: "FareHarbor is 'free' to operators... It's hard to sell a subscription against $0" — [D07]
- Corpus score 19/25, #12 by Priority. It ranks in the top 3 in 7 states (AK, CO, HI, KY, MA, SC, SD) — [INDEX], [STATES]

**D08 TeeFree (golf tee sheet)**
- The ~$94,500/yr cost of GolfNow barter is an estimate by a competitor (TeeAhead). foreUP is about $400–$800/mo and Lightspeed Golf about $300–$700/mo. TeeAhead is free for year one, then $349/mo. There are about 14,000 US golf facilities (not re-verified). Municipal courses buy through RFPs — [D08]

**D09 ShelfPOS (independent retail POS)**
- Clover retail equipment runs on 36-month terms. One retailer got a $930 invoice for declining Lightspeed's card processing. The corpus says "Square and Shopify POS are strong and cheap", and the hardware needs driver support — [D09]

**K01 BayBook (independent auto repair)**
- Tekmetric is $199/mo for Start, $349 for Grow (the first tier with a labor guide) and $439 for Scale (the first with two-way texting). Marketing adds $345/mo. Cheap rivals: ARI $39.99, AutoRepair Cloud $49.99, Torque360 $99.99 (from a competitor's blog) — [K01]
- "We found no hard legal deadline". Labor-guide data (MOTOR/ALLDATA) has to be licensed — [K01]

**K02 DealJacket (California CARS Act deal compliance)**
- SB 766 took effect **Oct 1 2026**. It creates a 3-day cancellation right on used vehicles priced at $50,000 or less. The buyer may drive at most 400 miles, the restocking fee is 1.5% bounded at $200–$600, and the refund is due within 48 hours. It also requires a total price in ads and precontract disclosures on cash and lease deals. Records must be kept 2 years, alongside the DMV's 3 years and 7+ years under finance rules — [K02] (citing the CA Dealer Academy guide and the bill text at https://leginfo.legislature.ca.gov/faces/billNavClient.xhtml?bill_id=202520260SB766)
- DealerCenter is $99/mo flat. Frazer is $129/mo for desktop or $199/mo hosted — [K02]
- "CA dealer licenses are public records", so the DMV Occupational Licensing list can be used for outreach — [K02]
- The file's own risk: "DMS vendors may ship CARS Act features for free". ComplyAuto and ProMax already sell CARS Act help, at prices not captured — [K02]
- Corpus score 17/25 (Price gap 2, Market 3, Sales speed 5). The California file ranks it #4 in CA — [K02], [CA]

**K03 HaulDesk (small-fleet back office plus IFTA)**
- IFTA returns are due quarterly on the last day of the month after each quarter (Oct 31, Jan 31, Apr 30, Jul 31). The Q3 2026 return is due **Oct 31 2026** — [K03]
- DAT plans cost $59–$339/mo, and renewals have risen 25–45% (Small Fleet HQ, Sep 10 2026) — [K03]
- Samsara has 90 BBB complaints in 3 years. They include an auto-renewal for three more years (Jan 2026) and billing that continued for two years after a cancellation — [K03]
- Cheap TMS options already exist: AscendTMS is free for 3 or fewer users, and TruckLogics costs $36/mo billed annually and "includes IFTA" — [K03]
- "FMCSA publishes new MC authority grants daily". Trucking Facebook groups are multilingual (Punjabi, Russian/Ukrainian, Spanish) — [K03]
- It ranks in the top 3 in IL, IN, ND and OH, and is listed with the IFTA Oct 31 hook in TX, GA, IA and AR — [STATES], [TX], [GA], [IA], [AR], [ND]

**K04 TowLedger (towing/impound)**
- Towbook costs $109–$429/mo depending on call volume, is month to month with a 30-day trial, and is rated 4.8/5 on 82 Capterra reviews. The file says "Evidence is thin". DMV owner lookups require DPPA permissible use — [K04]

**K05 MoveBoard (movers/junk removal)**
- SmartMoving and Supermove publish no prices. Incumbents rate 4.4–4.9 on Capterra, and the category has 101 products. The file says "Do not build this until 10 owner interviews confirm the pain" — [K05]

**K06 WashClub (car-wash memberships)**
- Rinsed CRM costs $765–$849 per location per month, plus $599 implementation and a 4% commission — [K06]
- "Membership status lives in the tunnel POS and LPR system. Without integration we are an overlay". The file also says "Evidence is thin", and the auto-renewal law angle is unverified — [K06]

### Inferences

#### Full score table (solo-developer rubric, ideas as written by the corpus; 5 = best for a solo developer)

Columns: **B** = solo build scope, **R** = regulatory/liability, **S** = self-serve sale, **Di** = solo-reachable distribution, **W** = willingness to pay/ARPU, **G** = gap versus cheap tools, **U** = urgency Oct 2026–Apr 2027, **Su** = support load and retention.

| ID | Product | Corpus /25 | B | R | S | Di | W | G | U | Su | **Solo /40** | Kill flags (full; *partial*) | Verdict |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| K02 | DealJacket (CA CARS Act) | 17 | 4 | 2 | 4 | 4 | 4 | 3 | 4 | 4 | **29** | *one-state legal rules with liability* | **Shortlist #1** |
| K03 | HaulDesk (fleet + IFTA) | 19 | 3 | 3 | 5 | 5 | 3 | 2 | 5 | 3 | **29** | Crowded with cheap tools (TruckLogics $36 with IFTA, AscendTMS free) | **Shortlist #2** (wedge) |
| C05 | FlatBuild (CoConstruct exodus) | 20 | 2 | 4 | 3 | 4 | 5 | 2 | 5 | 3 | **28** | Feature-parity monster; *funded rivals already running the same migration play* | **Shortlist #3** (wedge only) |
| C04 | RouteBook (pool/cleaning) | 16 | 3 | 5 | 5 | 4 | 3 | 1 | 2 | 4 | **27** | Crowded with cheap tools | Rule out |
| C03 | SprayLog (pest/lawn + NY report) | 18 | 2 | 3 | 4 | 3 | 4 | 3 | 4 | 3 | **26** | Feature-parity (full route FSM); offline-first mobile (as written) | **Shortlist #4** (wedge only) |
| C06 | LienClock (lien deadlines) | 18 | 4 | 1 | 4 | 4 | 4 | 3 | 2 | 4 | **26** | Multi-state legal rules with customer liability | Rule out for now |
| K05 | MoveBoard (movers/junk) | 14 | 3 | 3 | 5 | 4 | 4 | 2 | 2 | 3 | **26** | Crowded (101 products; Jobber/HCP); pain unproven | Rule out |
| C07 | ClaimKit (restoration/supplements) | 17 | 2 | 3 | 4 | 3 | 5 | 3 | 2 | 3 | **25** | Offline-first mobile capture (as written); *partial parity vs CompanyCam/Encircle; public-adjuster limits* | **Shortlist #5** (conditional, wedge only) |
| D04 | ShiftTip (scheduling + tips) | 18 | 3 | 2 | 4 | 4 | 3 | 2 | 4 | 3 | **25** | Crowded with free tiers (Homebase, 7shifts Comp, Sling); *multi-state wage/tip rules* | Rule out (near miss) |
| D06 | SiteLoop (campgrounds) | 16 | 2 | 3 | 3 | 3 | 5 | 3 | 4 | 2 | **25** | Feature-parity; payments core; offline (rural) | Rule out |
| D07 | BookTrail (tours) | 19 | 3 | 3 | 4 | 4 | 3 | 2 | 4 | 2 | **25** | Crowded booking market; *payments core (Stripe Connect checkout, weather refunds)* | Rule out |
| C02 | StormDesk (roofing CRM) | 17 | 2 | 3 | 3 | 3 | 5 | 2 | 3 | 3 | **24** | Feature-parity (full CRM, supplier ordering); *Roofr flat and free tier* | Rule out |
| K06 | WashClub (car wash) | 14 | 2 | 2 | 3 | 3 | 5 | 4 | 2 | 3 | **24** | Payments core (dunning needs processor access); deep POS integration needed; *multi-state auto-renewal rules* | Rule out |
| D03 | TableKeep (reservations) | 19 | 3 | 3 | 3 | 3 | 4 | 2 | 3 | 2 | **23** | SMS/10DLC at scale (waitlist core); *crowded (judgment)* | Rule out |
| K01 | BayBook (auto repair) | 18 | 2 | 3 | 4 | 3 | 5 | 2 | 1 | 3 | **23** | Feature-parity; crowded low end (ARI $39.99, AutoRepair Cloud $49.99); *two-way texting core* | Rule out |
| C01 | FlatRate (HVAC/plumbing/electrical) | 19 | 1 | 4 | 3 | 3 | 5 | 2 | 2 | 2 | **22** | Feature-parity monster; offline-first mobile; crowded (Jobber $49, HCP $79, Workiz, FieldEdge) | Rule out |
| D08 | TeeFree (golf) | 15 | 2 | 3 | 2 | 2 | 5 | 2 | 4 | 2 | **22** | Feature-parity (tee sheet + POS); hardware (POS); *committee/RFP for munis and clubs* | Rule out |
| D02 | DirectPlate (online ordering) | 19 | 3 | 3 | 3 | 3 | 4 | 1 | 2 | 2 | **21** | Payments core; crowded (8 named rivals, Square Online) | Rule out |
| K04 | TowLedger (towing) | 13 | 3 | 2 | 4 | 4 | 4 | 1 | 1 | 2 | **21** | *State/city legal rules*; incumbent cheap and loved (no pain) | Rule out |
| D05 | InnDesk (hotel PMS) | 14 | 1 | 2 | 3 | 3 | 4 | 2 | 3 | 1 | **19** | Feature-parity; payments core; deep integrations (channel managers); crowded | Rule out |
| D01 | FlatTab POS (restaurant) | 15 | 1 | 2 | 3 | 3 | 3 | 1 | 3 | 1 | **17** | Payments core; hardware/offline; feature-parity; crowded (Square) | Rule out |
| D09 | ShelfPOS (retail) | 16 | 1 | 2 | 3 | 3 | 4 | 1 | 2 | 1 | **17** | Hardware; payments core; feature-parity; crowded (Square/Shopify POS) | Rule out |

#### Scoring conventions (judgment)
- Each idea is scored **as the corpus wrote it**, meaning its MVP list. Section 3 re-scores the narrow wedges.
- Urgency (U): 5 means a hard date between Oct 2026 and Apr 2027 that a product shipped by about Nov 21 2026 can still meet. 4 means a law already in force, or an off-season switching window plus a live reason to leave. 3 means rolling renewal or contract triggers. 2 means a season alone or a trigger that has already passed. 1 means none.
- Gap (G) uses the cheap competitors the corpus itself names. Cheap tools I believe the corpus missed are listed as verification asks in Key question 4, not scored as fact.
- Regulatory (R): C06 = 1 because the product computes multi-state lien deadlines, where one error loses a lien right. The corpus's own fact-check found four errors in eight states. K02 = 2 because it makes single-state legal determinations (return eligibility, restocking fee) that the dealer relies on. K03 = 3 because IFTA is mechanical arithmetic under one interstate agreement, and the carrier signs the return. D04 = 2 because of state-by-state tip-pool and break rules.

#### Short rationale per idea (judgment, grounded in the findings above)
- **K02:** The build is CRUD, timers, a photo checklist, e-sign and PDFs. The buyer is an owner who pays by card. A public license list makes cold outreach cheap. Seven-year records make customers sticky. The risks are a California-only market and DMS vendors adding the same features.
- **K03:** Owner-operators pay by card. The FMCSA new-authority list plus multilingual Facebook groups and Reddit make it the most solo-reachable buyer in the group. IFTA deadlines recur inside the window. The cheap end is crowded, though (TruckLogics at $36 includes IFTA), and owner-operators are very price-sensitive.
- **C05:** It has the strongest dated trigger in the group, a reachable list (builders who link CoConstruct client portals) and ARPU of $249+. But customers leaving CoConstruct need a full PM replacement, and well-funded flat-price rivals already offer migration.
- **C03:** The dated NY deadlines are real and the OGC 3 field list is concrete. As written, though, it is a full route FSM with offline mobile. Only a report generator plus application log fits a solo developer.
- **C04 and K05:** They score high on build, self-serve and low regulation, but the corpus's own evidence says the pain is mild or unproven and the incumbents are cheap and well liked. The crowding flag decides it.
- **C06:** The build is small and distribution is good (one deadline-calculator SEO page per state), but the liability is the worst in the group.
- **C07:** High ROI per claim. The full product needs a field-capture mobile app. Only an AI supplement-drafting wedge fits.
- **D01, D05, D09:** Every rubric flag points the same way: POS or PMS parity, hardware, payments, and real-time support at peak hours.
- **D02 and D03:** Large markets, but crowded, payments- or SMS-core products whose failures happen live during service.
- **D07:** Operators pay FareHarbor nothing, so a subscription is a hard sell. The checkout is payments-core, and many vendors already chase "FareHarbor alternative".
- **D06 and D08:** Real off-season windows, but the products are booking + billing + POS suites.
- **K01:** Parity monster (labor guide, parts catalogs, history) with cheap rivals and no deadline.
- **K04:** Towbook is cheap, month to month and rated 4.8/5, so there is no pain to sell against.
- **K06:** Pricing gap is high, but the product cannot work without POS integration and processor access.

### Gaps
- Market sizes in every file are corpus estimates labeled "not verified" (Census CBP counts were not pulled). That affects ARPU-to-$10k-MRR math for C03 (NY only) and K02 (CA only) most.
- Complaint evidence is thin or secondhand for K04, K05, K06 and C04, and mostly from competitor pages for D02, D07 and D08. No first-hand Reddit threads were pulled for D02, D03 or D05. Pain scores there may be off in either direction.
- The scores are one analyst's judgment. Rubric criteria 6 (cheap-tool gap) and 8 (support load) are the least evidenced, because the corpus did not research cheap indie competitors or support burden.

## Key question 2: Where does the corpus score (/25) disagree with the solo-developer view, and why?

### Takeaway
The biggest disagreements run in both directions. The corpus ranks C01, D02, D03 and D07 near the top of this group (19/25 each), but for a solo founder they are parity, payments or real-time products with crowded cheap markets. Meanwhile it ranks K02 mid-pack (17/25), and K02 is the best solo fit. The cause is structural. The corpus rubric rewards pain and market size and measures "build ease" as MVP buildability. It has no criterion for the parity customers need before they switch, for cheap competitors, for support load or for legal liability.

### Cited Findings
- The corpus scores five criteria: Pain, Price gap, Build ease, Sales speed and Market size. "Build ease" is defined as "how fast AI-assisted dev can ship a credible MVP (5 = CRUD + forms + notifications in 2–4 weeks; 1 = needs deep integrations, certifications, hardware...)", and "Market size" gives 5 to "500k+ businesses or a large dollar pool" — [CORPUS-RUBRIC]
- The solo rubric adds criteria for regulatory liability, cheap-tool gap, support load and retention, plus a feature-parity kill flag ("customer won't switch until most of the incumbent's features exist") — [RUBRIC]
- The corpus's own Priority list puts C05 (#4), D07 (#12), C01 (#13) and K03 (#14) in its top 15 — [INDEX]
- The INDEX's "ideas to put off" list (14/25 or below) includes D05, K04, K05 and K06 from this group — [INDEX]
- C01's corpus scores are Pain 5 and Market 5 but Build ease 2. The file concedes the category is crowded — [C01]
- K02's corpus scores are Price gap 2 and Market 3 but Sales speed 5 — [K02]
- D07's file concedes it is "hard to sell a subscription against $0" yet still scores Price gap 4 — [D07]

### Inferences

| ID | Corpus /25 (rank in group of 22) | Solo /40 (rank) | Direction | Why the views differ (judgment) |
|---|---|---|---|---|
| C01 | 19 (tied 2nd) | 22 (tied 16th) | Corpus much higher | Large market and loud pain earn corpus points, but switching requires dispatch, offline tech app, pricebook, memberships and payments. Jobber at $49 and HCP at $79 are cheap and good. |
| D02 | 19 (tied 2nd) | 21 (tied 18th) | Corpus much higher | Eight named rivals plus free Square Online. Checkout and delivery are payments-core, and order failures land during dinner rush. |
| D03 | 19 (tied 2nd) | 23 (tied 14th) | Corpus higher | SMS waitlist and host-stand reliability are core. OpenTable's diner network locks restaurants in. Both triggers (Jan 2026 fee, summer 2026 merger) are aging. |
| D07 | 19 (tied 2nd; top 3 in 7 states) | 25 (tied 8th) + flags | Corpus higher | The incumbent is free to operators, the product is payments-core, and many booking vendors already compete for "FareHarbor alternative". The corpus's broad geography (7 states) does not help a solo seller. |
| K02 | 17 (tied 11th) | 29 (tied 1st) | Solo much higher | A small CA-only market and price gap don't matter when $10k MRR needs about 127 rooftops at $79/mo (judgment). What matters solo: CRUD build, a law in force now, a public buyer list, sticky records. |
| C04 | 16 (tied 14th) | 27 (4th) | Solo higher on total but killed | Easy build and self-serve inflate the total, but the corpus's own evidence (mild pain, cheap incumbents) triggers the crowding flag. |
| K05 | 14 (tied 19th) | 26 (tied 5th) but killed | Same as C04 | The pain is unproven (the corpus itself says interview 10 owners first). |
| C06 | 18 (tied 7th) | 26 (tied 5th) but killed | Total similar; solo flags it | The corpus scores the price gap against Levelset, but its own fact-check found 4 legal errors in 8 states. That is a liability problem the corpus rubric cannot see. |
| D04 | 18 (tied 7th) | 25 (tied 8th) | Roughly agree, solo rules out | Free tiers from Homebase, 7shifts and Sling, plus wage-and-hour liability. |
| K03 | 19 (tied 2nd) | 29 (tied 1st) | Agree (high) | Both rubrics like card-paying owners and the IFTA deadline. The solo view adds a crowding warning. |
| C05 | 20 (1st) | 28 (3rd) | Agree on urgency | The solo view accepts it only as a narrow wedge, because the full PM is a parity monster against funded rivals. |
| D01, D05, D09 | 14–16 (bottom) | 17–19 (bottom) | Agree (low) | Both rubrics penalize hardware, POS/PMS parity and integrations. |

- The pattern (judgment): the corpus's "replace a bloated incumbent" frame favors big horizontal-vertical suites (field service, POS, reservations, booking). The solo frame favors narrow, compliance- or deadline-driven add-ons that sit beside the incumbent (K02, the K03 IFTA wedge, the C03 report, the C05 exit kit).
- On "Build ease" (judgment), the corpus scored whether an MVP can be built (C05 = 3, D07 = 4, D03 = 4). The solo rubric asks whether customers would switch to that MVP, and for suites they won't.

### Gaps
- The corpus gives no data on support load or churn in any of these 22 categories, so criterion 8 rests entirely on judgment.
- The corpus did not search for cheap indie competitors (under $30/mo) in most categories, so some solo "Gap" scores may be too generous, especially for K02, C03 and C07.

## Key question 3: What is the shortlist, and what is the narrowest sellable wedge for each?

### Takeaway
Ranked for "revenue fast", the shortlist is: (1) **K02 CARS Act 3-Day Return & Delivery Log** for California independent dealers, (2) **K03 IFTA Close** for owner-operators and small fleets, aimed at the **Jan 31 2027** return, (3) **C05 CoConstruct Exit Kit** before the **Mar 31 2027** cutoff, (4) **C03 NY Pesticide Report Builder** before **Dec 31 2026 and Feb 1 2027**, and (5, conditional) **C07 AI Supplement Drafter**. Each wedge can ship in 4–6 weeks (by about Nov 21 2026) as a web app that sits beside the incumbent, not in place of it. K02 and K03 are the only two that are recurring SaaS with no full kill flag once narrowed. C05's wedge is mostly one-time revenue that ends after Mar 31 2027.

### Cited Findings
- **K02:** The SB 766 duties (3-day return, $50k cap, 400 miles, 1.5% restocking fee bounded at $200–$600, 48-hour refund, total-price disclosure, retention periods) are listed with sources — [K02]. Vendors already market vehicle-condition photo documentation, because returns under the 3-day law depend on proving condition at delivery — [K02]. The California file says independents in LA, the Inland Empire and the Central Valley "are improvising on paper right now" and suggests selling a "first-90-days audit" — [CA]. Channels: CIADA, NIADA state associations, CA Dealer Academy, dealer-law firms, r/askcarsales and the public DMV license list — [K02]
- **K03:** The MVP list includes IFTA built from any ELD's CSV, fuel receipts by fuel-card CSV or photo OCR, per-state tax computation with a 4-year audit binder, AI-read rate confirmations, a broker MC/DOT check through the FMCSA QCMobile API, and factoring packets — [K03]. Corpus prices: Solo $39/mo, Fleet $99/mo, with IFTA included — [K03]. Channels: OOIDA, r/Truckers, TruckersReport, multilingual Facebook groups, daily new-authority lists, factoring partners, and "IFTA calculator" SEO published before each deadline — [K03]
- **C05:** Its MVP item 1 is a "CoConstruct and Buildertrend importer... We do it for you for free". The suggested outreach is to "Find CoConstruct client-portal links on builder websites... cold-email campaign with a 'free import' offer" — [C05]. Exports are limited, and some of the import is manual — [C05]
- **C03:** The suggested lead magnet is "Upload last year's service tickets CSV → get your NY DEC annual report file", which then converts users to paid — [C03]. The NY file suggests a "what can I still spray on Jan 1 2027" product checker for Long Island and Westchester lawn and tree companies — [NY]. Channels: the NYS Pest Management Association and distributors such as Target Specialty Products — [C03]
- **C07:** The MVP's AI supplement writer would "Compare the carrier's estimate (PDF upload) with our field evidence and draft a line-item supplement letter that cites the photos, measurements and code items", with a human reviewing every draft — [C07]. The corpus prices it at $149/mo flat, including the supplement writer — [C07]. Measurement reports are a commodity at $9–$19 from challengers — [C02]

### Inferences

All wedge specifications, prices and wedge-adjusted scores below are my judgment. A ship date of about Nov 21 2026 assumes 6 weeks from today.

**#1 K02 → "CARS Act 3-Day Log" (wedge-adjusted ~30/40: B5 R2 S4 Di4 W4 G3 U4 Su4)**
- **What ships in 4–6 weeks:**
  - A per-deal record keyed by VIN (free NHTSA decode), with manual entry or CSV import from DealerCenter/Frazer.
  - Automatic eligibility flag (used vehicle, $50k or less) and a 3-day countdown.
  - Odometer out/in against the 400-mile cap.
  - Restocking-fee calculator (1.5%, bounded at $200–$600).
  - A **48-hour refund timer** with SMS/email alerts to the manager.
  - A guided **delivery-condition photo walk-around** in mobile web, e-signed by the buyer at delivery and again at any return.
  - Total-price and add-on disclosure checklist, and printable 36-point signage.
  - A tamper-evident PDF "deal jacket" with retention set to 7 years.
- **Not in v1:** DMS integration, ad scanning, e-titling, contract (RISC) drafting (dealers keep their forms vendor).
- **Buyer:** Owner or GM of a California independent or BHPH used-car lot (10–150 cars a month).
- **Price:** $79/mo per rooftop, or $699/yr including 7-year storage (the corpus's price). A $49 "audit-only" tier is an option.
- **Channel:** Cold email to the public CA DMV dealer license list, starting with LA, the Inland Empire and the Central Valley. Then a CIADA webinar with a dealer attorney, and co-marketing with CA Dealer Academy.
- **Why #1:** The law is in force now, there is a public buyer list, the build is CRUD, and records accumulate.
- **Kill condition:** DealerCenter and Frazer already ship equivalent features for free, or SB 766 details have changed (see Key question 4).

**#2 K03 → "IFTA Close" (wedge-adjusted ~30/40: B4 R3 S5 Di5 W3 G2 U5 Su3)**
- **What ships:**
  - Upload of the ELD's jurisdiction-mileage export (Motive, Samsara or generic CSV).
  - Fuel purchases from fuel-card CSVs or **receipt photos read by Claude vision**, with a weekly "snap your receipts" text nudge so it gets used between quarters.
  - Per-jurisdiction taxable miles, gallons, tax due or credit, with MPG and missing-receipt anomaly flags.
  - A base-state return worksheet (PDF and CSV), a 4-year audit binder, and deadline reminders.
- **Month 2 (retention layer):** forward a rate confirmation by email → AI-extracted load → POD/BOL photo link → invoice and factoring packet, plus the FMCSA broker check.
- **Not in v1:** ELD, load board, dispatch, settlements.
- **Buyer:** Owner-operators with their own authority and 2–10 truck fleets. Often the spouse or office person does the paperwork.
- **Price:** $39/mo solo and $99/mo fleet (the corpus's prices), plus a $49 pay-per-quarter option for occasional users (judgment).
- **Channel:** FMCSA daily new-authority list, r/Truckers and TruckersReport, Punjabi, Russian/Ukrainian and Spanish Facebook groups (Claude-localized UI), "IFTA calculator" SEO, and factoring-company referral deals.
- **Timing:** The **Oct 31 2026** deadline is 21 days away and cannot be met by a new build. Launch content in December for the **Jan 31 2027** Q4 return, then Apr 30 2027.
- **Kill condition:** Major ELDs already produce filing-ready IFTA summaries for free, or $10–$36 tools already do receipt OCR (see Key question 4).

**#3 C05 → "CoConstruct Exit Kit" (wedge-adjusted ~29/40: B4 R4 S4 Di4 W3 G3 U5 Su2)**
- **What ships:**
  - A Chrome extension plus web app. Using the builder's own logged-in session, it exports every job (selections, specs, change orders, schedules, messages, photos, documents, budget summaries) into a neutral, searchable archive (a PDF per job plus CSV and JSON).
  - Mapper templates for importing into the builder's next tool (JobTread, Buildertrend, Houzz Pro, QuickBooks Online).
  - Optional "done-for-you" migration as a productized service.
- **Recurring tail:** a $29–$49/mo read-only archive vault for warranty-period records. A later upsell could be a standalone selections-and-change-order client portal at $99/mo.
- **Buyer:** Owner or office manager of a remodeler or custom builder still on CoConstruct.
- **Price:** $299–$999 one-time per company, by job count, plus the vault.
- **Channel:** Cold email to builders whose sites link CoConstruct client portals (the corpus method), "CoConstruct export / shutting down" SEO and a Chrome Web Store listing, NARI chapters, ContractorTalk and r/Contractor.
- **Caveat:** This is fast cash, not durable SaaS. Revenue peaks before Mar 31 2027 and then fades. The full PM product is not recommended.
- **Kill condition:** CoConstruct keeps historical data viewable for free indefinitely and offers a full native export, or its terms forbid automated extraction.

**#4 C03 → "NY Pesticide Report Builder + Neonic Checker" (wedge-adjusted ~28/40: B5 R3 S4 Di3 W3 G3 U5 Su2)**
- **What ships:**
  - A free web tool: upload last year's service-ticket or application CSV (from GorillaDesk, Jobber, PestPac or FieldRoutes exports, or a spreadsheet) and get a validated NY annual-report file with all OGC 3 fields. Errors are flagged, such as a missing EPA registration number or a bad 5-digit ZIP.
  - **Paid tier at $29–$49/mo or $299/yr:** a mobile-web application log (product picked from a registered-product list with the EPA registration number filled in automatically, GPS address and ZIP), an audit PDF, and a **neonic checker**. The checker flags products containing imidacloprid, thiamethoxam or acetamiprid for outdoor ornamental and turf use from Dec 31 2026.
- **Buyer:** NY lawn, tree and pest companies with 1–30 technicians.
- **Channel:** NYS Pest Management Association, Long Island and Westchester lawn and tree associations, distributor counters, r/lawncare and r/pestcontrol, and the DEC registered-business list if it is public (verify).
- **Weakness:** Annual cadence (churn risk after Feb 1) and a NY-only market. The expansion path is California pesticide use reporting and other states, one at a time.
- **Kill condition:** NY DEC already offers a free online submission tool or template that does the same validation, or incumbents already export the file.

**#5 (conditional) C07 → "Supplement Draft" (wedge-adjusted ~27/40: B4 R3 S4 Di3 W5 G3 U2 Su3)**
- **What ships:**
  - A web app that takes the carrier's estimate PDF, a measurement-report PDF (EagleView, Roofr or Hover) and photos.
  - Claude extracts the line items, compares quantities to the measurements, flags commonly missed items, and drafts a supplement letter that cites the evidence. A human approves every draft.
  - A simple claim tracker.
- **Not in v1:** field-capture app, moisture logs, ESX output.
- **Buyer:** Owner or estimator at an insurance roofing or restoration firm. Independent supplement writers are a white-label second buyer.
- **Price:** $149/mo flat (the corpus's price), or $29–$49 per claim in credits (judgment).
- **Channel:** r/Roofing, supplement-writer Facebook groups, and partnerships with supplement services. Paid catastrophe ads are optional and expensive.
- **Why conditional:** There is no dated trigger, public-adjuster laws limit the language the product can use, and the AI-supplement competitor field was not researched.

**Near misses (not shortlisted; judgment)**
- **D04 → a "tip ledger + qualified-tips W-2 report" add-on** sold through the Square and Clover app marketplaces. Payroll providers will probably absorb this, and the rules were not verified.
- **C06 → a Texas-only lien calendar.** Viable only with attorney-reviewed rules and E&O insurance.
- **D06 → a metered-electric and seasonal-site billing add-on beside Campspot.** The supporting complaint is from 2020.
- **C01 → an AI flat-rate pricebook builder** that exports to Jobber/HCP/ServiceTitan formats. Likely one-time use.

**Revenue math (judgment):**

| Wedge | Path to $10k MRR | Note |
|---|---|---|
| K02 at $79/mo | about 127 rooftops | California only |
| K03 at a blended ~$60/mo | about 170 carriers | |
| C03 at $49/mo | about 204 NY firms | probably a large share of the NY market (unverified) |
| C07 at $149/mo | about 68 firms | |
| C05 | about 20 kits a month at ~$499 | roughly $10k/month of one-time cash until Mar 2027 |

### Gaps
- None of the five wedges has customer-interview evidence in the corpus. Each needs 5–10 buyer conversations before or during the build.
- The corpus does not give the number of California independent dealers, NY registered pesticide businesses or remaining CoConstruct users. Those numbers set the ceiling for K02, C03 and C05.
- CoConstruct's export options and terms of service, which decide whether C05's Chrome-extension approach is feasible, are not in the corpus.
- Whether ELDs already output filing-ready IFTA, which decides K03's value, is not in the corpus.

## Key question 4: Which corpus claims most need fresh web verification, and which switching windows have already passed (as of Oct 10 2026)?

### Takeaway
The two top-ranked ideas (K02, K03) come from files that were **never fact-checked**. In this group only C05 and C06 have a Verification section. So the first web-validation round should confirm the SB 766 provisions and competing CARS Act tools, then IFTA tool density and what ELDs already provide. Several corpus triggers have already passed or aged out: the CARS Act took effect Oct 1, and the Jobber promo, the OpenTable fee, the Resy–Tock merger, the FTC fee rule and the NYC cap settlement are all behind us. The Oct 31 IFTA deadline is too close for a new build.

### Cited Findings
- INDEX section 8 says the fact-check pass covered "the top 12 ideas... along with C06, H02 and the S1/S2/S8 ideas", and that each checked file "ends with a Verification section" — [INDEX]. In this group only C05 and C06 have one. D07 (#12 by Priority), C01 (#13) and K03 (#14) do not (observed by listing the files' headings).
- The INDEX switching-window calendar lists, for this group:
  - Oct 1 2026 CARS Act (K02)
  - Oct 31 2026 IFTA Q3 (K03)
  - Oct–Dec 2026 off-season switching for tours, campgrounds and golf (D06, D07, D08)
  - Jan 1 2027 payroll and wage changes (D04)
  - Feb 1 2027 NY pesticide annual report "(verify)" (C03)
  - Mar 31 2027 CoConstruct stops new projects (C05)
  - Source: [INDEX]
- The C05 cutoff was verified against coconstruct.com on Sep 24 2026. That page "gives no end-of-life date for the product itself" — [C05]
- The NY Feb 1 report date is marked "(verify)" because the DEC page doesn't state it. The Dec 31 2026 neonic expansion is ✅ against DEC — [NY]
- D04's federal "no tax on tips" reporting is "Not re-verified via web in this pass" — [D04]
- D03's Resy–Tock merger timing is "per Eat App. A later pass should confirm the migration timeline" — [D03]
- K02 calls Oct 1 2026 "one week from today", written Sep 24 — [K02]
- C01: "Jobber is running a 'save up to 40%' promo for sign-ups before Sep 30 2026" — [C01]
- Prices across the group were "checked Sep 24 2026" (Tekmetric, Jobber, HCP, Towbook, Rinsed, Frazer, Skimmer, CompanyCam, Roofr), and INDEX warns "Prices change often, so check them before quoting them" — [INDEX], [K01], [K04], [K06]

### Inferences

#### Switching-window status on Oct 10 2026

| Date | Trigger | Ideas | Status |
|---|---|---|---|
| Early 2023 / Sep 1 2024 | Toast $0.99 fee (reversed) and +0.23% processing increase | D01, D02 | **Passed** (stale hooks) |
| May 12 2025 | FTC junk-fee rule for lodging and tickets | D05, D06, D07 | **Passed.** Still a selling point, not a deadline |
| Jun 2025 | NYC delivery fee-cap settlement | D02 | **Passed** (16 months old) |
| Jul 2 2025 | 7shifts plan changes | D04 | **Passed** |
| Jan 2026 | OpenTable 2% deposit fee | D03 | **Passed** (9 months old) |
| "Summer 2026" | Resy–Tock merger | D03 | **Likely passed.** Timeline was never confirmed |
| Sep 30 2026 | Jobber up-to-40% promo ends; Florida minimum-wage step | C01, D04 | **Passed** |
| Sep–Oct 2026 | HVAC shoulder season before the heating rush | C01 | **Closing now** |
| **Oct 1 2026** | CA CARS Act (SB 766) in force | K02 | **Passed 9 days ago.** The obligation is live, so this is now a first-90-days compliance sale, not a pre-deadline one |
| **Oct 31 2026** | IFTA Q3 return | K03 | **21 days away.** Too soon for a new build. Use it for content and list-building only |
| Oct 2026–Feb/Mar 2027 | Off-seasons for roofing, tours, campgrounds, pool, golf and hotels | C02, C04, D05–D08 | **Open** |
| Nov 30 2026 | End of hurricane season | C02, C07 | **Open** |
| **Dec 31 2026** | NY neonic ban expansion | C03 | **Upcoming** (verified against DEC in the NY file) |
| Jan 31 2027 | IFTA Q4 return | K03 | **Upcoming: first realistic launch target** |
| Jan 31 2027 | W-2s for tax year 2026 with tip reporting (date is judgment; corpus says "2026 W-2s") | D04 | **Upcoming, unverified** |
| **Feb 1 2027** | NY Pesticide Reporting Law annual report | C03 | **Upcoming. Date needs verification** |
| **Mar 31 2027** | CoConstruct stops new projects | C05 | **Upcoming** (verified Sep 24 2026) |
| Apr 30 2027 | IFTA Q1 return | K03 | Upcoming |
| Rolling, late 2026 to mid 2027 | Clover 36-month equipment terms from the 2023–24 Payeezy migration expire (corpus inference) | D01, D09 | Rolling, with no single date |

#### Verification asks, in priority order (judgment on priority)
1. **K02 SB 766 provisions and date:**
   - Confirm it took effect Oct 1 2026 with no delay or 2026 cleanup amendment.
   - Confirm the 3-day-return thresholds: $50k cap, 400 miles, 1.5% restocking fee bounded at $200–$600, 48-hour refund.
   - Confirm the covered dealers and the retention periods.
   - The corpus relies on a dealer-education vendor's guide plus the bill text, and the file has no Verification section.
2. **K02 competitor density:**
   - Did DealerCenter ($99) or Frazer ($129/$199) ship CARS Act modules by Oct 1? What do ComplyAuto and ProMax charge?
   - Are there low-cost independent-dealer compliance or deal-jacket tools the corpus missed? Possibilities (judgment): forms-vendor add-ons, e-contracting platforms, dealer-association toolkits.
   - Also check whether the FTC Safeguards Rule (GLBA) imposes vendor obligations for storing buyer IDs and credit documents (judgment).
3. **K02 market size:** the count of CA licensed independent dealers, and the format and availability of the DMV Occupational Licensing list.
4. **K03 IFTA tool density:**
   - What Motive and Samsara already output for IFTA (filing-ready or not).
   - TruckLogics' current $36/mo price and IFTA features (the source is from May 2026).
   - Other low-cost IFTA calculators and filing services (judgment: several exist), and the prices of IFTA filing services, which the corpus did not capture.
   - Whether factoring companies bundle free TMS or document apps.
5. **K03 dates and data:** confirm the Jan 31 and Apr 30 2027 due dates, the availability of IFTA's quarterly tax-rate table, and the fields and contact data in FMCSA's daily new-authority records.
6. **K03 single-source claims:** DAT renewals up 25–45% and "about 19,000 fake loads" in March 2025 both come only from Small Fleet HQ. Neither should be used in marketing until confirmed.
7. **C05 cutoff and post-cutoff access:**
   - Is Mar 31 2027 still the date?
   - After it, is historical data viewable for free, for how long, and at what cost?
   - What can CoConstruct's native export do, and do its terms of service allow automated extraction from a user's own account?
8. **C05 competitors:**
   - JobTread's $199 + $20/user price and its free-migration terms.
   - Buildertrend's incentives for CoConstruct users and Projul's offer.
   - Cheaper flat-price PM tools the corpus did not price. Possibilities (judgment): Contractor Foreman, Houzz Pro, Knowify, Buildxact.
9. **C03 NY reporting mechanics:**
   - The actual due date (the corpus says Feb 1, marked verify) and the OGC 3 fields.
   - Whether DEC offers its own online submission system or spreadsheet template.
   - Whether GorillaDesk, FieldRoutes, PestPac or ServSuite already export the NY report. The corpus claims GorillaDesk and Jobber lack chemical compliance, which needs a check.
   - How many registered NY pesticide businesses there are, and whether the list is public.
10. **C07 AI supplement competitors and limits:**
    - Which AI supplement-drafting tools exist and what they charge (judgment: there is a growing set of AI tools, plus outsourced supplement firms that take a percentage of the recovered amount; I did not name them because I could not verify them).
    - Public-adjuster restrictions on contractors in TX, FL and LA.
    - Current Xactimate and CompanyCam prices.
    - Note that the "85% O&P denial" figure is one reviewer's claim.
11. **Cross-cutting price re-checks** before any comparison page: Tekmetric, Jobber, HCP, Roofr, Towbook, Rinsed, Frazer and DealerCenter, all checked Sep 24 2026.
12. **If D07 is revisited:**
    - FareHarbor's 6% fee and the status of its "Desk" rollout.
    - Whether CA SB 478 or CO HB25-1090 actually reach guest-paid booking fees (both marked "legal check needed" in the corpus).
    - Cheap booking tools (judgment: Bookeo, Checkfront and similar).

#### Cheap indie competitors the corpus probably missed (judgment, all to verify)

| Idea | Possible missed competitors |
|---|---|
| D03 | Tablein, resOS, Yelp Guest Manager, Toast Tables |
| D04 | Connecteam and When I Work free or cheap tiers |
| D07 | Bookeo, Checkfront |
| C05 | Contractor Foreman, Houzz Pro |
| K03 | Low-cost IFTA-only tools |

These would harden the "crowded" flags on D03, D04 and D07 and could lower K03's and C05's Gap scores.

### Gaps
- I could not check any date, price or competitor on the live web, by design. Every "upcoming" status above assumes the corpus dates still hold.
- The corpus does not say whether SB 766 had follow-up legislation, whether CoConstruct extended its cutoff, or whether IRS tip-reporting rules for 2026 W-2s were finalized. These are the three date risks with the biggest impact on the shortlist and D04.

[RUBRIC]: </home/user/independant-saas-ideas/research_notes/Solo developer SaaS opportunity shortlist/_solo_dev_rubric.md>
[INDEX]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/INDEX.md
[CORPUS-RUBRIC]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/_TEMPLATE_AND_RUBRIC.md
[SCORE]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/_scoreboard.csv
[STATES]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/_states_summary.csv
[C01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C01-field-service-hvac-plumbing-electrical.md
[C02]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C02-roofing-exteriors-crm-storm.md
[C03]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C03-pest-control-lawn-care-compliance.md
[C04]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C04-pool-cleaning-route-businesses.md
[C05]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C05-construction-pm-remodelers-coconstruct-exodus.md
[C06]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C06-lien-deadlines-notices-waivers.md
[C07]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/C07-restoration-claims-documentation-supplements.md
[D01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D01-restaurant-pos-toast-clover-alternative.md
[D02]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D02-direct-online-ordering-chownow-owner-alternative.md
[D03]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D03-reservations-waitlist-opentable-resy-alternative.md
[D04]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D04-restaurant-scheduling-tips-7shifts-homebase-alternative.md
[D05]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D05-independent-hotel-pms-cloudbeds-alternative.md
[D06]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D06-campground-rv-park-campspot-alternative.md
[D07]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D07-tours-activities-fareharbor-peek-alternative.md
[D08]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D08-golf-tee-sheet-golfnow-barter-alternative.md
[D09]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/D09-independent-retail-pos-lightspeed-clover-alternative.md
[K01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/K01-auto-repair-shop-tekmetric-shopmonkey-alternative.md
[K02]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/K02-independent-dealer-ca-cars-act-compliance-dealercenter-frazer.md
[K03]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/K03-small-fleet-back-office-eld-tms-ifta-samsara-motive-dat.md
[K04]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/K04-towing-impound-compliance-towbook-alternative.md
[K05]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/K05-movers-junk-removal-smartmoving-supermove-alternative.md
[K06]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/K06-car-wash-membership-crm-rinsed-alternative-detailers.md
[NY]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/NY-new-york.md
[CA]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/CA-california.md
[CO]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/CO-colorado.md
[TX]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/TX-texas.md
[GA]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/GA-georgia.md
[IA]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/IA-iowa.md
[AR]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/AR-arkansas.md
[ND]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/ND-north-dakota.md
[LA]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/LA-louisiana.md
