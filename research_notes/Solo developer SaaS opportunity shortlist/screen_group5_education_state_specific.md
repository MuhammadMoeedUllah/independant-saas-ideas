# Screen group 5: education/books and state-specific SaaS ideas, re-scored for a solo developer

Scope: 23 idea files (P01–P07, R01–R08, S1-01, S2-01, S4-01, S5-01, S7-01, S8-01, S9-02, S9-04), scored with the solo-developer rubric ([RUBRIC][]). Method: each idea file was read in full, along with INDEX sections 1–6 and 8 and the state top-3 tables (`_states_summary.csv`, `_states_edu_summary.csv`). No web search was used. All facts come from the corpus, which was written Sep 24–25 2026. Citations like [P03][] point to the corpus file, and the corpus's own underlying URL is added where a number or date matters. Anything marked **(judgment)** is this screener's opinion, not a sourced fact. Today is 2026-10-10.

**Flag codes.** Rubric kill flags: PHI (HIPAA), PAY (core value depends on payments or holding funds), SMS (telephony or A2P 10DLC at scale), HW (hardware or offline-first mobile), GOV (enterprise, government or committee buyer), LAW (multi-state legal rules where a wrong answer creates liability), PARITY (feature-parity monster), CROWD (crowded with cheap indie tools). Extra watch flags for this group: CHILD (COPPA/FERPA/student-privacy exposure), WTP (consumer price under about $15/mo, or buyers expect free), CEIL (reachable market too small to reach about $10k MRR), SEASONAL (one-shot yearly use).

---

## Key question 1: What are the 8 rubric scores (/40), the kill flags and the evidence for each assigned idea?

### Takeaway
Five of the 23 ideas score 28/40 or more with at most one partial kill flag: S9-04 CoverDesk (32), S1-01 Part500 Kit (29), S2-01 ParCheck (29), R05 SpineDesk (28) and S4-01 FortiFile (28). All five are owner-operator compliance or back-office tools. The child- and school-facing education ideas mostly land between 16 and 27. They fail on school, library or government procurement (R01, P02, R02, P06), child-data exposure (R08, P06, P02) or consumer prices under $15/mo (P03, P07, R07, R08, R06).

### Cited Findings

#### Score table (scores are judgment applied to the cited evidence below; sorted by /40)
Columns 1–8 follow the rubric: Build = solo build scope, Reg = regulatory/liability, Self = self-serve sale, Reach = solo-reachable distribution, WTP = willingness to pay/ARPU, Gap = gap versus cheap indie tools, Urg = urgency Oct 2026–Apr 2027, Supp = support load and retention.

| ID | Product (buyer) | Build | Reg | Self | Reach | WTP | Gap | Urg | Supp | **/40** | Corpus /25 | Rubric kill flags | Watch flags | Verdict |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| S9-04 | CoverDesk (SC Option 3 association directors) | 5 | 4 | 4 | 5 | 3 | 3 | 4 | 4 | **32** | 17 | none | CEIL (81 buyers) | Shortlist |
| S1-01 | Part500 Kit (NY DFS-licensed agency/broker owners) | 4 | 3 | 4 | 3 | 3 | 4 | 5 | 3 | **29** | 19 | none | legal-advice liability (mild) | Shortlist |
| S2-01 | ParCheck (Delaware corp/LLC owners, startup CPAs) | 5 | 4 | 5 | 4 | 2 | 2 | 5 | 2 | **29** | 19 | CROWD (partial; judgment) | WTP, SEASONAL | Shortlist (seasonal cash) |
| R05 | SpineDesk (indie bookstore owners) | 3 | 4 | 5 | 4 | 4 | 3 | 2 | 3 | **28** | 15 | CROWD (partial: book by book at $29) | CEIL (about 3–4.5k stores) | Shortlist |
| S4-01 | FortiFile (FORTIFIED-certified roofers, OK/LA) | 3 | 4 | 4 | 4 | 5 | 3 | 2 | 3 | **28** | 16 | HW (partial: field photo app) | CEIL, grant-round volatility | Shortlist (conditional) |
| P01 | PhonicsPrep (OG/structured-literacy tutors) | 4 | 4 | 5 | 4 | 2 | 2 | 2 | 4 | **27** | 17 | CROWD | WTP | Near-miss |
| P03 | HomeRoll (homeschool parents) | 4 | 4 | 5 | 4 | 1 | 2 | 3 | 4 | **27** | 18 | CROWD; LAW (partial: 50-state homeschool wizard) | WTP | Reuse as S9-04's family log, not standalone |
| P04 | ClassHouse (independent kids'-class teachers) | 3 | 3 | 5 | 4 | 3 | 3 | 3 | 3 | **27** | 19 | PAY (partial); CROWD (partial; judgment) | CHILD | Near-miss |
| R06 | LaunchShelf (indie authors) | 3 | 4 | 5 | 5 | 2 | 2 | 2 | 3 | **26** | 19 | CROWD | WTP | Near-miss |
| S8-01 | RebuildLedger (LA fire-rebuild GCs) | 2 | 2 | 3 | 4 | 5 | 3 | 5 | 2 | **26** | 19 | PARITY; LAW (single-state contract rules) | time-bound market | Near-miss (document wedge only) |
| P07 | LearnLedger (parents spending 529/ESA money) | 4 | 2 | 5 | 3 | 1 | 3 | 4 | 2 | **24** | 17 | LAW | WTP, SEASONAL, unproven pain | Kill as a product |
| S7-01 | GuideLedger (Mountain West outfitters) | 2 | 3 | 4 | 3 | 3 | 3 | 4 | 2 | **24** | 16 | HW; PAY; PARITY | CEIL, SEASONAL | Kill |
| S9-02 | ReadyTutor LA (LA voucher-paid reading tutors) | 4 | 3 | 5 | 2 | 2 | 2 | 3 | 3 | **24** | 15 | CROWD (partial; judgment) | CEIL, WTP | Fold into P01 if P01 proceeds |
| R03 | Branchline (small public libraries) | 4 | 3 | 2 | 2 | 3 | 3 | 2 | 4 | **23** | 13 | GOV | low pain | Pass |
| P02 | ReadingPlan Home (K–3 schools) | 3 | 2 | 2 | 2 | 3 | 4 | 3 | 3 | **22** | 16 | GOV; LAW | CHILD | Kill |
| R02 | ReadRally (libraries, PTAs) | 3 | 3 | 3 | 3 | 2 | 2 | 4 | 2 | **22** | 19 | GOV; CROWD; PAY | CHILD, WTP | Kill |
| R08 | Readlings (parents of 4–8-year-olds, K–2 teachers) | 3 | 2 | 5 | 3 | 1 | 2 | 2 | 3 | **21** | 18 | CROWD | CHILD, WTP | Kill |
| S5-01 | ClockRight IL (Illinois hourly employers) | 2 | 2 | 4 | 3 | 3 | 1 | 3 | 2 | **20** | 17 | PARITY; CROWD; LAW | — | Kill |
| P05 | PTOHub (PTO boards) | 2 | 3 | 3 | 3 | 2 | 1 | 2 | 2 | **18** | 17 | PARITY; CROWD; PAY; GOV | CHILD | Kill |
| P06 | StoryNest (Head Start, preschools, home daycares) | 3 | 2 | 2 | 2 | 2 | 2 | 2 | 2 | **17** | 15 | SMS; GOV | CHILD, WTP | Kill |
| R01 | ClearShelf (school districts) | 2 | 1 | 1 | 2 | 4 | 3 | 2 | 2 | **17** | 16 | GOV; LAW; PARITY | CHILD, political | Kill |
| R07 | ReadClear (parents, librarians) | 2 | 1 | 4 | 3 | 1 | 2 | 2 | 2 | **17** | 13 | CROWD | WTP, copyright/defamation liability, political | Kill |
| R04 | OpenBookFair (PTAs + indie bookstores) | 2 | 2 | 2 | 3 | 1 | 2 | 3 | 1 | **16** | 15 | PAY; PARITY; GOV; HW (partial: event POS) | WTP | Kill |

#### Per-idea evidence (ordered as in the table)

**S9-04 CoverDesk (32/40).**
- The whole buyer pool is a public list. SCDE's 2026–27 Option 3 list names 81 associations, and each must file an Annual Standards Assurance form under S.C. Code §59-65-47 ([S9-04][]; [SCDE](https://ed.sc.gov/districts-schools/state-accountability/home-schooling/home-school-option-3/)).
- The status quo is email plus web forms. One association says "We do all communication via email" and enforces its Mar 1 and Jul 31 check-ins "strictly". Another guide gives ~Jan 5 and ~Jun 5 ([S9-04][]; [HHASC FAQ](https://www.hometownhasc.com/faqs/)).
- Associations charge families $35–$75 each, or $20–$50 per student. A 400-family association on Homeschool-life Connections ($9.95/family/yr) pays about $3,980/yr. CoverDesk's proposed tiers are free up to 50 families, $49/mo up to 400 and $99/mo up to 1,500 ([S9-04][]).
- Growth is real: South Carolina homeschooling grew +21.5% in 2024–25, the fastest of any state (JHU, via [S9-04][]).
- No public complaints about association tooling were found. The pain is process burden, and the corpus scores market size 1 for South Carolina alone and 2 with Tennessee umbrella schools ([S9-04][]). No child login in the MVP, and records stay parent-owned ([S9-04][]).
- Not in any state's top 3 ([EDU-CSV][]). The SC state file calls it a "B2B2C channel into P03" ([SC-state][]).

**S1-01 Part500 Kit (29/40).**
- Dated trigger: the annual certification or acknowledgment is due **Apr 15** and must be signed by the highest-ranking executive and the CISO or senior officer. Incident notice is due in 72 hours, and notice of an extortion payment in 24 hours ([S1-01][]; [DFS Submissions](https://www.dfs.ny.gov/cybersecurity/submissions)).
- Small entities still carry real duties. The 500.19(a) limited exemption (<20 staff, <$7.5M revenue or <$15M assets) still requires a program, written policies, MFA, an asset inventory, a risk assessment and training ([S1-01][]; [DFS Small Business](https://www.dfs.ny.gov/cybersecurity/small-business-resources)). Individual brokers and agents must file unless fully exempt ([S1-01][]).
- DFS says the emailed receipt "is the only confirmation" and "you may need the receipt number to renew your license" ([S1-01][]).
- Incumbent fit: Vanta and Drata are quote-only and don't list 23 NYCRR 500 as a featured framework (fetched Sep 24 2026) ([S1-01][]).
- Proposed price: $19/mo solo producer, $59/mo for agencies up to 20 people, and a $299 one-time done-with-you add-on ([S1-01][]).
- Weak spots the file admits: no review-site complaints and no competitor search (no web search that pass); DFS doesn't publish licensee counts; "many small licensees may certify without doing the work" ([S1-01][]). Ranked #4 in New York's state file ([NY-state][]).

**S2-01 ParCheck (29/40).**
- Dated trigger: corporations' annual report and franchise tax are due **Mar 1**, with a $200 penalty plus 1.5%/mo. The LLC/LP/GP tax is $400, due Jun 1 ([S2-01][]; [DE Division of Corporations](https://corp.delaware.gov/frtax/)).
- Concrete pain: by the official tables, 10M authorized shares gives $85,165 under the Authorized Shares method versus $400 under Assumed Par Value Capital, and the Division says to use the lesser method ([S2-01][]; [DE calculation](https://corp.delaware.gov/frtaxcalc/)).
- Market: 2.28M+ Delaware entities, including 334,461 formed in 2025 (74,716 of them corporations) ([S2-01][]).
- Incumbent prices: Harbor Compliance registered agent $99 intro rising to $159 at renewal; Northwest $125; Stripe Atlas $100/yr after year one, with no franchise-tax help ([S2-01][]).
- Proposed price: $49/yr per entity; $299/yr firm plan for 25 entities, then $8 each ([S2-01][]). The file itself flags "Free calculators exist" and "Seasonality and low ARPU" ([S2-01][]). Top-3 only in Delaware ([STATE-CSV][]).

**R05 SpineDesk (28/40).**
- The owner or GM decides and pays by card ([R05][]).
- Expensive incumbents: Basil from $245/mo plus 1% of gross sales and $250 setup; BookManager $6,000 one-time plus $1,330/yr for data; IndieCommerce $175/mo plus 1% (capped at $500), with a fee increase effective Jan 1 2026 ([R05][]).
- A cheap rival already exists: **book by book**, a Square add-on at **$29/mo or $299/yr**, imports Ingram, Edelweiss and PubEasy orders, but lists no consignment or events features. Bookflow is another Square add-on ([R05][]; [book by book](https://bookbybook.app/)).
- Pain: Square doesn't fill in book details from an ISBN scan (Mar 2025), and one shop enters "every single book that walks in the door" by hand ([R05][]).
- Market: 2,844 ABA member companies in 2024, 3,218 indie bookstores in 2025 (SAN) and 600+ stores added in 2025. The corpus estimates a $4–10M ARR pool ([R05][]).
- Proposed price: Starter $39/mo, Pro $79/mo. Channels: the Square App Marketplace and Shopify App Store, plus the public ABA store finder ([R05][]). Not in any state's top 3 ([EDU-CSV][]).

**S4-01 FortiFile (28/40).**
- Oklahoma's Strengthen Oklahoma Homes pays up to $10,000 per home, **directly to the contractor after the FORTIFIED certification is submitted**, so paperwork completeness is cash flow ([S4-01][]; [OID](https://oid.ok.gov/okready/)).
- Louisiana's Fortify Homes pays up to $10,000 per roof, but new rounds are "to be announced" ([S4-01][]; [LDI](https://ldi.la.gov/fortifyhomes/)).
- Louisiana contractors must keep a license, an IBHS listing, $1M general liability and workers' comp current, for subcontractors too (rules dated Mar 17 2025) ([S4-01][]).
- Incumbent prices: CompanyCam Core $63/mo for 1 user, Crew $129/mo for 3, plus $29 per extra user, so about $332/mo for a 10-person crew. AccuLynx is estimated at $350–$450/mo for 1–3 users. One JobNimbus user lost about 2,000 photos ([S4-01][]).
- Honest caveats in the file: no FORTIFIED-specific complaints were found; the market is "a few thousand firms" (estimate); and the IBHS directory is the outreach list ([S4-01][]).
- Proposed price: $149/mo flat with unlimited users ([S4-01][]). Ranked inside the C02 bundle in the OK and LA state files ([OK-state][]; [LA-state][]).

**P01 PhonicsPrep (27/40).**
- Free tools crowd the space. Project Read's free plan allows "up to 5 per week, no customizations". Its only listed paid plan is the $1,999/yr school plan; there is no individual tutor plan ([P01][]; [Project Read pricing](https://www.projectread.ai/pricing)). LitLab has a free teacher sign-up, and TeachQuill, TeacherTool.ai and Storytime AI are also on the market ([P01][]).
- Buyers can pay. Tutors bill $113.06/hr on average, and many providers are "maxed out" ([P01][]; Reading Guru).
- Proposed price: $15/mo or $149/yr per solo tutor; $49/mo for centers; $8/mo for classroom teachers; $5/mo for parents ([P01][]).
- No child accounts in the MVP ([P01][]). Pain evidence comes from news and research, not tutor complaints (Reddit blocked) ([P01][]). In 17 states' education top 3 ([EDU-CSV][]).

**P03 HomeRoll (27/40).**
- The corpus calls it "**Crowded and cheap** (low price gap)". Homeschool Planet costs $84.95/yr and Homeschool Manager $49/yr; Panda, Syllabird, Scholaric ($3–7/mo) and new App Store apps (Homeschooly, Home Edify, Schoolfolio, Hipling) compete too ([P03][]).
- Proposed price: Family $59/yr or $7/mo ([P03][]). Complaints are "moderate, not angry" and review volume is thin ([P03][]).
- The real gap: no listed planner advertises NY IHIP or quarterly-report generators, or a PA evaluator packet (corpus observation, not a user quote) ([P03][]). New York requires a letter of intent within 14 days, an IHIP within 4 weeks and quarterly reports ([P03][]; [NYSED](https://www.nysed.gov/nonpublic-schools/home-instruction-questions-and-answers)).
- Market: 3.408M homeschool students, estimated at 1.5–2M families, and TEFA pays $2,000 per homeschooler ([P03][]). It is in 35 states' education top 3 and is INDEX's recommended education bet ([EDU-CSV][]; [INDEX][]).

**P04 ClassHouse (27/40).**
- Marketplace cuts: Outschool keeps 30% and pays out 7–13 days later; Wyzant takes 25% plus a 9% fee; Preply takes 33% (falling to 18%) plus each new student's first lesson ([P04][]; [Outschool policy](https://support.outschool.com/en/articles/2382129-teacher-earnings-and-payments-policy)).
- Recent changes: Nerdy committed on Jul 31 2026 to wind down Varsity Tutors for Schools, and Outschool added pay-per-class on May 25 2026 ([P04][]).
- Proposed price: $29/mo solo, $79/mo studio, 0% platform fee on Stripe Connect. A teacher grossing $3,000/mo on Outschool would save about $9,300/yr ([P04][]).
- The file names the biggest risk as "losing marketplace demand". Teachers say "the market for classes is highly saturated", and new teachers "commonly launch with 1 to 2 students" ([P04][]).
- COPPA: parent-owned accounts and parent-gated class links ([P04][]). In 12 states' education top 3 ([EDU-CSV][]).

**R06 LaunchShelf (26/40).**
- BookFunnel's new plans took effect **Feb 20 2026**. Mid-List is $200/yr, against an old $100 plus $50 integration, so +33% like-for-like. **Existing customers are grandfathered** ([R06][]; [BookFunnel blog](https://blog.bookfunnel.com/2026/new-plans/)).
- Cheap alternatives in the file itself: StoryOrigin (free tier), Storyfinch magnets ($29/yr), Payhip (free plus 5%) and BookSirens ($100/yr) ([R06][]).
- Low willingness to pay: 44% of authors earn ≤$100/mo and 13% earn >$5k/mo (Written Word Media 2025) ([R06][]). Proposed price: $12/mo Author, $24/mo Pro ([R06][]).
- Incumbent reviews: Booksprout 1.7/5 on 39 reviews; BookBub 2.9/5 on 2,401 ([R06][]).
- The corpus lowered Sales speed 5 → 4 after verification ([R06][]). Not in any state's top 3 ([EDU-CSV][]).

**S8-01 RebuildLedger (26/40).**
- Market and trigger: 16,264 structures were destroyed (CAL FIRE), and CoConstruct stops taking new projects **Mar 31 2027** ([S8-01][]; [CoConstruct](https://www.coconstruct.com/migration)).
- Rules: LA County says a rebuild requires a fixed-price contract, a down payment of no more than the lesser of $1,000 or 10%, and progress payments no larger than the work completed ([S8-01][]).
- Incumbent prices: Buildertrend from the mid-$300s to $1,000+/mo; JobTread $199 plus $20 per user ([S8-01][]).
- Build scope: the MVP has 8 items, including an attorney-reviewed CA contract builder, draw packets with statutory lien releases, a homeowner portal, a permit tracker and CoConstruct/Buildertrend import ([S8-01][]).
- The file calls the market a "time-bound beachhead" and names JobTread and Projul as rival migration plays ([S8-01][]). INDEX makes it part of "Bet 2" ([INDEX][]).

**P07 LearnLedger (24/40).**
- The file admits the pain is "**inferred from rule complexity, not yet from user quotes**" and recommends 20 parent interviews first ([P07][]).
- The rules engine tells families "you can withdraw $X tax-free" across 13 non-conforming states (California adds a 2.5% penalty). The file names tax-advice liability and E&O insurance as risks ([P07][]).
- Price: $39/yr. Trigger: tax season Jan–Apr 2027 ([P07][]). In 17 states' education top 3 ([EDU-CSV][]).

**S7-01 GuideLedger (24/40).**
- The MVP includes an **offline-first guide app** and Stripe Connect deposits with payment plans ([S7-01][]).
- Incumbents: FareHarbor adds a 6% fee to the guest's checkout price; Rezdy costs $99/mo ([S7-01][]).
- Idaho requires use reports and charges a $150 late penalty ([S7-01][]).
- Market: "several thousand" outfitters (estimate). Outfitter complaints were not collected ([S7-01][]).
- Price: $79/mo in season, $19/mo off-season. Top-3 in Montana and Wyoming ([S7-01][]; [STATE-CSV][]).

**S9-02 ReadyTutor LA (24/40).**
- 369,033 students are eligible, but the $10M 2025–26 budget covers at most about 6,667 vouchers, and the fiscal note assumed 0.8% participation (~2,952 students) ([S9-02][]).
- The state voucher platform is closed, and GATOR purchases run through Odyssey ([S9-02][]).
- Price: $19/mo solo. Louisiana's tutor count is unknown, estimated in the low thousands ([S9-02][]).

**R03 Branchline (23/40).**
- Only **9.7%** of public libraries said they were interested in changing systems ([R03][]; Library Perceptions 2025).
- LibCal is about $4,867/yr in one older contract. 77% of libraries are small; one runs on $48k/yr. The corpus estimates the events-and-rooms slice at $7–21M/yr ([R03][]).
- Purchases need board approval, though directors can often buy under $1,000–$2,500 (estimate). Proposed price: $49–$199/mo ([R03][]).

**P02 ReadingPlan Home (22/40).**
- "District-wide deals are slow (DPA, board approval, often 3–9 months)" ([P02][]).
- Privacy load: FERPA, NY Ed Law 2-d, IL SOPPA, SOC 2 readiness and a 12-state rulebook ([P02][]).
- Price: $1,200/yr per school. Indiana retained ~3,040 third graders and 10,663 failed IREAD-3 ([P02][]). In 19 states' education top 3 ([EDU-CSV][]).

**R02 ReadRally (22/40).**
- Library side: Beanstack costs $1,430/yr (Dubuque) and READsquared $595 ([R02][]).
- Read-a-thon side: 99Pledges charges a 0% platform fee, PledgeAthon 0%, PledgeStar is free or 7% capped at $1,195, and PagePledge is flat ([R02][]).
- The Beanstack Tracker app has **4.8★ from ~98K ratings**; the pain is the buyer's price, not the reader's experience ([R02][]).
- Proposed price: libraries $0–$1,499/yr; read-a-thons 0% platform fee (optional tip or $199 per campaign) ([R02][]).

**R08 Readlings (21/40).**
- Incumbent prices: Epic $84.99/yr, ABCmouse $45 for the first year, Reading Eggs $99.99/yr, Ello $139/yr (AI Storytime since Sep 30 2024) ([R08][]).
- Full compliance with the amended COPPA rule has been required since **Apr 22 2026** ([R08][]). This product is child-directed.
- Proposed price: $49/yr per family ([R08][]). ABCmouse rates 1.2/5 on 83 reviews ([R08][]).

**S5-01 ClockRight IL (20/40).**
- Free tiers already exist: Homebase Basic (1 location, 10 employees) and 7shifts Comp ([S5-01][]).
- Most Illinois leave and tip-credit parameters are marked (verify), and the file flags legal accuracy as a risk ([S5-01][]). Proposed price: $39/mo per location ([S5-01][]).

**P05 PTOHub (18/40).**
- Cheap and free incumbents: Givebacks $499/yr; MoneyMinder $299/yr including Cheddar Up Team; Cheddar Up free or $15/mo; 99Pledges 0% ([P05][]).
- After verification the corpus cut Price gap to 3. Booster says schools keep 95% on average on MyBooster, and the 40–50% fee figures are only historical ([P05][]).
- The MVP spans a site, directory, dues, a store with Tap to Pay, pledge pages, a treasurer ledger and newsletters ([P05][]).

**P06 StoryNest (17/40).**
- Delivery is **text-first**, and parents upload photos and voice notes. Head Start records fall under 45 CFR 1303 ([P06][]).
- Prices: $9/mo for home daycares; $1,500/yr for grantees. Free substitutes include Vroom, Khan Kids and Imagination Library ([P06][]).
- Head Start funding is unstable: it was zeroed out in the preliminary FY2026 draft, and programs missed Nov 1 funding ([P06][]).

**R01 ClearShelf (17/40).**
- Buyers are district coordinators plus an assistant superintendent, buying through POs and board approval ([R01][]).
- The lead trigger is gone: Nebraska's LB 390 deadline passed, and "a paper binder would do" ([R01][]). Texas districts already run a Destiny Parent Portal ([R01][]).
- Price: $0.50 per student, $500 minimum. In 20 states' education top 3 ([R01][]; [EDU-CSV][]).

**R07 ReadClear (17/40).**
- The file names copyright and data access as the biggest risk: "We **cannot ingest full texts without a license**" ([R07][]).
- Price: Family $2.49/mo or $19/yr, against Common Sense Media at $3.99/mo. Shelf Checkout is free to download ([R07][]).

**R04 OpenBookFair (16/40).**
- Scholastic has $541.6M in fair revenue across ~90,000 fairs, and Literati already holds the "better fair" position ([R04][]; [INDEX][]).
- E-wallets "can look like stored value", and the bookstore margin is thin (about $600–$1,000 before labor). Revenue would be 3% of fair GMV ([R04][]).

### Inferences
- **The pattern (judgment):** the rubric rewards owner-operator buyers with a dated filing or season and a public list (S9-04, S1-01, S2-01, S4-01). It punishes ideas whose buyer is a school, library, Head Start grantee or district (R01, P02, R02, P06, R03), and kid-facing consumer apps priced at $2–$12/mo (R07, R08, P03, P07).
- **The rubric ignores market size,** so the top 5 need a ceiling check (judgment arithmetic):
  - S9-04 tops out at roughly $4–8k MRR in South Carolina even at 100% capture (81 associations × $49–99).
  - R05's pool is about 3.2k–4.5k stores. 200 stores at $49 would be about 5% share.
  - S4-01's pool is "a few thousand firms" nationally but smaller in grant states.
  - S1-01 (tens of thousands of NY licensees, estimate) and S2-01 (2.28M entities) have room but low or seasonal ARPU.
- **COPPA:** the amended rule has been in force since Apr 22 2026, so it is now a fixed cost for any child-facing product. That pushes P04, R08, R02 and P06 down further, compared with adult-only, parent-owned designs like P01, P03 and S9-04 (judgment).
- **Low consumer willingness to pay recurs** in this domain: $19–$59/yr (R07, P07, R08, P03), $5–$15/mo (P01's parent and solo tiers, R06). At those prices, $10k MRR needs 700–3,000+ paying households or authors. That is a paid-acquisition business, not a solo fast-revenue one (judgment).

### Gaps
- Competitor density was not checked in this round, and the corpus's own competitor lists are thin wherever web search had run out (S1-01, S2-01, S4-01, S7-01, S8-01 say so explicitly). Competitors added here (MagicSchool-type suites for P01; Sawyer, Jackrabbit, TutorBird or Teachworks for P04 and S9-02; Doola, Firstbase, Carta or Clerky calculators for S2-01; Connecteam, When I Work or Sling for S5-01; ComplianceForge-type policy packs for S1-01) are **judgment from background knowledge and unverified**.
- Pain evidence is weak for S9-04, S1-01, S2-01, S4-01, S7-01 and P07. Reddit was blocked in the corpus pass, and these files rely on regulator documents or inference rather than user complaints.
- Most market counts are corpus estimates: NY DFS licensees, FORTIFIED roofers, SC association member counts, Tennessee umbrella schools, OG tutors and Louisiana tutors.

---

## Key question 2: Where does the corpus's own score (/25) disagree with the solo-developer view, and why?

### Takeaway
The two views roughly agree on the compliance ideas (S1-01, S2-01) and on P01. They diverge most where the corpus rewards big but unreachable or low-ARPU markets and large state counts: P03, R02, R08, R01 and P05 drop, and INDEX's three recommended education bets (P03, P04+P01, R08) all score lower solo. The corpus also under-rates small, reachable niches with owner buyers: S9-04, R05 and S4-01 rise.

### Cited Findings

| ID | Corpus /25 (% of max) | Solo /40 (% of max) | Direction | Main reason (evidence) |
|---|---|---|---|---|
| S9-04 | 17 (68%) | 32 (80%) | **Up** | The corpus scored market size 1–2 ([S9-04][]). The solo rubric rewards a 5-score build and a fully public 81-name list. |
| R05 | 15 (60%) | 28 (70%) | **Up** | Corpus market size 2 ([R05][]). Solo: the owner pays by card, app-marketplace distribution, $39–79/mo. |
| S4-01 | 16 (64%) | 28 (70%) | **Up** | Corpus market size 2 ([S4-01][]). Solo: $149/mo, and the IBHS directory is a cold list. |
| R03 | 13 (52%) | 23 (58%) | Slightly up | The events/rooms slice is easy to build and support. The library board and 9.7% switching interest keep it low ([R03][]). |
| S1-01 | 19 (76%) | 29 (73%) | Agree | Dated Apr 15 filing, owner buyer, simple build ([S1-01][]). |
| S2-01 | 19 (76%) | 29 (73%) | Agree on total, differ on parts | The corpus's Build 5 and Sales speed 4 match. Solo adds the low per-entity ARPU ($49/yr) and the one-shot seasonality the file admits ([S2-01][]). |
| P01 | 17 (68%) | 27 (68%) | Agree | Both see a solo-friendly tutor buyer. Solo marks down the $15/mo price and free AI decodable tools ([P01][]). |
| S9-02 | 15 (60%) | 24 (60%) | Agree | Small single-state pool; 0.8% voucher take-up assumed ([S9-02][]). |
| S7-01 | 16 (64%) | 24 (60%) | Roughly agree | Solo adds HW/PAY/PARITY flags: an offline guide app and deposits are in the MVP ([S7-01][]). |
| P03 | 18 (72%), **#1 education Priority, 35 states** | 27 (68%) | **Down in rank** | The file admits "crowded and cheap" and prices at $59/yr ([P03][]). Its 35-state count reflects homeschool laws existing everywhere, not sellability ([EDU-CSV][]). |
| P04 | 19 (76%), Price gap 5 | 27 (68%) | Down | The price gap is against commissions, but marketplaces supply demand the teacher loses on leaving. The file calls lost demand the "biggest risk" ([P04][]). Payments and chargebacks add support. |
| R06 | 19 (76%) | 26 (65%) | Down | BookFunnel's repricing (Feb 20 2026) is past and grandfathered. The proposed $12/mo price and 44% of authors earning ≤$100/mo cap WTP ([R06][]). |
| S8-01 | 19 (76%), INDEX "Bet 2" | 26 (65%) | Down | The corpus gave Build ease 4. Solo sees construction-PM parity plus attorney-reviewed CA contracts and statutory lien forms, in a time-bound market ([S8-01][]; [INDEX][]). |
| P07 | 17 (68%) | 24 (60%) | Down | Unproven pain ("inferred"), tax-advice liability and $39/yr ([P07][]). |
| S5-01 | 17 (68%) | 20 (50%) | Down | Homebase and 7shifts free tiers, plus multi-layer leave-rule liability ([S5-01][]). |
| P02 | 16 (64%), 19 states | 22 (55%) | Down | School procurement takes "3–9 months", plus the FERPA/state-privacy stack ([P02][]). |
| R02 | 19 (76%), Build ease 5, Sales speed 4 | 22 (55%) | **Big down** | Public-library buyers. 0%-fee read-a-thon rivals are listed in the file itself. The Beanstack app is rated 4.8★ ([R02][]). |
| R08 | 18 (72%), INDEX third bet | 21 (53%) | **Big down** | Child-directed product under the amended COPPA rule (in force Apr 22 2026), $49/yr, and Ello's AI Storytime ([R08][]). |
| R01 | 16 (64%), 20 states | 17 (43%) | **Big down** | District procurement, state-law packs, library-record privacy and politics ([R01][]). |
| P05 | 17 (68%) | 18 (45%) | **Big down** | Feature-parity suite, free or cheap rivals, and Booster's "95% on average" claim ([P05][]). |
| P06 | 15 (60%) | 17 (43%) | Down | SMS delivery, grantee procurement, child media uploads ([P06][]). |
| R07 | 13 (52%) | 17 (43%) | Down | Data rights and liability ([R07][]). |
| R04 | 15 (60%) | 16 (40%) | Down | Stored-value wallet, logistics, and Literati already in place ([R04][]). |

- INDEX's education recommendation is "a 'family learning' suite built around HomeRoll (P03)", then "ClassHouse (P04) with PhonicsPrep (P01)", then "Readlings (R08)" ([INDEX][]).
- INDEX's quick-cash list includes "J06 LicenseLedger, plus S2-01 ParCheck: Delaware franchise tax is due Mar 1" ([INDEX][]).
- INDEX's Priority formula "adds 0.1 point for each state that ranks the idea in its education top 3" ([INDEX][]). The state counts: P03 35, R01 20, P02 19, P01 17, P07 17, R08 13, P04 12, R02 9 ([EDU-CSV][]).
- The corpus rubric has five criteria: Pain, Price gap, Build ease, Sales speed, Market size. It has no separate absolute-ARPU, support-load or child-privacy criterion ([INDEX][]).

### Inferences
- **Why the views diverge (judgment):**
  1. The corpus's "Price gap" measures how much cheaper we are than the incumbent. The solo rubric's WTP criterion asks whether the absolute price can reach $10k MRR with ≤200 customers. A cheaper rival to a $49–$139/yr consumer tool (P03, R08, R06, P07) scores well on the first and badly on the second.
  2. The corpus's "Market size" rewards large populations (homeschool families, K–2 children, schools) whether or not one person can reach them. The solo rubric ignores size but rewards reachability, which flips S9-04, R05 and S4-01.
  3. The state-count Priority bonus favors ideas tied to laws present in every state (homeschool, reading, library-materials laws). Those laws are mostly enforced through schools, districts and libraries, the exact buyers the solo rubric flags as GOV. So Priority inflates R01, P02 and P03 for this founder.
  4. The corpus's "Build ease" scores the app and leaves out content, legal and data work: S8-01's attorney-reviewed contracts, P06's 52-week video library, R07's licensed descriptor data, P02's 12-state rulebook.
  5. Several corpus triggers had passed by Oct 10 2026 (see Q3), which the corpus's Sales speed could not reflect.
- **Where the solo view may be too harsh (judgment):** P04 and P01 serve large adult, card-paying audiences in reachable Facebook and Reddit communities. A price test (P01 at $29/mo; P04's hybrid "keep Outschool for discovery" pitch) could move either into the shortlist.

### Gaps
- No interview or conversion data exists in the corpus to settle the WTP disagreements, for example whether OG tutors would pay $29/mo or homeschool association directors $49/mo.
- The percentage comparison treats both scales as linear and comparable. That is a convenience, not a calibration.

---

## Key question 3: For the best 3–5, what is the narrowest sellable wedge, and which corpus claims most need fresh web verification?

### Takeaway
Shortlist, in order:
1. **S1-01 Part500 Kit:** an Apr 15 filing kit for NY independent insurance agencies.
2. **S9-04 CoverDesk:** a check-in desk for the 81 SC Option 3 associations, the fastest to first revenue but capped low.
3. **R05 SpineDesk:** special orders plus local-author consignment as a Square add-on.
4. **S2-01 ParCheck:** a Delaware franchise-tax fixer for accountants, as seasonal cash before Mar 1 2027.
5. **S4-01 FortiFile:** conditional on open Oklahoma or Louisiana grant rounds.

Each needs a competitor-density check before building, because the corpus did little or no competitor search for any of these five.

### Cited Findings

#### Switching windows: status on 2026-10-10
| Date | Trigger | Ideas | Status |
|---|---|---|---|
| Jan 1 2026 | IndieCommerce fee increase ([R05][]) | R05 | **Passed** |
| Feb 20 2026 | BookFunnel new plans; existing users grandfathered ([R06][]) | R06 | **Passed**; only new signups are affected |
| Apr 22 2026 | Amended COPPA rule full compliance ([R08][]; [P01][]; [P04][]) | R08, P01, P04 | **Passed**; now a standing obligation |
| May 25 2026 | Outschool pay-per-class ([P04][]) | P04 | **Passed** |
| Jul 31 2026 | Nerdy commits to wind down Varsity Tutors for Schools ([P04][]; [S9-02][]) | P04, S9-02 | **Passed**; displaced tutors are the remaining pull |
| Before fall 2026 | Nebraska LB 390 policies ([R01][]) | R01 | **Passed** |
| Sep–Oct 2026 | Fall fun runs ([P05][]); beginning-of-year screeners ([P02][]; [S9-02][]) | P05, P02, S9-02 | **Passed or closing** |
| Oct 1 2026 | Texas TEFA first payments ([INDEX][]) | P03, P07 | **Passed**; money now flowing |
| Oct 6 2026 | Head Start proposed-rule comments close ([P06][]) | P06 | **Passed** |
| Oct–Feb | Spring read-a-thon planning ([R02][]) | R02, P05 | Live |
| Oct–Dec | Bookstore holiday special-order crunch ([R05][]) | R05 | Live, but a poor time to switch systems (judgment) |
| Dec 2026 | Louisiana middle-of-year K–3 screener ([S9-02][]) | S9-02 | Live |
| Dec–Mar | Outfitter off-season ([S7-01][]) | S7-01 | Live |
| ~Jan 5 or Mar 1 2027 | SC Option 3 semiannual check-ins; dates vary by association ([S9-04][]) | S9-04 | Live |
| Jan 2027 | CA AB 1454 materials adoption ([P01][]) | P01, R08 | Live (district-level trigger) |
| Jan 1 2027 | Federal tax-credit scholarships start ([P07][]) | P07 | Live |
| Jan–Apr 2027 | Tax season, the first under expanded 529 rules ([P07][]); library summer-reading contracting ([R02][]) | P07, P03, R02 | Live |
| Feb 2027 | ABA Winter Institute ([R05][]) | R05 | Live |
| **Mar 1 2027** | Delaware corporate franchise tax and annual report ([S2-01][]) | S2-01 | Live; must be re-verified |
| Mar–Jun 2027 | Oklahoma hail season ([S4-01][]) | S4-01 | Partly in window |
| **Mar 31 2027** | CoConstruct stops new projects ([S8-01][]) | S8-01 | Live |
| ~Mar 2027 | LA GATOR application window, marked (verify) ([S9-02][]) | S9-02 | Unconfirmed |
| **Apr 15 2027** | NY DFS Part 500 certification ([S1-01][]) | S1-01 | Live |
| Apr 2027 | DOJ Title II web-accessibility deadline for small public entities, marked (verify) ([R03][]) | R03 | Unconfirmed |
| After Apr 2027 | Delaware LLC tax Jun 1; Chicago tip step Jul 1 2027; PTA handoff May–Aug; WI promotion gate Sep 1 2027 ([S2-01][]; [S5-01][]; [P05][]; [INDEX][]) | — | Outside the 6-month window |

#### Evidence behind the five shortlisted wedges
- **S1-01:** Apr 15 two-signature certification; 500.19(a) small entities still owe policies, MFA, an asset inventory and training; Vanta and Drata are quote-only without 23 NYCRR 500 featured; corpus price $59/mo per agency ([S1-01][]). Channels named: IIABNY, PIANY, MSP white-label, and SEO terms such as "23 NYCRR 500 small business checklist" ([S1-01][]; [NY-state][]).
- **S9-04:** 81 associations on the SCDE list; email-and-forms status quo; $35–$75 family fees; Homeschool-life at $9.95/family/yr; proposed $49–$99/mo ([S9-04][]). The plan is direct outreach to all 81 during Oct–Dec 2026 ([S9-04][]).
- **R05:** Square lacks ISBN fill-in. book by book ($29/mo) covers ISBN and invoice import but "lists no consignment or events features". Corpus says consignment is run "on paper or spreadsheets" today (unsourced). Corpus price $39/$79 ([R05][]).
- **S2-01:** Mar 1 deadline; $85,165 vs $400 worked example; firm plan $299/yr for 25 entities; channels are SEO, Show HN/Indie Hackers, startup CPAs and fractional CFOs, plus accelerator perks ([S2-01][]; [DE-state][]).
- **S4-01:** Oklahoma pays the contractor after certification; Louisiana requires a current credential binder; CompanyCam costs $63–$332/mo for small crews; the IBHS provider directory is the list; corpus price $149/mo ([S4-01][]; [OK-state][]; [LA-state][]).

### Inferences

#### Shortlist and narrowest sellable wedges (all judgment unless cited)

**1. S1-01 Part500 Kit: "April 15 Filing Kit" for NY independent insurance agencies with 1–20 staff.**
- **Ships in 4–6 weeks:**
  - an exemption wizard (500.19 category, and whether a Notice of Exemption is needed);
  - an AI-drafted policy pack (500.3 cybersecurity, 500.7 password, 500.11 third-party, incident response, data retention), with staff e-sign;
  - an MFA and asset-inventory checklist with evidence uploads (CSV or manual; no Google/M365 integration in v1);
  - a 20-minute training module with certificates;
  - the Apr 15 binder PDF, a two-signer workflow, a DFS-portal walkthrough and a receipt-number vault.
- **Cut from v1:** the incident clock, the third-party-vendor tracker and the MSP console (V2 in [S1-01][]).
- **Buyer:** the agency principal who signs the certification.
- **Price:** $49–59/mo, or about $490–590/yr billed annually up front, so post-April churn doesn't erase revenue. The corpus's $19/mo solo-producer tier looks too low (judgment); a one-time $99–149 "solo filing pack" fits a yearly job better.
- **Channels:** IIABNY/PIANY webinars in Jan–Mar; SEO pages live by December; cold email to agencies if DFS or association licensee lists are obtainable; MSPs serving agencies as resellers.
- **Timeline:** build Oct 15–Nov 30; pre-sell in December; main selling season Jan 2–Apr 15 2027.
- **Why #1:** highest ARPU among the dated-trigger ideas, an owner buyer, no child data, a single-state rulebook, and evidence that accumulates year over year.

**2. S9-04 CoverDesk: "Option 3 Check-in Desk" for South Carolina homeschool associations.**
- **Ships in 3–4 weeks:**
  - a join form with Stripe fee collection and the parent diploma/GED attestation;
  - a per-association check-in calendar with email reminders and a live "not yet submitted" list;
  - a letter generator (membership letter, wallet card, withdrawal notice, DMV letter);
  - a director dashboard with CSV/PDF export for the SCDE assurance form;
  - a free parent attendance log that produces the semiannual report.
- **Cut from v1:** SMS (avoids A2P registration), transcripts and testing.
- **Buyer:** the association director.
- **Price:** the corpus tiers (free ≤50 families, $49/mo ≤400, $99/mo ≤1,500) ([S9-04][]).
- **Channel:** call or email all 81 associations in October–December with "run your January/March check-in free, pay from the next cycle". Then push the HomeRoll family upgrade ($49–59/yr; [P03][]) through each association.
- **Realistic 6-month result:** 10–20 associations, about $0.5–1.5k MRR. The South Carolina ceiling is about $4–8k MRR, so Tennessee umbrella schools ([TN-state][]) or other umbrella models must be confirmed before investing past v1.
- **Why it is shortlisted despite the ceiling:** the fastest build, the most complete buyer list in the corpus, a dated check-in, and it turns P03's crowded consumer play into a B2B2C channel.

**3. R05 SpineDesk: "Special Orders + Consignment" add-on for Square bookstores.**
- **Ships in 4–6 weeks:**
  - special-order intake at the counter and on the web, with an optional Stripe deposit, an "arrived" email and an aging report;
  - local-author consignment: an application form with an e-signed agreement and intake fee, per-author stock linked to Square items by ISBN, and quarterly statements;
  - Square catalog sync.
- **Cut from v1:** scan-to-shelf and invoice import, which book by book already covers (integrate or coexist); events, subscriptions and the used-book desk.
- **Buyer:** the store owner.
- **Price:** $39–49/mo flat.
- **Channels:** a Square App Marketplace listing; cold email to new stores from the ABA store finder (600+ opened in 2025; [R05][]); regional bookseller shows and the Feb 2027 Winter Institute; a free "consignment program in a box" lead magnet.
- **Main risk:** book by book or Bookflow may already ship these features (verify). Weak urgency means slow, steady growth rather than a spike.

**4. S2-01 ParCheck: "Delaware Franchise-Tax Fixer" for startup CPAs, fractional CFOs and founders.**
- **Ships in 2–3 weeks:**
  - a free public two-method calculator (lead magnet);
  - a paid firm dashboard: bulk entity import, a per-entity Assumed Par Value Capital worksheet with filing-ready figures, Mar 1 and Jun 1 reminders, a receipt store and a scam-mailer explainer page.
- **Cut from v1:** the registered agent and filing on the customer's behalf (V2 in [S2-01][]).
- **Price:** firm plan $299/yr for 25 entities plus $8 per extra ([S2-01][]); founders $49/yr per entity, or a one-time $79 "filing prep" (judgment).
- **Channels:** SEO for "$85,000 Delaware franchise tax", Show HN and Indie Hackers in January, outreach to startup CPA firms ([S2-01][]).
- **Caveat:** revenue is a Dec–Feb burst with heavy post-March churn. Treat it as a cash bridge and lead list, not a core MRR engine.

**5. S4-01 FortiFile (conditional): "FORTIFIED Grant-Job Photo Checklist" for Oklahoma and Louisiana roofers.**
- **Ships in 4–6 weeks as a mobile web app:**
  - stage-gated photo checklist with GPS and timestamps;
  - evaluator packet export (PDF plus zip);
  - contractor credential binder with expiry alerts;
  - a days-to-cash grant pipeline.
- **Buyer:** the roofing owner or production manager.
- **Price:** $99–149/mo flat.
- **Channels:** cold outreach to the IBHS FORTIFIED provider directory in OK and LA, evaluator referrals and supply-house counter days ([S4-01][]).
- **Go/no-go:** build only if (a) Strengthen Oklahoma Homes or Louisiana's program has open 2027 rounds and (b) CompanyCam or IBHS doesn't already ship a FORTIFIED checklist. Otherwise it is a sub-$5k MRR niche with volatile demand. The founder also lacks roofing domain access, so an evaluator partner is a prerequisite.

#### Near-misses and what would change the call
- **P01:** promote it if 10+ OG tutors in Facebook groups pre-pay $29/mo for a per-student mastery map, decodability checker and parent progress report. That would be about twice the corpus's $15, justified by $113/hr billing ([P01][]). S9-02 would then become a Louisiana landing page on the same codebase.
- **P04:** promote it if a "keep Outschool for discovery, move your repeat families" landing page converts Outschool teachers at $29/mo. Watch chargebacks and COPPA ([P04][]).
- **R06:** test only an ARC-team manager (reliability scoring, watermarked delivery) at $9–15/mo. The Feb 2026 BookFunnel window is past and grandfathered ([R06][]).
- **S8-01:** only a document wedge fits a solo founder: a CA-compliant contract, a payment guard and a draw packet beside the contractor's existing PM tool, for $49–99/mo before Mar 31 2027. Full PM is parity work and belongs with C05 in another screening group ([S8-01][]).

### Gaps
Claims that most need fresh web verification, prioritized for the next round:

**S1-01**
- Is the Apr 15 2027 certification still due and unchanged? Is the 500.19(a) list of duties unchanged? Was there a final phase-in in Nov 2025? Check the Delta Dental amount and whether Order Express exists. All are marked (verify) in [S1-01][].
- **Competitor density:** do Vanta, Drata, Secureframe or others now support 23 NYCRR 500? Are there cheap NYDFS template kits (ComplianceForge-type packs), IIABNY/PIANY member tools, MSP bundles or carrier cyber programs? The corpus did no search here.
- Can NY DFS licensee lists (agents, brokers, mortgage brokers) be obtained for outreach? Does IIABNY grant CE credit for vendor webinars?
- Suggested queries: "NYDFS 500 small agency", "23 NYCRR 500 templates", "IIABNY cybersecurity resources".

**S9-04**
- Confirm the 81 associations on SCDE's 2026–27 list, typical member counts and each association's check-in dates.
- What software do associations use today? Homeschool-life, Jotform, custom sites, or a homeschool-association tool the corpus missed?
- Is the 50-member statutory minimum real? Are homeschoolers eligible for ESTF? How many Tennessee Category IV umbrella schools are there, and do they buy software?
- Suggested queries: "Option 3 association software", "homeschool umbrella school software".

**R05**
- What do book by book and Bookflow include now: special orders, consignment, events? Are there other Square or Shopify bookstore apps?
- What are IndieCommerce 2.0's actual new fees, and does Basil's 1% apply to all sales?
- Square App Marketplace listing requirements and timeline; ISBN metadata API licensing costs (ISBNdb, Google Books, Open Library terms).
- Suggested queries: "bookstore consignment app Square", "special orders app bookstore".

**S2-01**
- Is the **Mar 1 2027** due date unchanged, along with the $200 penalty plus 1.5%/mo? When did the LLC tax rise from $300 to $400 ([S2-01][] marks it verify)?
- Does Delaware's eCorp portal now prompt or auto-compute the lesser method? If so, the pain shrinks (judgment).
- **Competitor density:** free APVC calculators (Carta, Clerky, Stripe Atlas, Mercury, Brex) and bundled startup-compliance services (Doola, Firstbase, Every, Pilot). This is judgment and unverified.
- Re-check the corpus's "FinCEN Aug 2026 final rule exempts U.S. companies from BOI" (cited via J06) and Harbor's $99 → $159 pricing.

**S4-01**
- Are Strengthen Oklahoma Homes rounds funded for 2026–27, and when does Louisiana Fortify Homes reopen? Do Alabama, Mississippi, South Carolina or North Carolina programs exist ([S4-01][] marks these verify)?
- How many FORTIFIED-certified roofers are in OK and LA (fortifiedproviders.com)?
- Do CompanyCam, AccuLynx, JobNimbus or IBHS already offer FORTIFIED checklists or apps? Can IBHS checklist content be licensed?

**Required re-checks outside the shortlist**
- **R06 BookFunnel:** confirm the Feb 20 2026 plan change and the grandfathering are unchanged, and check for any newer promotion or price move. Check cheap ARC and delivery rivals the corpus may have missed (Prolific Works, Hidden Gems, Pubby, Gumroad or Lemon Squeezy plus a delivery app; judgment, unverified).
- **P04:** Outschool's current fee and whether the "17% to 30%" reviewer claim holds.
- **P01:** whether Project Read or LitLab have added a paid individual-tutor plan since Sep 2026.

**Method gaps**
- The rubric scores cannot be checked against real conversion. For every shortlisted wedge, a landing page plus 10–20 buyer conversations should come before the build. The corpus has no interviews for any of the five.

<!-- Reference link targets: corpus copy used for this screen (scratchpad). -->
[RUBRIC]: </home/user/independant-saas-ideas/research_notes/Solo developer SaaS opportunity shortlist/_solo_dev_rubric.md>
[INDEX]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/INDEX.md
[EDU-CSV]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/_states_edu_summary.csv
[STATE-CSV]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/_states_summary.csv
[P01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P01-science-of-reading-decodables-og-tutor-toolkit-project-read-litlab-alternative.md
[P02]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P02-third-grade-reading-plan-parent-portal-mclass-iready-companion.md
[P03]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P03-homeschool-state-compliance-records-esa-529-homeschool-planet-alternative.md
[P04]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P04-independent-kids-class-teachers-outschool-varsity-wyzant-preply-alternative.md
[P05]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P05-pto-pta-hub-diy-fun-run-read-a-thon-givebacks-memberhub-boosterthon-alternative.md
[P06]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P06-preschool-family-reading-engagement-book-lending-readyrosie-footsteps2brilliance-alternative.md
[P07]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/P07-family-screen-time-bark-qustodio-assessment-pivot-learning-spend-wallet.md
[R01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R01-school-library-compliance-catalog-follett-destiny-alternative.md
[R02]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R02-reading-challenges-readathon-beanstack-readathon-alternative.md
[R03]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R03-small-public-library-events-rooms-ils-libcal-sirsidynix-alternative.md
[R04]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R04-school-book-fairs-indie-bookstores-scholastic-alternative.md
[R05]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R05-indie-bookstore-back-office-bookmanager-basil-square-isbn-alternative.md
[R06]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R06-indie-author-hq-bookfunnel-netgalley-booksprout-alternative.md
[R07]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R07-neutral-book-content-descriptors-common-sense-media-alternative.md
[R08]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/R08-ai-decodable-reading-epic-abcmouse-raz-kids-alternative.md
[S1-01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S1-01-ny-dfs-part-500-cyber-compliance-kit.md
[S2-01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S2-01-delaware-franchise-tax-annual-report-autopilot.md
[S4-01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S4-01-fortified-roof-grant-documentation.md
[S5-01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S5-01-illinois-bipa-safe-time-clock-leave-compliance.md
[S7-01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S7-01-outfitter-guide-booking-permit-reporting.md
[S8-01]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S8-01-rebuildledger-ca-fire-rebuild-contract-draw-compliance.md
[S9-02]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S9-02-louisiana-reading-voucher-tutor-kit-steve-carter-gator.md
[S9-04]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/ideas/S9-04-sc-option3-homeschool-association-umbrella-school-admin.md
[DE-state]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/DE-delaware.md
[NY-state]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/NY-new-york.md
[SC-state]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/SC-south-carolina.md
[TN-state]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/TN-tennessee.md
[OK-state]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/OK-oklahoma.md
[LA-state]: /tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/states/LA-louisiana.md
