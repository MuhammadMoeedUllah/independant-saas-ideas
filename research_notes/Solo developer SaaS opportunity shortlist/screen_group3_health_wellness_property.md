# Solo-developer screen, group 3: health practice (E01–E08), wellness/kids activities (F01–F07) and real estate/property (H01–H06)

Scope and method: 21 idea files from the local corpus, each read in full, plus INDEX.md (sections 1–5 and 8), `_scoreboard.csv`, `_states_summary.csv` and the state files that cite these IDs (IN, TX, FL, NV, AZ, MN, NM, MS, AL). Corpus root: `/tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/`. Links such as `[E01]` point to `ideas/<file>.md` under that root (definitions at the bottom). The corpus was written Sep 24–25 2026; today is 2026-10-10. **No web search was used.** All corpus facts are third-party claims, and many come from competitor blogs (the corpus labels these). Rubric scores, kill-flag calls, wedges and prices proposed here are **my judgment** unless a source is attached.

Rubric (from `_solo_dev_rubric.md`): 1 Build scope · 2 Regulatory/liability · 3 Self-serve sale · 4 Solo-reachable distribution · 5 WTP/ARPU · 6 Gap vs cheap indie tools · 7 Urgency Oct 2026–Apr 2027 · 8 Support load/retention. Each 1–5, 5 = best for a solo founder, total /40.

---

## Q1. For each of the 21 ideas: rubric scores (/40), kill flags and the evidence behind them

### Takeaway
Only one idea scores clearly well as specced: **F06 ESA Desk (31/40)**. **H05 InspectKit (29)** is next. Every E-series idea except E05 carries the HIPAA flag, and most of the health and property ideas also carry the "feature-parity monster" flag. Four ideas improve a lot when cut down to a narrow wedge: E04 (a non-PHI med-spa compliance binder), H02 (a Florida condo records website), F03 (a recital and costume add-on) and F07 (folded into F06 as its vendor tier). The full score table is under Inferences.

### Cited Findings

**Health practice (E-series)**
- **E01 Hearth EHR (therapists).**
  - Prices: SimplePractice is $49/$79/$99 a month, and the Care Aide AI add-on costs $59. TherapyNotes Solo is $69 plus $40 for TherapyFuel AI. A solo SimplePractice Plus user with AI pays $158/mo. [E01] citing [SimplePractice pricing](https://www.simplepractice.com/pricing/).
  - Trigger: Aetna flattened rates for Alma-contracted therapists effective **Jul 15 2026**. [E01] citing [BHB, May 21 2026](https://bhbusiness.com/2026/05/21/aetna-cuts-rates-with-alma-contracted-therapists/).
  - The idea file itself says the category is crowded ("Many low-cost EHRs already exist") and that the product needs BAAs with every subprocessor. [E01]
  - The MVP list has 8 items, including telehealth, an AI scribe, payments, a client portal and claims through a clearinghouse API. [E01]
  - Market size is the corpus's own unverified estimate: 150k–250k private-practice clinicians. [E01]
- **E02 Alignly (chiro and PT).**
  - ChiroTouch publishes no prices. One BBB complainant reports a promo of $74/mo that renewed at $198+/mo.
  - ChiroTouch has 26 BBB complaints in 3 years, and 24 of them are unanswered.
  - One customer was billed $12,809.16 after cancelling. [E02] citing [ChiroTouch BBB](https://www.bbb.org/us/ca/san-diego/profile/computer-hardware/chirotouch-1126-30000841/complaints).
  - WebPT costs about $99/provider plus $500–$2,000 in setup. [E02]
  - Jane App ($54/$79/$99, AI Scribe $15) is already the "good" cheap incumbent. [E02] citing [Jane pricing](https://jane.app/pricing).
  - The file admits it is a HIPAA business-associate product. [E02]
- **E03 Bitewing (dental comms and membership plans).**
  - Weave's prices are estimates: $300–$700/mo, with renewals rising 15–25%. [E03] citing [NoShowCost](https://noshowcost.com/tools/weave-pricing).
  - Weave is the exclusive ADA-endorsed patient engagement platform for 2026. [E03]
  - The MVP depends on 10DLC two-way texting and on PMS integration: the Open Dental API, with CSV exports for Dentrix and Eaglesoft. [E03]
  - "PMS integration is the moat." [E03]
  - Membership plans run into state insurance and discount-plan rules. [E03]
- **E04 Glowchart (med spas).**
  - Boulevard costs $158/$263/$369 per location. Aesthetic Record is $15/user plus a $399 startup fee. Vagaro is $23.99. These figures come from Vagaro's own comparison, so a competitor source. [E04] citing [Vagaro, Aug 6 2026](https://www.vagaro.com/learn/best-emr-software).
  - Laws:
    - TX HB 3749 has been in force since Sep 1 2025 and requires "ordered by / administered by" records.
    - IN SB 282 took effect Jul 1 2026. It requires **registration by Jan 1 2027** and adverse-event reporting within 15 days.
    - CA SB 351 took effect Jan 1 2026.
    - NJ S2996 took effect Mar 30 2026.
    - FL SB 1728 failed on Mar 13 2026.
    - All of these come from Decoda Health's summary, and the file says to verify them against statute text. [E04] citing [Decoda Health](https://decodahealth.com/blog/new-med-spa-laws-2026).
  - Market: 10,488 US med spas in 2023, and 81% of operators run a single location. [E04] citing [AestheticHires](https://www.aesthetichires.com/med-spa-industry-statistics/).
  - A cash-only med spa "may not technically be a HIPAA covered entity". [E04]
  - The Indiana state file ranks E04 #1 in IN and suggests a "$49 one-time registration checklist" wedge. [IN state file]
- **E05 Tailwag PIMS (vets).**
  - Covetrus Pulse is estimated at $300–$500/mo, from a competitor blog.
  - Covetrus has published **no official AVImark end-of-life date**. The "sunset" is an inference. [E05] citing [PawChart](https://pawchart.io/blog/avimark-being-sunset-what-are-your-options/).
  - "HIPAA does not apply to animal medical records." [E05]
  - The MVP still includes an AI scribe, invoicing and POS through Stripe Terminal, a DEA controlled-drug log and inventory. Lab and imaging integrations come in V2. [E05]
- **E06 SkillTrack (ABA, speech and OT).**
  - The MVP is an "offline-first RBT session app". [E06]
  - CentralReach is quote-only. The strongest recent complaint is an early auto-renewal (Aug 2024), and several complaints date from 2019–2022. [E06] citing [Capterra](https://capterra.com/p/140743/CentralReach/reviews/).
  - Practices that bill insurance are covered entities, and the product holds minors' data. [E06]
- **E07 Shiftwell (home care with EVV).**
  - Two 2026 vendor sources agree on the EVV aggregator in only 11 states. [E07] citing [HHAeXchange](https://www.hhaexchange.com/state-evv-status) and [AveeCare](https://www.aveecare.com/resources/evv-vendors-by-state).
  - The MVP needs an offline-capable caregiver GPS app and certification with each state aggregator. [E07]
  - Mississippi's mandatory caregiver-app change was **Aug 31 2026**, and Alabama ended its free EVV tools on Apr 1 2025. [MS and AL state files]
- **E08 Clipboardless (clinic intake and front office).**
  - Tebra's pricing policy (effective Jul 1 2026) allows increases of up to 4.9% a year, requires 60 days' notice of non-renewal and allows early-termination fees. [E08] citing [Tebra pricing policy](https://www.tebra.com/tebra-pricing-policy).
  - IntakeQ: Forms costs $54.90/mo plus $20 per extra practitioner, and Practice Management costs $84.90 plus $30. Low-volume plans start at $29.90. The BAA is included. [E08] citing [IntakeQ pricing](https://intakeq.com/pricing).
  - "Commodity category: Many HIPAA form builders exist (IntakeQ, Jotform HIPAA…)". [E08]

**Wellness and kids activities (F-series)**
- **F01 Chairly (salons and barbers).**
  - Fresha: Independent $19.95/mo, Team $14.95 per team member, and a **20% commission on marketplace new clients** ($6 minimum). [F01] citing [Fresha pricing](https://www.fresha.com/pricing).
  - Vagaro: $30 plus $10 per calendar, with an intro price of $23.99 for 6 months. [F01] citing [Vagaro pricing](https://www.vagaro.com/pro/pricing).
  - Vagaro's Trustpilot score is 3.6/5. Reviews from Sept 2026 report frozen funds and outages. [F01] citing [Trustpilot](https://www.trustpilot.com/review/vagaro.com).
  - Chairly's planned price is **$19 solo and $49 for a studio**. [F01]
  - The file itself lists "Feature breadth / crowded category" and "Payments dependency" as risks. [F01]
  - Corpus score 22/25. It is #3 of 106 ideas, a top-3 idea in 8 states, and Bet 3 in the INDEX. [INDEX §1–2]
- **F02 OpenStudio (gyms and studios).**
  - Mindbody base plans run $139–$599 and often reach $1,000+/mo all-in. Contracts last 12–24 months and auto-renew. [F02] citing [Vibefam](https://vibefam.com/mindbody-reviews-reddit-2026/).
  - Glofox adds a surcharge of 2.9% + $0.30 on top of Stripe. [F02]
  - The "70–300%" Glofox hikes are two individual reviews, and the corpus downgraded them to anecdote. [F02 Verification]
  - Crowded challengers named in the file: PushPress (free tier), Arketa, Momence, Gymdesk. [F02]
  - The core product is Stripe Connect membership billing plus a PCI card-token migration. [F02]
- **F03 RecitalReady (dance, gymnastics, swim and martial arts).**
  - Jackrabbit Class starts at $49/mo, tiered by student count. Plus is $93 plus $169 setup, and Enterprise is $245. [F03] citing [Jackrabbit pricing](https://www.jackrabbitclass.com/pricing/).
  - Spark Membership is $99/$149 with a typical 12-month term. [F03]
  - Complaints:
    - Staff archive students to keep the per-student bill down (Mar 2024).
    - The recital module doesn't track participation cleanly (Dec 17 2024).
    - The costume module "only handles ordering" (Dec 7 2024).
    - All three from [F03] citing [Capterra Jackrabbit Dance](https://www.capterra.com/p/93349/Jackrabbit-Dance/reviews/?page=3).
  - Switching windows are June–August and January. [F03]
  - The claim that Akada is shutting down is false, and the corpus says not to use it. [F03]
- **F04 PackLeader (pet care).**
  - Gingr costs $95/$135/$150. MoeGo's mobile plans are $49/$99/$159 per van, with SMS capped at 200–1,350 messages a month. [F04] citing [GroomBoard](https://groomboard.com/blog/moego-pricing-2026-complete-breakdown).
  - One Gingr customer reports a surprise $2,000 gateway fee (Nov 2025). [F04]
  - The pitch rests on unlimited SMS plus bring-your-own processor. [F04]
- **F05 RollCall (childcare).**
  - Brightwheel and Procare are quote-only. [F05]
  - HHS ordered states to justify child-care (CCDF) spending in Jan 2026. [F05] citing [The 74](https://www.the74million.org/zero2eight/after-minnesota-fraud-allegations-hhs-orders-states-to-justify-child-care-spending/).
  - The CCDF Final Rule took effect **Jul 13 2026** and allows states to pay on attendance again. [F05] citing [ACF](https://acf.gov/occ/law-regulation/2026-ccdf-final-rule).
  - The Minnesota funding freeze was **rescinded on Jul 8 2026**. [MN state file]
  - The MVP needs a sign-in kiosk, per-state subsidy exports and a parent app. [F05]
- **F06 ESA Desk (microschools and small private schools).**
  - Texas TEFA, year 1:
    - The provider portal (run by Odyssey) opened Dec 9 2025.
    - Awards: $10k+ for private school, up to $30k for students with an IEP, $2,000 for homeschool.
    - Schools must be accredited, have operated 2+ years and give a norm-referenced test.
    - Source: [F06] citing the [Texas Comptroller](https://comptroller.texas.gov/about/media-center/news/20251125-acting-texas-comptroller-kelly-hancock-announces-final-rules-and-key-dates-for-texas-education-freedom-accounts-program-1764103747312).
  - TX state file: $1B appropriated, 274,000+ applications and 100,000+ awards. Payments arrive **Oct 1 2026 and Feb 1 2027**. "There's no incumbent default yet." [TX state file]
  - About 18 states run ESAs on three payment rails (ClassWallet, Odyssey, Step Up). The closest point tool, **GetESAPaid, costs $39/mo**. [F06] citing [GetESAPaid](https://getesapaid.com/become-an-esa-vendor).
  - Arkansas found ClassWallet "fragmented, inefficient" (Jun 2026). [F06] citing [Grand Canyon Times](https://grandcanyontimes.com/report-finds-esa-vendor-classwallet-fragmented-inefficient-and-increasingly-misaligned).
  - Arizona has 106,253 ESA students in 2026–27. [AZ state file]
  - F06 appears in 7 rows of `_states_summary.csv`, the second most of my 21 after F01's 8. [_states_summary.csv]
- **F07 LessonLedger (tutors and music teachers).**
  - Teachworks Starter is $16.49 plus $0.32 a lesson. TutorBird is $14.95 plus $4.95 per extra tutor. [F07] citing [Teach 'n Go](https://www.teachngo.com/blog/teachworks-vs-tutorbird).
  - Planned price: $12 solo. The file says "Low price gap: incumbents are already cheap", the category is crowded (Opus1, Teach 'n Go, Duet Partner, Wise), and it "could be the same codebase as F06 (a vendor tier)". [F07]

**Real estate and property (H-series)**
- **H01 DoorLedger (small landlords).**
  - Buildium: Essential $62, Growth $192, Premium $400. EFT costs $2.35/$1.35 per transaction and eSignature $5/$1 per document. [H01] citing [Buildium pricing](https://www.buildium.com/pricing/).
  - TurboTenant has a free tier, and Avail Unlimited Plus is $9/unit. [H01] citing [RenPro](https://renpro.com/turbotenant-vs-avail/).
  - A Buildium manager counted 6 price increases in 2.5 years. [H01]
  - Colorado HB25-1090 took effect Jan 1 2026. [H01]
  - The MVP needs rent ACH, trust-style ledgers and a state compliance engine covering every state's deposit and notice rules. [H01]
- **H02 BoardBinder (Florida condos and HOAs).**
  - FS 718.111(12)(g):
    - Condos with 25+ units must post records within 30 days.
    - Recordings of video-conference meetings must be posted.
    - The statute text was verified by the corpus.
    - The Jan 1 2026 deadline is still marked "(verify)".
    - Source: [H02 Verification] citing [FS 718.111](http://www.leg.state.fl.us/statutes/index.cfm?App_mode=Display_Statute&URL=0700-0799/0718/Sections/0718.111.html).
  - HOAs with 100+ parcels needed a website by Jan 1 2025. [H02] citing [FS 720.303](http://www.leg.state.fl.us/statutes/index.cfm?App_mode=Display_Statute&URL=0700-0799/0720/Sections/0720.303.html).
  - There are 373,000+ US community associations. [H02] citing [National Law Review/CAI](https://natlawreview.com/press-releases/us-surpasses-373000-community-associations-housing-model-reaches-new-heights).
  - Cheap and free tools already exist (PayHOA, HOA Start, HOA Express, and Florida-specific compliance-site vendors), and "Volunteer boards decide slowly". [H02]
  - Planned price: $29/mo for the compliance-only tier. [H02]
- **H03 StayDesk (short-term rentals).**
  - Airbnb moved PMS-connected hosts to a 15.5% host-only fee on **Oct 27 2025**. [H03] citing [Rental Scale-Up](https://www.rentalscaleup.com/airbnb-host-only-fee/).
  - Hospitable has a free tier, and paid properties cost $10–$15 each. [H03] citing [Hospitable pricing](https://hospitable.com/pricing).
  - Airbnb's API is gated to approved partners, and iCal lag causes double bookings. [H03]
  - Crowded: Hospitable, Lodgify, Hostfully, Smoobu. [H03]
- **H04 AgentPact (real-estate agents).**
  - Follow Up Boss Grow is $69/user, and the calling add-on is $39. [H04] citing [FUB pricing](https://www.followupboss.com/pricing).
  - The NAR practice changes date from **Aug 17 2024**. [H04] citing [NAR](https://www.nar.realtor/the-facts/what-the-nar-settlement-means-for-home-buyers-and-sellers).
  - The file itself names a crowded category (Wise Agent, Real Geeks, Lofty, LionDesk) and Twilio calling and texting with 10DLC. [H04]
- **H05 InspectKit (home inspectors).**
  - Spectora:
    - $109/mo or $1,090/yr.
    - Additional inspectors $99/mo.
    - **$4 per inspection** for the "Advanced" tier.
    - Websites cost $699–$1,599/yr plus $499–$799 setup.
    - Source: [H05] citing [Spectora pricing](https://www.spectora.com/pricing/).
  - Spectora added portal pop-up ads with no opt-out (Apr 2026). [H05] citing [G2](https://www.g2.com/products/spectora/reviews).
  - Buyers are solo owner-operators who pay by card. Willingness to pay is "$1,000+/yr per inspector today". [H05]
  - The winter slow season (Nov–Feb) is when inspectors rebuild templates. [H05]
  - The MVP is an "offline-first mobile report writer". [H05]
  - The market is "a few tens of thousands" of inspectors (verify), and no Reddit or InterNACHI threads could be fetched. [H05]
- **H06 UnitLedger (self-storage).**
  - Storable pricing is quote-only.
  - Easy Storage Solutions is rated 4.8/5 on 703 reviews.
  - Capterra puts entry pricing at "$9 to $45+".
  - [H06] citing [Capterra self-storage](https://www.capterra.com/self-storage-software/).
  - The core moat is gate hardware integration. The product needs per-state lien-sale rules, and "getting it wrong exposes them to wrongful-sale liability". [H06]
  - Corpus score 14, and the INDEX lists it under "put off". [INDEX §5]

**Dated triggers as of 2026-10-10 (already passed vs still ahead)**
- **Already passed:**
  - E01: Aetna/Alma rate flattening, Jul 15 2026. [E01]
  - E02: ChiroTouch server-migration outage, Apr 2026. [E02]
  - E04: TX Sep 1 2025, CA Jan 1 2026, NJ Mar 30 2026. These laws are now in force rather than upcoming. [E04]
  - E07: Mississippi caregiver-app mandate Aug 31 2026, and Alabama's free EVV tools ended Apr 1 2025. [MS and AL state files]
  - E08: Tebra's new policy took effect Jul 1 2026. Individual renewal dates still roll. [E08]
  - F01: Fresha went paid in Mar 2025. [F01]
  - F03: the June–August switch window. [F03]
  - F05: the HHS freeze (Jan 2026), the Minnesota rescission (Jul 8 2026) and the CCDF rule (Jul 13 2026). [F05], [MN state file]
  - F06: the first TEFA payment (Oct 1 2026) and the Arizona Treasurer's RFP responses (Jul 29 2026). [F06], [TX state file]
  - H01: Colorado HB25-1090, Jan 1 2026. [H01]
  - H02:
    - FL HOA website deadline, Jan 1 2025.
    - FL condo website deadline, Jan 1 2026 (verify).
    - SIRS deadline, Dec 31 2025.
    - DBPR annual report, Oct 1 2026. The next one falls Oct 1 2027, outside the window.
    - AZ HB 2397, Sep 12 2026 (enactment unconfirmed).
    - Source: [H02].
  - H03: the Airbnb fee change (Oct 27 2025) and the World Cup hosting surge (summer 2026). [H03]
  - H04: the NAR practice changes, Aug 17 2024. [H04]
  - H05: the Spectora portal ads, Apr 2026. [H05]
- **Still ahead, inside Oct 2026–Apr 2027:**
  - F06: Tennessee scholarship payout Oct 15 2026, and the second TEFA payment **Feb 1 2027**. [INDEX §3], [TX state file]
  - H05: Fannie/Freddie UAD 3.6 becomes mandatory **Nov 2 2026**. This affects appraisers, not inspectors. [H05]
  - H05: the inspector slow season, Nov–Feb. [H05]
  - E04: Indiana med-spa registration deadline **Jan 1 2027**. [E04], [IN state file]
  - F03: the January studio switch window. [F03]
  - H01: the Jan 1 year-end/1099 migration window. [H01]
  - H04: teams reset their tech stack in January. [H04]
- **Outside the window:** H03's Maryland county lodging-tax collection starts **Jul 1 2027**. [H03]

### Inferences

#### Full score table (judgment; evidence above)

| ID | Product | Build | Reg | Self-serve | Distrib | WTP | Gap | Urgency | Support | **/40** | Kill flags (bold = hard) | Why, in one line |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **F06** | ESA Desk | 4 | 3 | 5 | 4 | 4 | 3 | 5 | 3 | **31** | (partial: rules churn across 18 programs, but an error means a rejected invoice, not legal liability) | Founder pays by card, Feb 1 2027 TEFA installment, file-based (no API), GetESAPaid at $39 proves people pay |
| **H05** | InspectKit | 2 | 4 | 5 | 4 | 4 | 3 | 4 | 3 | **29** | **Offline-first mobile app**; parity on templates (partial) | Solo card buyers paying $1,090–$3,389/yr to Spectora; ads/fee anger; Nov–Feb slow season; offline report-writing is the build risk |
| F03 | RecitalReady | 2 | 4 | 4 | 4 | 4 | 2 | 3 | 3 | **26** | **Payments core** (tuition runs); parity (partial) | Good buyer, but owners won't move tuition billing mid-season; the recital/costume module is the separable wedge |
| F07 | LessonLedger | 4 | 4 | 5 | 4 | 1 | 1 | 3 | 4 | **26** | **Crowded with cheap tools** | Easy to build and sell, but $12–15 ARPU against $15 incumbents; use only as F06's vendor tier |
| E04 | Glowchart | 2 | 2 | 4 | 3 | 4 | 3 | 4 | 3 | **25** | HIPAA expected (partial); state legal rules (partial); **parity** (booking + charting + POS) | Full med-spa suite is a parity build against Vagaro/Boulevard; the non-PHI compliance binder, timed to the Jan 1 2027 IN deadline, is the play |
| F02 | OpenStudio | 2 | 3 | 3 | 4 | 5 | 2 | 3 | 3 | **25** | **Payments core**; **crowded challengers**; parity (partial) | High ARPU, but the product *is* membership billing plus card-token migration; PushPress (free) and Gymdesk already fill the gap |
| F01 | Chairly | 3 | 4 | 5 | 4 | 2 | 1 | 3 | 2 | **24** | **Crowded with cheap tools**; payments/no-show deposits (partial); SMS at scale (partial) | Easiest buyer in the set, but $19 ARPU against $19.95–$30 incumbents plus GlossGenius/Square; high support per dollar |
| H02 | BoardBinder | 3 | 3 | 2 | 4 | 3 | 2 | 3 | 4 | **24** | Committee buyer (partial); cheap competitors (partial) | Statute forces the purchase and public lists exist, but volunteer boards are slow and $29 is low; sell the compliance site to CAM firms |
| E08 | Clipboardless | 4 | 1 | 4 | 3 | 3 | 2 | 3 | 3 | **23** | **HIPAA**; **crowded** (IntakeQ, Jotform HIPAA) | The simplest health build, but a commodity category with a BAA obligation |
| F04 | PackLeader | 2 | 4 | 4 | 3 | 3 | 2 | 2 | 3 | **23** | **Crowded**; SMS at scale ("unlimited SMS" is the pitch); payments (partial) | Facilities need full operations parity; groomer tools are cheap and plentiful |
| F05 | RollCall | 2 | 2 | 4 | 4 | 3 | 2 | 3 | 2 | **22** | State subsidy rules (partial); parity (parent app); crowded (partial) | Urgency softened (MN freeze rescinded Jul 8 2026); per-state subsidy exports and a parent app make it a parity build |
| H04 | AgentPact | 2 | 3 | 4 | 4 | 3 | 1 | 2 | 3 | **22** | **Crowded**; **telephony/SMS core**; parity (CRM) | The NAR trigger is two years old; transaction tools already cover agreement e-sign |
| E01 | Hearth EHR | 2 | 1 | 4 | 4 | 3 | 2 | 2 | 3 | **21** | **HIPAA**; **parity**; **crowded** | Good channels (r/therapists), but a full EHR with telehealth and an AI scribe on PHI |
| E02 | Alignly | 2 | 1 | 3 | 3 | 4 | 2 | 2 | 3 | **20** | **HIPAA**; **parity** | Jane App already serves cash practices; migrating ChiroTouch on-prem data needs white-glove help |
| E03 | Bitewing | 2 | 1 | 2 | 3 | 5 | 3 | 2 | 2 | **20** | **HIPAA**; **SMS/10DLC core**; parity (PMS integration) | Great ARPU ($149), but PMS integrations, texting and demo-driven buyers |
| E05 | Tailwag PIMS | 1 | 3 | 2 | 2 | 5 | 3 | 2 | 2 | **20** | **Parity monster**; hardware/POS and lab integrations (partial) | No HIPAA, but a PIMS is a full clinic system; the AVImark "sunset" is unofficial |
| H03 | StayDesk | 1 | 2 | 5 | 4 | 3 | 1 | 2 | 2 | **20** | **Parity** (channel manager, Airbnb API gated); **payments**; **crowded**; tax determinations | Hospitable's free tier plus double-booking support risk |
| E06 | SkillTrack | 1 | 1 | 3 | 3 | 5 | 2 | 2 | 2 | **19** | **HIPAA**; **offline-first app**; **parity** | Every flag the rubric names for clinical field apps |
| H01 | DoorLedger | 1 | 1 | 4 | 4 | 3 | 1 | 3 | 2 | **19** | **Payments core**; **50-state legal rules**; **parity**; **crowded free tools** | Free TurboTenant/Avail/Baselane-type tools plus trust accounting |
| E07 | Shiftwell | 1 | 1 | 2 | 3 | 5 | 3 | 2 | 1 | **18** | **HIPAA**; **offline mobile app**; **50-state EVV rules**; SMS broadcast; **parity** | State-aggregator certification work in each state is beyond a solo founder |
| H06 | UnitLedger | 1 | 1 | 3 | 3 | 5 | 2 | 1 | 2 | **18** | **Payments core**; **hardware (gates)**; **50-state lien rules**; **parity** | The corpus already says "put off" |

#### HIPAA and non-PHI wedges for the E-series (judgment)
- **Why HIPAA kills these ideas for a solo founder:** the corpus treats HIPAA as "a few hundred dollars a month" plus a pen test, as in [E01] and [E08]. The binding constraints for one person are elsewhere:
  - breach liability;
  - a BAA with every subprocessor, including the AI model provider (the corpus routes this through AWS Bedrock/Transcribe);
  - security questionnaires from buyers;
  - the fact that every HIPAA idea here is also a parity build.
- **Non-PHI wedges found:**
  - **E04 (best).** A compliance binder holding only clinician, protocol and agreement data, with adverse events logged under internal case IDs. Details in Q3.
  - **E01.** The "Go-direct kit" (V2 item 9): a tracker for CAQH, NPI and payer applications plus a payer-rate comparison. It holds clinician data, not client data. It overlaps J06 LicenseLedger, and its ARPU and retention look weak because use is close to one-time.
  - **E06.** A tracker for BCBA trainee fieldwork hours and RBT supervision, holding supervisee data only. Unverified, but cheap tracker apps probably already exist.
  - **E07.** A caregiver credential file (TB tests, background checks, training hours), holding employee data only. It is close to generic HR tooling, so willingness to pay is likely low.
  - **E08.** A Good Faith Estimate builder that renders client-side and stores templates but no patient rows. The architecture is plausible, but standalone willingness to pay is unproven. The "Tebra non-renewal calculator" is a lead magnet, not a product.
  - **E02 and E03.** No clean non-PHI wedge. Any patient list held by a covered dental or chiro office is PHI.
  - **E05.** HIPAA doesn't apply. A standalone controlled-drug log is possible, but it carries DEA record-keeping liability and vets are hard to reach.

### Gaps
- No primary-source check was made of any price or law in this pass (web search was barred). Several price inputs come only from competitor blogs:
  - Weave (NoShowCost)
  - Mindbody and Glofox (Vibefam)
  - MoeGo (GroomBoard)
  - Teachworks and TutorBird (Teach 'n Go)
  - WebPT and Prompt (SPRY)
  - Pulse (PawChart)
  - Boulevard and Aesthetic Record (Vagaro)
- For several ideas the corpus never looked for cheap indie competitors (H05, F03 recital tools, E04 compliance tools, F06 ESA tools beyond GetESAPaid). My "Gap" scores for these rest on my own knowledge and need checking.
- Market-size figures are mostly marked estimates in the corpus (E01, E02, E03, E05, E06, E07, E08, F01–F05, F07, H01, H03–H06). Only E04 (med-spa count), F06 (the National Microschooling Center's student estimate) and H02 (CAI association count) carry sourced figures.

---

## Q2. Where the corpus score (/25) and the solo-developer score (/40) disagree, and why

### Takeaway
The corpus rewards big markets, a large price gap and high pain. The solo rubric punishes payments, HIPAA, parity builds and crowding with cheap tools, and it does not care about total market size beyond roughly 200 customers. That flips the order: **F01 and F02**, the corpus's #1 and #2 of these 21 (and Bet 3 in the INDEX), drop to the middle. **F06, H05 and F07**, which the corpus scored 16–18, rise to the top.

### Cited Findings
- The corpus scores Pain, Price gap, Build ease, Sales speed and Market size, each 1–5, for a total out of 25. Priority adds 0.1 for each state that ranks the idea in its top 3. [INDEX intro]
- F01 scored 22: Pain 4, Price gap 4, Build ease 4, Sales speed 5, Market size 5. INDEX Bet 3 is "an owner-operator booking app with fast card sales (F01, then F02)". [F01], [INDEX §2]
- F02 scored 20, with Pain 5 and Price gap 5. The file lists "Crowded challengers (PushPress free tier, Arketa, Momence, Gymdesk)" as a risk. [F02]
- H05 scored 18, with Market size 2 and Sales speed 5. [H05]
- F06 scored 17, with Price gap 3 and Market size 3. [F06]
- F07 scored 16, with Pain 2 and Price gap 2. [F07]
- H01 scored 18, with Market size 5 and Build ease 2. [H01]
- The E-series HIPAA cost is framed as "a few hundred dollars a month… plus a few thousand dollars a year". [E01], [E02], [E08]
- The INDEX's "put off" list (14/25 or below) includes H06. [INDEX §5]

### Inferences

| ID | Corpus /25 (rank in group) | Solo /40 (rank) | Direction | Main reason for the gap |
|---|---|---|---|---|
| F01 | 22 (1) | 24 (7–8) | ↓↓ | The corpus's Market size 5 and Sales speed 5 are real, but the solo rubric adds ARPU (a $19 plan means 500+ customers for $10k MRR), a crowded cheap field (Fresha $19.95, Vagaro intro $23.99, GlossGenius, Square, Booksy) and the support cost of deposits, no-shows and SMS. A good market, but a bad fit for one person who needs revenue fast. |
| F02 | 20 (2) | 25 (5–6) | ↓ | Price gap 5 is real ($1,000+/mo Mindbody bills), but the product's core value is recurring payments plus card-token migration (payments flag). Challengers with free tiers already exist. Studios also switch around auto-renew dates, which is slow. |
| H01 | 18 (3–7) | 19 (18–19) | ↓↓ | Market size 5 drives the corpus score. The solo view sees four hard flags: rent payments and trust funds, 50-state deposit and notice law, accounting parity, and free competitors. |
| E01, E02, E08 | 18 each | 21, 20, 23 | ↓ | The corpus prices HIPAA as an infrastructure cost. Solo, it is a liability and sales-friction cost on top of a parity build (E01, E02) or a commodity category (E08). |
| H05 | 18 (3–7) | 29 (2) | ↑↑ | The corpus docks it for Market size 2. A solo founder needs about 170–200 inspectors at $49–59, and the buyers are solo, pay by card and are angry about ads and the $4 fee. The real solo risk is the offline-first build, which the corpus scored as Build ease 4. I would score it lower. |
| F06 | 17 (8–13) | 31 (1) | ↑↑ | The corpus docks Price gap (spreadsheets are free) and Market size. The solo rubric rewards a dated window (Feb 1 2027 TEFA installment), a founder who decides alone, the absence of any API, and the absence of payments or HIPAA. |
| F07 | 16 (14–18) | 26 (3–4) | ↑ (as a tier only) | Easy to build and sell. ARPU and crowding kill it standalone, but it adds cheap reach for F06 (tutors and therapists as ESA vendors). |
| F03 | 17 | 26 | ↑ | Self-serve owners and reachable Facebook groups. The recital/costume module avoids the billing core. |
| E04 | 17 | 25 (wedge ~29) | ↑ | The corpus scored it as a full suite. Cut to compliance-only, the build is small and the Indiana Jan 1 2027 deadline is inside the window. |
| H02 | 17 | 24 (wedge ~27) | ↑ | The statute forces the purchase and the compliance-only build is small. The solo score is held down by committee buying and $29 ARPU. |
| E05, E06, E07, H03, H04, H06 | 14–16 | 18–22 | ≈ | Both views say no. The solo reasons are harder: parity, offline apps, aggregator certification, gated channel APIs, telephony, hardware and lien law. |

- **Pattern (judgment):** the corpus's "Build ease" ignores *switching parity*. F01, F02, H01 and H03 are buildable, but a customer will not move until payments, migration and every daily workflow work, and that is what makes them parity monsters. Its "Market size" also overweights large pools that are already crowded with cheap tools (F01, H01, H03, H04).

### Gaps
- The corpus gives no sub-scores for urgency or support load, so these disagreements partly reflect new criteria rather than different readings of the same evidence.
- I could not check whether the corpus's rationale for F01's state priority (8 state top-3s) reflects real salon density or just repetition across state files.

---

## Q3. The best 3–5 for this founder: the narrowest sellable wedge, and the corpus claims that most need fresh web verification

### Takeaway
Shortlist, in order:
1. **F06 + F07 "ESA Get-Paid Ledger"**
2. **H05 "AI report writer for solo inspectors"**
3. **E04 "Med-spa compliance binder" (non-PHI, time-boxed to Indiana's Jan 1 2027 deadline)**
4. **H02 "Florida condo records website + proof log"**, sold through small management (CAM) firms
5. **F03 "Recital & costume manager" add-on** (a conditional probe, because the evidence is thin)

Every wedge stays out of payments, PHI and parity builds. Each one's survival depends on a few unverified claims, listed below.

### Cited Findings
- F06:
  - TEFA has "no incumbent default yet", and schools must reconcile the Oct 1 2026 and Feb 1 2027 installments against their own tuition ledgers. [TX state file]
  - The TX file suggests offering "TEFA installment reconciliation free through the Feb 1 2027 payment". [TX state file]
  - GetESAPaid sells an invoice generator, rejection checker and audit binder for $39/mo or $390/yr. [F06] citing [GetESAPaid](https://getesapaid.com/become-an-esa-vendor)
  - ClassWallet and Odyssey have no public APIs, so the product generates files and guided upload steps. [F06]
  - Arizona's state file proposes a "ClassWallet invoice and receipt pack… at $19–39/mo" for tutors, therapists and microschools. [AZ state file]
- H05:
  - Worked savings example: Spectora annual ($1,090) plus Base Website ($699) plus Advanced on 400 inspections ($1,600) comes to about $3,389/yr, against $590/yr for InspectKit. [H05]
  - State forms: Texas TREC REI 7-6, and Florida's OIR-B1-1802 wind-mitigation and 4-point forms ("verify current form versions"). [H05]
  - Florida's My Safe Florida Home program funds free wind-mitigation inspections and grants of up to $10,000. [FL state file] citing [MSFH](https://mysafeflhome.com/)
- E04:
  - Indiana SB 282 requires registration by Jan 1 2027, a responsible practitioner and adverse-event reporting within 15 days. [E04], [IN state file]
  - Texas requires "ordered by / administered by" records and written delegation protocols. [E04] citing [Holland & Knight](https://www.hklaw.com/en/insights/publications/2025/06/texas-governor-signs-bill-into-law-increasing-regulations)
  - New Jersey requires service-specific collaborating-physician agreements. [E04]
  - Planned partners: medical-director-as-a-service and good-faith-exam (GFE) providers such as Qualiphy and Spakinect. [E04]
- H02:
  - The plan has a compliance-only tier at $29/mo per association, and a $2/unit/mo plan for management firms. [H02]
  - Planned lead magnet: a free "Is your condo website compliant?" scanner. [H02]
  - Channels: Florida CAI chapters, condo attorneys, board-certification education providers, and milestone-inspection engineers. [H02]
  - "Many associations use whatever software their CAM firm uses." [H02]
- F03:
  - Capterra complaints say the Jackrabbit Dance costume module "only handles ordering" and the recital module "doesn't track participation status cleanly" (Dec 2024). [F03]
  - V2 item 7 specifies costume sizes, fees billed to family ledgers, checkout/return inventory, and a quick-change conflict checker. [F03]

### Inferences

#### Wedge scores (judgment, same rubric)

| Rank | Wedge | Build | Reg | Self | Dist | WTP | Gap | Urg | Supp | /40 | Evidence confidence |
|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | F06+F07 ESA Get-Paid Ledger | 5 | 3 | 5 | 4 | 4 | 3 | 5 | 3 | **32** | Medium-high (state sources, live competitor) |
| 2 | H05 AI report writer (online-first, offline capture queue) | 3 | 4 | 5 | 4 | 4 | 3 | 4 | 3 | **30** | Medium (Spectora prices from its own page; competitor density unknown) |
| 3 | E04 Med-spa compliance binder (non-PHI) | 5 | 2 | 4 | 3 | 4 | 3 | 4 | 4 | **29** | Medium-low (laws from one vendor summary; IN market size unknown) |
| 4 | H02 Florida condo records website + proof log | 5 | 3 | 3 | 4 | 3 | 2 | 3 | 4 | **27** | Medium-high on law, low on willingness to pay and competitors |
| 5 | F03 Recital & costume manager (probe) | 5 | 5 | 4 | 4 | 3 | 3 | 4 | 2 | **30** | Low (two Dec 2024 reviews; seasonality is my judgment) |

#### 1. F06 + F07: "ESA Get-Paid Ledger"
- **What ships in 4–6 weeks:**
  - A family roster tagged by payer: ESA program, award amount and the parent's remaining share.
  - A **split-payer tuition ledger**, with the ESA portion and parent portion tracked per installment.
  - A **TEFA installment reconciliation** view: expected vs received per student, with aging. It is aimed at the Feb 1 2027 installment.
  - An **itemized invoice and receipt generator** for each payment rail (Odyssey TX/IA/UT; ClassWallet AZ/AR/TN), output as PDF and CSV. A pre-submit field checker uses Claude to flag missing service dates, IDs and line-item detail.
  - A **compliance binder**: accreditation certificate, operating-history proof, test roster and attendance, with expiry reminders.
  - A parent statement link.
- **Left out:** no portal integration, no payment processing (parents pay the remainder through the school's existing tools or an optional Stripe Payment Link) and no SIS.
- **Who buys:**
  - Texas: heads of small accredited private and faith-based schools receiving TEFA.
  - Arizona and Florida: microschool founders.
  - Vendor tier: tutors, music teachers and enrichment providers, which is the F07 market.
- **Price (judgment):**
  - School: $79/mo up to 100 students, $149 up to 300.
  - Vendor: $19–29/mo, set close to GetESAPaid's $39 so the full ledger looks cheap by comparison.
  - About 130 schools gets to roughly $10k MRR.
  - I would charge from day one with an annual-prepay discount, rather than the "free through Feb 1" idea in the TX state file, because the founder needs revenue fast.
- **Channel:**
  - TEFA provider and parent Facebook groups, and "Arizona ESA Families".
  - Texas Private Schools Association, the National Microschooling Center and KaiPod.
  - SEO pages: "TEFA vendor invoice", "ClassWallet invoice rejected", "Odyssey ESA provider payment".
  - Cold email to approved-vendor or school directories, if Odyssey or ClassWallet publish them (verify).
- **What most needs web verification:**
  1. **How TEFA money reaches schools.** Does Odyssey pay schools directly in installments? What do schools submit? Does the Odyssey vendor portal already give reconciliation reports or invoices? If it does, the wedge shrinks to multi-rail vendors only.
  2. **Whether the Oct 1 2026 and Feb 1 2027 payment dates are correct**, and the Tennessee Oct 15 2026 payout.
  3. **Competitor density.** GetESAPaid's current price, features and traction. Whether FACTS, TADS, Smart Tuition, Blackbaud Tuition, Sycamore or Brightwheel (schools) added TEFA/ESA split billing in 2026. Any other indie ESA vendor tools the corpus missed.
  4. **The accreditation and 2-year operating rule.** It may exclude most Texas microschools in year 1, which would make Texas buyers accredited private schools that already use FACTS-type tools.
  5. **Payment-rail churn.** Arizona's Treasurer procurement (responses were due Jul 29 2026) and Arkansas's ClassWallet review. A new administrator would change invoice formats, which is both a risk and an update-driven sales trigger.
  6. **Political and litigation risk** to TEFA and the Arizona ESA.

#### 2. H05: "AI report writer for solo home inspectors"
- **What ships in 4–6 weeks (scope cut hard):**
  - A template and comment library imported from a Spectora export or PDF, mapped by AI.
  - A phone PWA for capture: photos with annotation plus voice notes. Offline it **only queues** capture in IndexedDB and syncs later. This avoids building fully offline-first report editing, which is the rubric's kill flag.
  - Claude vision and text drafts each defect narrative "in the inspector's voice", with severity and the recommended trade, and the inspector approves every line.
  - Branded web and PDF reports with **no third-party ads**.
  - A pre-inspection agreement e-signature and a pay-to-release link through Stripe (inspector's own account).
- **Deferred:** scheduling, CRM, websites, multi-inspector dispatch.
- **Fallback probe (cheaper to test):**
  - A Florida **wind-mitigation (OIR-B1-1802) and 4-point form filler** with photo pages, at $29–39/mo.
  - Florida insurance inspections are high-volume standardized forms, and My Safe Florida Home funds them.
  - Whether anyone pays for a standalone form tool is **unverified** (my judgment).
- **Who buys:** solo inspectors in Texas and Florida first. Both have state forms and large licensee pools, per [H05].
- **Price:** $49–59/mo or $490–590/yr, with free template migration. About 170–200 inspectors gets to roughly $10k MRR.
- **Channel:**
  - r/homeinspectors and inspector Facebook groups.
  - An InterNACHI member-benefit listing.
  - Cold email to Texas TREC and Florida DBPR licensee lists, if they can be downloaded (verify).
  - "Spectora ads in client portal" search intent.
  - Timed to the **Nov–Feb slow season**.
- **What most needs web verification:**
  1. **Cheap competitor density the corpus missed.** HomeGauge, Palm-Tech, Home Inspector Pro, Horizon, Tap Inspect, ReportHost, Inspector Toolbelt, and any AI-first report writers launched in 2025–26: their prices and whether they already include AI narratives.
  2. **Spectora's current state.** Whether the portal ads and lack of opt-out persist after the April 2026 complaints, and whether $109/mo and the $4 Advanced fee are unchanged.
  3. **Sentiment on r/homeinspectors and InterNACHI**, which the corpus could not fetch.
  4. **Inspector count and licensee-list availability** in Texas and Florida.
  5. **Current versions** of TREC REI 7-6 and OIR-B1-1802, and the 4-point form standards insurers expect.
  6. **Whether inspectors write reports on-site or at the office.** This decides whether the online-first scope cut is acceptable.

#### 3. E04: "Med-spa compliance binder" (non-PHI)
- **What ships in 4–6 weeks:**
  - A practice profile, plus a responsible-practitioner and medical-director roster.
  - A provider license and certification expiry tracker.
  - A **protocol and standing-order library** with medical-director e-signature and version history (Texas delegation protocols).
  - A **collaborating-agreement tracker** for each service (New Jersey S2996).
  - An **Indiana SB 282 registration checklist and data export**.
  - An **adverse-event log keyed by internal case ID** (no patient identifiers) with a 15-day countdown.
  - A medical-director chart-review sampling log by chart ID.
  - A one-click audit binder PDF.
  - Templates must be attorney-reviewed, with "not legal advice" terms.
- **Left out:** no booking, no charting, no photos, no payments.
- **Who buys:** owner-operator injectors (NP, RN or PA) and physician owners. Indiana first because of the deadline, then Texas, which has more spas and laws already in force, then New Jersey.
- **Price:**
  - $49–79/mo per location.
  - The IN state file's "$49 one-time registration kit" can be the entry offer, upselling to the subscription.
- **Channel:**
  - Medical-director-as-a-service and GFE providers, which each serve many spas.
  - AmSpa events.
  - Injector Facebook and Instagram groups.
  - SEO: "Indiana med spa registration" and "Texas HB 3749 compliance".
- **Timing risk:** Jan 1 2027 is about 12 weeks away, so the product would have to ship by early November to sell into the Indiana deadline.
- **What most needs web verification:**
  1. **The statute text of IN SB 282.** Who registers (entity or practitioner), whether registration repeats each year (this decides retention), and whether adverse-event reports need patient identifiers. If they do, the log becomes PHI.
  2. **How many Indiana med spas, IV bars and GLP-1 clinics are covered.**
  3. **The details of TX HB 3749 / TMB Rule 169.28**, and whether NJ S2996 has an effective date.
  4. **Whether Florida refiles its med-spa bill in the 2027 session.**
  5. **Existing compliance offerings:** AmSpa toolkits, Moxie, GFE vendors' protocol tools, and compliance features in Aesthetic Record and Boulevard. Also compliance consultants' prices.

#### 4. H02: "Florida condo records website + proof log"
- **What ships in 4–6 weeks:**
  - A hosted statutory site for each association: a public page plus an owner login, with owners provisioned by CSV.
  - A **document checklist mapped to FS 718.111(12)(g) and 720.303** with a 30-day upload clock.
  - A **tamper-evident posting log** recording hash, timestamp, uploader and version.
  - Meeting-notice posting plus video link or recording upload.
  - A deadline tracker for SIRS, milestone inspections, the annual DBPR report and board certification.
  - The free "is your site compliant?" URL scanner as lead capture.
- **Left out:** no assessments or payments, no e-voting, no accounting.
- **Who buys:** first, owners of **small management (CAM) firms** with 5–60 associations, because one decision covers many sites. Second, treasurers of self-managed condos.
- **Price (judgment):**
  - $39/association/mo, or a CAM portfolio plan of about $299/mo for up to 15 associations.
  - Roughly 35 CAM firms or 250 associations gets to $10k MRR.
- **Channel:**
  - Florida CAI chapters and condo attorneys.
  - Direct mail and email from public DBPR and Sunbiz records, if usable (verify).
  - SEO: "Florida condo website requirements 25 units".
- **What most needs web verification:**
  1. **The Jan 1 2026 condo website deadline**, which the corpus itself flagged "(verify)".
  2. **Penalties and enforcement for non-compliance.** My recollection, not verified, is that the 2024 Florida law added stronger penalties for records violations.
  3. **Prices of Florida compliance-website vendors**, and HOA Express or PayHOA free tiers.
  4. **Whether DBPR offers a downloadable list of condo associations** with unit counts.
  5. **How many small CAM firms operate in Florida**, and how they buy.
  6. **Bills in Florida's 2027 session** that could change the rules.

#### 5. F03: "Recital & costume manager" add-on (conditional probe)
- **What ships in 4 weeks:**
  - A parent measurement form for each dancer.
  - Costume assignment for each routine, with auto-built vendor order sheets.
  - **Costume fee CSV export** for Jackrabbit and iClassPro family ledgers, so the product never touches payments.
  - Distribution and return checkout.
  - A recital lineup builder with a **quick-change conflict checker**.
  - Printable programs and backstage rosters.
- **Buyer:** dance studio owners and office managers.
- **Price (judgment):** $39/mo or about $299 per season.
- **Channel:** dance studio owner Facebook groups, the Dance Studio Owners Association, Dance Teacher Summit, and costume vendors as referral partners.
- **Why only a probe:**
  - The evidence is two Capterra reviews from Dec 2024.
  - Retention is seasonal.
  - I am **assuming, not verifying,** that studios place costume orders in the fall and winter for spring recitals. If so, the window is open right now.
- **What most needs web verification:**
  1. **When costume orders are actually placed.**
  2. **What the recital and costume modules do in 2026** in Jackrabbit, DanceStudio-Pro, iClassPro and Akada, and whether indie recital or costume apps exist.
  3. **Jackrabbit's current prices.**

#### Not shortlisted despite corpus prominence (judgment)
- **F01 and F02** stay out. They are good markets, but a solo founder would compete on price in crowded categories while carrying payments and SMS support.
- **One F01 sub-wedge is worth a later look:** the V2 "suite-owner mode", in which a salon-suite landlord manages 20–60 renters. It brings higher ARPU and one decision-maker, but it still involves rent payments.
- **H03 has a Florida tourist-development-tax desk variant** (from the FL state file): about $15–25/property, where Avalara MyLodgeTax is the incumbent. It is held back by tax-determination liability.

### Gaps
- Without web search I could not confirm any wedge's standalone willingness to pay. Each wedge needs 10–20 buyer conversations or a pre-sale page before building.
- No public directory of TEFA or ClassWallet vendors, Texas or Florida inspector licensees, Florida condo associations or Indiana med spas was confirmed. Cold outreach for every shortlisted wedge depends on these lists.
- The corpus gives no data on how often prospects switch, or how fast they churn, for any of the five wedges.
- The incumbent's reaction is unknown: Odyssey or ClassWallet adding vendor tools, Spectora removing ads, or AmSpa bundling compliance.

[E01]: ideas/E01-therapy-ehr-simplepractice-therapynotes-alternative.md
[E02]: ideas/E02-chiro-pt-ehr-chirotouch-webpt-alternative.md
[E03]: ideas/E03-dental-comms-membership-weave-alternative.md
[E04]: ideas/E04-med-spa-compliance-ehr-zenoti-boulevard-alternative.md
[E05]: ideas/E05-vet-pims-avimark-pulse-ezyvet-alternative.md
[E06]: ideas/E06-aba-speech-ot-practice-centralreach-alternative.md
[E07]: ideas/E07-home-care-agency-evv-wellsky-axiscare-alternative.md
[E08]: ideas/E08-clinic-intake-scheduling-payments-tebra-intakeq-alternative.md
[F01]: ideas/F01-salon-barber-booking-vagaro-fresha-alternative.md
[F02]: ideas/F02-gym-studio-mindbody-glofox-alternative.md
[F03]: ideas/F03-kids-activities-dance-gym-martial-arts-jackrabbit-alternative.md
[F04]: ideas/F04-pet-grooming-boarding-daycare-gingr-moego-alternative.md
[F05]: ideas/F05-childcare-subsidy-attendance-brightwheel-procare-alternative.md
[F06]: ideas/F06-microschool-private-school-esa-billing-facts-alternative.md
[F07]: ideas/F07-tutoring-music-lessons-esa-ready-mymusicstaff-teachworks-alternative.md
[H01]: ideas/H01-small-landlord-pm-appfolio-buildium-alternative.md
[H02]: ideas/H02-hoa-condo-florida-website-compliance-vantaca-townsq-alternative.md
[H03]: ideas/H03-short-term-rental-pms-guesty-hostaway-alternative.md
[H04]: ideas/H04-agent-crm-buyer-agreement-follow-up-boss-boldtrail-alternative.md
[H05]: ideas/H05-home-inspection-report-software-spectora-alternative.md
[H06]: ideas/H06-self-storage-management-storable-sitelink-alternative.md
[H02 Verification]: ideas/H02-hoa-condo-florida-website-compliance-vantaca-townsq-alternative.md
[F02 Verification]: ideas/F02-gym-studio-mindbody-glofox-alternative.md
[INDEX §1–2]: INDEX.md
[INDEX §3]: INDEX.md
[INDEX §5]: INDEX.md
[INDEX intro]: INDEX.md
[IN state file]: states/IN-indiana.md
[TX state file]: states/TX-texas.md
[FL state file]: states/FL-florida.md
[AZ state file]: states/AZ-arizona.md
[MN state file]: states/MN-minnesota.md
[MS and AL state files]: states/MS-mississippi.md
[_states_summary.csv]: _states_summary.csv
