# Validation of two solo-developer wedges: F06 "ESA Get-Paid Ledger" and I03 "WildApricot escape kit" (research date 2026-10-10)

**How these notes were made:**
- About 35 web searches plus one GitHub repository search.
- Every direct page fetch failed in this environment. Even support.withodyssey.com and getesapaid.com returned DNS errors (ENOTFOUND). **So every web finding below comes from search-engine result summaries, not from reading the pages.** Treat exact figures as "per search summary".
- Facts cited as "[screen]" or "[corpus]" come from the earlier screen notes or the corpus idea files and were not re-verified unless stated.
- Paths: screen notes = `screen_group3_health_wellness_property.md` and `screen_group4_professional_nonprofit_compliance.md`; corpus = `SaaS-Opportunity-Research/ideas/F06…`, `F07…`, `I03…`.
- The founder: one developer building with Claude, no sales team, needs revenue soon. Scoring uses `_solo_dev_rubric.md` (8 criteria, /40).

---

## Q1. F06 trigger check: TEFA's 2026–27 status, how the money reaches schools and vendors, vendor approval and counts, payment dates, other states' ESA administrators, and whether those administrators already give schools reconciliation tools

### Takeaway
TEFA is live and big: 274k+ applications, 100k+ awards and ~2,600–2,700 approved private schools by mid-2026. But **schools do not send formatted invoices to Odyssey.** They confirm enrollment and set tuition inside Odyssey's school portal (with bulk CSV upload), the parent confirms, and Odyssey pays the school's bank account through Stripe. Florida's Step Up runs a similar in-portal flow: the school submits an invoice in EMA and the parent approves it. Arizona/ClassWallet is the main rail where schools and families upload invoice documents. **So the "invoices formatted per platform" piece of F06 is mostly unnecessary for schools.** What is left is a split ledger, installment reconciliation and chasing parent approvals. The installment dates conflict across sources: the final TEFA payment is given as either Feb 1 or Apr 1 2027.

### Cited Findings

**Texas TEFA: status and scale**
- The Texas Comptroller chose **Odyssey** (New York) to run TEFA: parent applications, eligibility checks, payments to approved providers and family complaints (reported Oct 30 2025). — [Spectrum News](https://spectrumlocalnews.com/tx/austin/news/2025/10/30/texas-selects-odyssey-to-manage-tefa-program)
- Applications passed **274,000** when the first deadline closed. — [FOX 7 Austin](https://www.fox7austin.com/news/texas-education-freedom-accounts-tefa-deadline-applications)
- **More than 100,000 students** had been awarded TEFA accounts by Jun 11 2026. — [Community Impact, Jun 11 2026](https://communityimpact.com/austin/central-austin/texas-legislature/2026/06/11/more-than-100k-students-have-been-awarded-texas-education-freedom-accounts-here-are-the-next-steps/)
- Homeschool students get their whole $2,000 award at once. Private-school students are paid in installments, with the last 50% "scheduled for February 1, 2027" if the student is still enrolled. — [Texas Policy Research](https://www.texaspolicyresearch.com/texas-education-freedom-accounts-begin-funding-students/)
- A student "should not be charged a different amount of tuition and fees" because they have a TEFA award (school guidance, May 2026). — [TEFA: Tuition and Fee Guidelines for Participating Private Schools](https://educationfreedom.texas.gov/newsupdates/tuition-and-fee-guidelines-for-participating-private-schools/)
- One Texas school has **57 TEFA students** in 2026–27, including 24 new families. That is a data point for how many TEFA students a school may carry. — [KBTX, Aug 4 2026](https://www.kbtx.com/2026/08/04/vouchers-valley-how-tefa-funds-split-private-homeschool-families/)
- The Comptroller sought legal clarity on blocking schools with alleged CAIR ties (Dec 2025). This shows school eligibility is politically contested. — [Spectrum News, Dec 22 2025](https://spectrumlocalnews.com/tx/south-texas-el-paso/news/2025/12/22/texas-comptroller-asking-to-block-private-schools-with-alleged-islamic--chinese-ties-from-funding)

**Texas TEFA: payment dates (sources conflict)**
- **Odyssey's own help article** "TEFA Funding Timeline and Installments": 25% of the annual award on **Oct 1 2026**, and the balance on **Apr 1 2027**. Schedules may change. — [Odyssey support](https://support.withodyssey.com/hc/en-us/articles/51295974654107-TEFA-Funding-Timeline-and-Installments)
- A second search summary of Odyssey content: "at least 25%" on Jul 1 2026, "at least 50%" on Oct 1 2026, and the rest on Apr 1 2027. — [Odyssey support (search summary)](https://support.withodyssey.com/hc/en-us/articles/50342541584667)
- **Contradicted by** these sources, which give 25% on Jul 1, 25% on Oct 1 and 50% on **Feb 1 2027**:
  - [Texas Policy Research](https://www.texaspolicyresearch.com/texas-education-freedom-accounts-begin-funding-students/)
  - the corpus TX state file, citing educationfreedom.texas.gov [corpus TX]
  - [Sacred Heart school page](https://shmuenster.com/school/sacred-heart-esa/)
- Next private-school deposit: Oct 1 2026, 25% of the $10,474 award (≈$2,618). Students had to confirm participation by **Sep 15 2026** to keep their full award. — [Outschool TEFA guide](https://learner.outschool.com/esa-guides/what-to-do-after-tefa-approval)
- **I found no reporting that confirms the Oct 1 2026 deposit was posted, or that reports payment delays.** — searches of [Outschool](https://learner.outschool.com/esa-guides/what-to-do-after-tefa-approval) and Texas news

**Texas TEFA: how money reaches schools**
- Odyssey's school steps:
  1. The school confirms enrollment and sets tuition and fees in the **Odyssey school portal**.
  2. The parent confirms the amount.
  3. The parent submits the quarter's tuition payment.
  4. Once approved, funds go to the school's bank account **through Stripe**.

  Bulk tuition and enrollment entry is by **CSV upload**. — [Odyssey: Steps to Receive Tuition Payments](https://support.withodyssey.com/hc/en-us/articles/40256443594395-Overview-Steps-Required-to-Receive-Tuition-Payments-Through-Odyssey); [Odyssey: Confirming Enrollments and Setting Tuition](https://support.withodyssey.com/hc/en-us/articles/50129971354011-Confirming-Enrollments-and-Setting-Tuition-Fees)
- The portal tracks status with filters such as "Enrollment Verification Pending" and "Tuition/Fees Awaiting Confirmation", where the school waits for the parent. Parents cannot pay until tuition is entered and confirmed. — [Odyssey: How to Confirm the Tuition Fees Set by the School](https://support.withodyssey.com/hc/en-us/articles/51446221185435-How-to-Confirm-the-Tuition-Fees-Set-by-the-School)
- One-off charges (registration, lunch) use a separate "fee request" from the Student Enrollment & Fees page. — [Odyssey: Requesting School Fees](https://support.withodyssey.com/hc/en-us/articles/55293420706843-Requesting-School-Fees)
- Parents see requested payments in the TEFA parent portal. — [Odyssey: Viewing Requested Payments](https://support.withodyssey.com/hc/en-us/articles/55293737472923-Viewing-Requested-Payments-in-the-TEFA-Parent-Portal)
- A school page says TEFA funds go from the parent's TEFA account straight to the school, and families pay any remaining tuition separately. — [Sacred Heart (Muenster TX)](https://shmuenster.com/school/sacred-heart-esa/)
- Purchases from vendors must go through the Odyssey marketplace. Families cannot pay and then claim reimbursement. — [Outschool TEFA marketplace guide](https://outschool.com/esa-guides/tefa-odyssey-marketplace-guide)

**Texas TEFA: vendor approval**
- To join the TEFA marketplace, a vendor must be a US business entity in good standing on Texas franchise tax and registered with the Texas Secretary of State. Sole proprietors can file an assumed name with the county instead. — [Odyssey Texas: Who Can Become a Vendor](https://texas.support.withodyssey.com/hc/en-us/articles/44174864219675-Who-Can-Become-a-Vendor-and-What-are-the-Requirements)
- The vendor help section also covers price caps and purchase restrictions, fingerprinting for Texas vendors and professional licenses. — [Odyssey Vendors section](https://support.withodyssey.com/hc/en-us/sections/44028618370587-Vendors)
- **How vendors (as opposed to schools) are paid was not found.**

**Texas TEFA: approved schools and vendors (the count is growing)**
- ~600 schools applied in the first 10 days, and "nearly 600" signed up by Dec 2025. — [AOL/Texas Tribune syndication](https://www.aol.com/articles/600-private-schools-apply-texas-145900935.html); [The Texan](https://thetexan.news/issues/education/nearly-600-texas-private-schools-to-participate-in-upcoming-esa-program/article_b7eccbd7-3d2b-4fe9-ae5d-f2699465f201.html)
- 700 schools by Jan 9 2026. — [Spectrum News](https://spectrumlocalnews.com/tx/south-texas-el-paso/news/2026/01/09/700-schools-to-take-part-in-texas--school-voucher-program)
- "Over 1,500" private schools (date unclear). — [San Antonio Report](https://sanantonioreport.org/school-vouchers-texas-need-to-know-about-tefa-esa/)
- **"Over 2,600"** private schools approved, per the program website's map (Jun 2026). — [Community Impact](https://communityimpact.com/austin/central-austin/texas-legislature/2026/06/11/more-than-100k-students-have-been-awarded-texas-education-freedom-accounts-here-are-the-next-steps/)
- **"Over 2,700"** in a later piece. — [Community Impact Katy](https://communityimpact.com/katy-fulshear/education/thousands-of-katy-area-families-apply-for-new-education-accounts/)
- The Comptroller's fiscal note says "more than 2,000 accredited private schools and pre-K providers" registered, plus **"over 200 education service providers"** (page undated). — [Comptroller Fiscal Notes](https://comptroller.texas.gov/economy/fiscal-notes/government/2026/esa-ftd)
- There is no deadline for schools or vendors to apply, and schools may decline students. — [Community Impact](https://communityimpact.com/austin/central-austin/texas-legislature/2026/06/11/more-than-100k-students-have-been-awarded-texas-education-freedom-accounts-here-are-the-next-steps/)
- TEFA private schools must be accredited, have operated 2+ years and give a norm-referenced test. — [corpus F06 citing Texas Comptroller, Nov 25 2025](https://comptroller.texas.gov/about/media-center/news/20251125-acting-texas-comptroller-kelly-hancock-announces-final-rules-and-key-dates-for-texas-education-freedom-accounts-program-1764103747312)

**Other Odyssey states**
- **Louisiana GATOR** and **Georgia** use the same "confirm enrollments and set tuition fees" school flow on Odyssey. — [Odyssey LA GATOR](https://support.withodyssey.com/hc/en-us/articles/34510445057307-How-to-Confirm-Student-Enrollments-and-Set-Tuition-Fees-for-LA-GATOR); [Odyssey Georgia](https://georgia.support.withodyssey.com/hc/en-us/articles/43717408733211-Overview-Steps-Required-to-Receive-Tuition-Payments-Through-Odyssey)
- **Iowa:** after entering tuition, the school clicks **"Generate Invoice"**, which sends the request to the parent and then the state. — [Iowa Dept of Education doc](https://educate.iowa.gov/media/8596/download)
- Iowa chose Odyssey in 2023: $4.3M over six years. Iowa's auditor says an undisclosed amendment more than doubles the annual cost by FY2026. — [Iowa Governor](https://governor.iowa.gov/press-release/2023-02-28/iowa-selects-odyssey-esas); [The Gazette](https://www.thegazette.com/state-government/iowa-auditor-school-choice-deal-hiked-cost-without-justification/)

**Arizona (ClassWallet)**
- Since Jul 1 2024, families paying a school or preschool with ESA funds must **upload invoices into ClassWallet "Pay Vendor"**. The state contract requires all tuition to go through the platform. — [AZ Dept of Ed ESA newsletter, Jun 2024](https://azed.gov/sites/default/files/2024/06/ESA%20Newsletter_June%202024.pdf); [AZ Dept of Ed ClassWallet page](https://azed.gov/esa/classwallet)
- Required invoice fields: student name, provider name, service description, transaction date, itemized tuition/fees and total. (This comes from a third-party summary of the ESA Handbook.) — [Recess AZ guide](https://help.recess.gg/support/how-to-use-arizona-esa-funds)
- An Arizona school's FAQ says the Pay Vendor option carries a ClassWallet fee that does not count toward tuition, and ESA distribution "can take several weeks". The school uses FACTS to keep family accounts current while ESA funds are pending. — [Valley Christian Tuition Payment FAQ 24–25](https://valleychristianaz.org/wp-content/uploads/2024/09/Tuition-Payment-FAQ-24-25.pdf)
- June 2026: the Treasurer and the Department of Education are reviewing ESA vendors. ClassWallet "could face competition". — [AZ Capitol Times, ClassWallet tag](https://azcapitoltimes.com/news/tag/classwallet/)
- AZ ESA had 106,253 students on Sep 21 2026. [corpus AZ state file citing azed.gov]

**Florida (Step Up For Students)**
- The school **submits an invoice in the EMA**, and the parent approves or denies it before each release. Private-school funds are released Aug 1/Sep 1, **Nov 1, Feb 1 and Apr 1**. Accounts are funded up to 2 weeks after Step Up receives the money. — [Step Up: private school funding](https://www.stepupforstudents.org/scholarships/private-school/fund/); [Step Up FAQ 2026–27](https://www.stepupforstudents.org/faq/faqs-for-2026-27-scholarship-deadlines-and-payment-schedules/); [2026–27 payment schedule PDF](https://go.stepupforstudents.org/hubfs/Website/Document-Library/2026-27_PaymentDistroSchedule.pdf)
- Students approved by Sep 30 2026 get 100% of the award; those approved by Jan 15 2027 get 50%. — [Tutero](https://www.tutero.com/us/blog/step-up-payment-schedule-award-amounts-2026-27)
- Sources conflict on whether PEP (Florida's personalized education program) is at capacity. — same search; [Outschool FL guide](https://outschool.com/esa-guides/florida-step-up-for-students)

**Other states**
- **Arkansas:** ADE sought a $70M transfer for LEARNS Education Freedom Accounts. A 2024 rule set four equal quarterly payments. — [KATV](https://katv.com/news/arkansas-department-of-education-seeks-70m-transfer-for-learns-education-freedom-accounts-katv-news-share-inform-community-public); [ADE rule markup](https://adecm.ade.arkansas.gov/Attachments/Payments_Under_the_Educational_Freedom_Account_Program_-_Repeal_Markup_082903.pdf)
- **North Carolina:** the ESA+ program publishes its own invoice-documentation rules. — [NCSEAA ESA+ invoice documentation](https://k12.ncseaa.edu/media/spgn2j44/esaplus-invoice-documentation.pdf)
- **Federal tax-credit scholarships** start "beginning in 2027", one more payer type for schools. This is a single opinion post. — [Substack (Goldstein)](https://michaelgoldstein.substack.com/p/a-solution-for-the-anxious-generation)
- **Payment rails by state:** [corpus F06 citing GetESAPaid](https://getesapaid.com/become-an-esa-vendor)
  - ClassWallet: AZ, AR, TN, WV, NC, IN, NH, AL, SC
  - Odyssey: TX, IA, UT, GA, LA, WY, MO
  - Step Up: FL
  - Correction: WV moved to its own portal plus TheoPay [corpus].

**Reconciliation tools from the administrators**
- **I found no documentation of payout or reconciliation reports for schools, from Odyssey or any other administrator.** The Odyssey portal shows enrollment and tuition status filters and supports bulk CSV upload of tuition. No export of payouts per student was found. — [Odyssey support](https://support.withodyssey.com/hc/en-us/articles/51446221185435-How-to-Confirm-the-Tuition-Fees-Set-by-the-School)

### Inferences
- **The Odyssey invoice generator in the F06 spec is not needed for schools.** The portal is the invoice. In TX, LA, GA and IA the school types tuition (or uploads a CSV) into Odyssey, and Iowa even has a "Generate Invoice" button. Step Up does the same in EMA. Only Arizona/ClassWallet (and possibly NC ESA+) needs separately formatted invoice documents.
- **What schools still have to do by hand (my judgment from the portal flow):**
  1. Chase parents who have not confirmed tuition or approved the invoice. Both Odyssey and Step Up block payment until the parent acts, and a missed step can delay or cut funding (the Sep 15 TEFA confirmation; Step Up's 100% vs 50% enrollment cut-off).
  2. Post each state payout against each family in the school's own tuition system (FACTS, QuickBooks or a spreadsheet). The ESA share and the parent remainder are billed differently, and TEFA rules forbid charging TEFA students a different price.
  3. Reconcile lump-sum Stripe payouts to students. **This is unverified.** It depends on whether Odyssey sends one payout per student or a batch.
- **Payment-date risk:** if Odyssey's Apr 1 2027 date is correct, the pitch should say "the next TEFA installment" rather than "Feb 1". Florida's Nov 1 2026, Feb 1 2027 and Apr 1 2027 releases give rolling quarterly reasons to reach out.
- **Two approved-school counts:** the TEFA map (~2,700 schools) is a public, scrapeable prospect list. The 2-year accreditation rule means Texas buyers are established private and faith schools, not new microschools.

### Gaps
- Whether the Oct 1 2026 TEFA installment was actually paid, and whether it was late. Searches found no October 2026 reporting.
- Whether Odyssey's school portal offers payout or remittance exports per student. This decides whether the "reconcile" feature is needed.
- How TEFA *vendors* (tutors, therapists) are paid and whether they invoice.
- Tennessee's Oct 15 2026 payout (from the screen notes) was not re-checked. Utah, West Virginia and Louisiana 2026–27 changes were not checked one by one.
- Political and litigation risk to TEFA and the AZ ESA was not searched this round.
- I could not read any official Odyssey page directly, and every Odyssey detail comes from search summaries.

---

## Q2. F06 competitor sweep: FACTS, TADS, Blackbaud, Veracross, Brightwheel, Transparent Classroom, GetESAPaid, ESA bookkeeping services, microschool networks

### Takeaway
**I found no product that does split ESA vs parent ledgers plus multi-program installment reconciliation.** That is a real gap, but it rests on absence of evidence from search summaries. Schools already run general tuition systems (FACTS claims 6,500+ schools) and use them *next to* the ESA portals. So the wedge must be a sidecar to FACTS, not a replacement. **GetESAPaid, the corpus's "live competitor at $39/mo", has no search footprint at all, and its domain did not resolve.** Its existence and traction are unverified.

### Cited Findings
- **FACTS:**
  - An Arizona school uses FACTS "to help families keep accounts current while scholarship funds are pending". It says the ESA contract is between the parent and the state, so the parent remains responsible for the tuition account. — [Valley Christian FAQ](https://valleychristianaz.org/wp-content/uploads/2024/09/Tuition-Payment-FAQ-24-25.pdf)
  - FACTS is "used by … over 6,500 schools nationally" (a school's FACTS page; the search summary did not say which school, likely one of these). — [New Hope Academy FACTS page](https://newhopeacademy.org/admin/FACTS.php); [Aquinas Academy](https://www.aquinasacademy.org/facts-and-financial-aid/)
  - **No search result showed FACTS integrating with TEFA or any ESA platform.** — same searches
  - Capterra reviewers call FACTS overpriced, cite unanswered support, and complain about automatic late fees. — [corpus F06 citing Capterra](https://www.capterra.com/p/10027955/FACTS-Tuition-Management/)
- **Brightwheel:**
  - Its billing help center covers program rates, billing plans, family invites and tuition insurance.
  - **No ESA or voucher feature was found.**
  - It is aimed at childcare and preschool.
  - — [Brightwheel billing help](https://intercom.help/brightwheel/en/collections/87111-billing)
- **Split-billing tools exist in general:**
  - Jackrabbit Care can split a charge between households or a third-party agency, but only in student-based billing mode, and only staff can set it up. — [Jackrabbit split billing](https://carehelp.jackrabbitclass.com/help/split-billing)
  - Zunia splits fees across debtor accounts by % or $. — [Zunia](https://educationhodev.wpengine.com/solutions/zunia/school-billing-software/)
- **Transparent Classroom:** search found no ESA or billing feature. — [same search](https://intercom.help/brightwheel/en/collections/87111-billing)
- **GetESAPaid:**
  - The corpus says it sells an invoice generator, rejection checker and audit binder for **$39/mo or $390/yr**. — [corpus F06 citing GetESAPaid](https://getesapaid.com/become-an-esa-vendor)
  - **This round:** a quoted search for "getesapaid" returned no matching results, and `getesapaid.com` gave DNS ENOTFOUND from this environment. The corpus's other fetches did work, so this may be an environment issue. **Status unverified.**
- **ESA bookkeeping services:**
  - The only relevant result was a July 2026 vendor-neutral bookkeeping guide for microschools. It says ESA payments come on the state's schedule ("30 to 60 day delays between approval and payment are common"), and it recommends tracking each family's funding source (full pay, fully ESA, or split) "or reconciling state payments to students becomes difficult".
  - It also says 25+ states let funding follow students.
  - — [beancount.io guide, Jul 16 2026](https://beancount.io/es/blog/2026/07/16/starting-a-microschool-learning-pod-bookkeeping-guide)
  - **I found no named ESA-specialist bookkeeping firm.**

### Inferences
- **The bookkeeping guide describes the F06 core in its own words.** Track the funding source per family, expect 30–60 day lags and reconcile state payments to students. This is evidence of the need from a neutral source, but it is not evidence that schools will pay for it.
- **Competitive position:**
  - Incumbents (FACTS, Blackbaud, Veracross, TADS) handle the parent side of tuition well and appear blind to ESA receivables.
  - A sidecar that imports a FACTS or QuickBooks family list plus Odyssey/EMA/ClassWallet status and produces "ESA expected vs received vs parent remainder" per family does not compete head-on with them.
- **Microschool networks (judgment, not searched):** KaiPod, Prenda and Primer probably handle billing centrally for their affiliated schools, so network members are not individual buyers. Independent microschools are, but their median of 20–22 students caps what they will pay.

### Gaps
- TADS, Blackbaud Tuition Management, Veracross, Alma, Sycamore and Gradelink were not searched because of the search budget. Whether any added TEFA/ESA split billing in 2026 is unknown.
- KaiPod, Prenda and Primer billing or ESA services were not searched.
- GetESAPaid: price, existence and traction are all unverified this round.

---

## Q3. F06 buyers, reachability and demand signals

### Takeaway
Texas gives an unusually reachable buyer list: a public TEFA map of ~2,700 approved private schools. Microschools are numerous (~75,000 estimated) but tiny: a median of about 20–22 students, and only 38% take state choice funds. **Demand signals are structural, not vocal.** The search found no 2026 posts from school administrators complaining about ESA reconciliation. The evidence is the shape of the workflow: parent-confirmation gates, quarterly releases and multi-week lags.

### Cited Findings
- **Microschools:**
  - About **75,000 microschools serving ~1.5M students**, per a National Microschooling Center estimate (May 2026). — [K-12 Dive](https://www.k12dive.com/news/what-you-need-to-know--about-microschools/827601/)
  - Median size: 20 students at nonpublic microschools (K-12 Dive). The 74 says the median rose from 16 (2024) to 22. — [K-12 Dive](https://www.k12dive.com/news/what-you-need-to-know--about-microschools/827601/); [The 74](https://www.the74million.org/article/exclusive-7-things-to-know-about-microschools-in-2026/)
  - **38% of surveyed microschools receive state school-choice funds** (up from 32% in 2024). — [The 74](https://www.the74million.org/article/exclusive-7-things-to-know-about-microschools-in-2026/)
  - More than 88% rely on tuition. — [NewsNation](https://digital-release.newsnationnow.com/?p=2388508)
  - The survey sample is reported as either 1,000 or 800 schools. — [K-12 Dive](https://www.k12dive.com/news/what-you-need-to-know--about-microschools/827601/); [The 74](https://www.the74million.org/article/exclusive-7-things-to-know-about-microschools-in-2026/)
- **Texas:**
  - ~2,600–2,700 approved private schools, listed on the program website's map. — [Community Impact](https://communityimpact.com/austin/central-austin/texas-legislature/2026/06/11/more-than-100k-students-have-been-awarded-texas-education-freedom-accounts-here-are-the-next-steps/); [Community Impact Katy](https://communityimpact.com/katy-fulshear/education/thousands-of-katy-area-families-apply-for-new-education-accounts/)
  - Over 200 education service providers. — [Comptroller](https://comptroller.texas.gov/economy/fiscal-notes/government/2026/esa-ftd)
- **Arizona:** 106,253 ESA students (Sep 2026). [corpus AZ]
- **Pain signals:**
  - Arizona's ESA distribution "can take several weeks", and Pay Vendor has a fee. — [Valley Christian FAQ](https://valleychristianaz.org/wp-content/uploads/2024/09/Tuition-Payment-FAQ-24-25.pdf)
  - "30 to 60 day delays between approval and payment are common". — [beancount.io guide](https://beancount.io/es/blog/2026/07/16/starting-a-microschool-learning-pod-bookkeeping-guide)
  - Arkansas's Jun 2026 assessment found ClassWallet "fragmented, inefficient", with manual workarounds and weak reporting. — [corpus F06 citing Grand Canyon Times](https://grandcanyontimes.com/report-finds-esa-vendor-classwallet-fragmented-inefficient-and-increasingly-misaligned)
  - Step Up tells parents to act quickly on invoice emails "to avoid tuition delays". — [Step Up private school funding](https://www.stepupforstudents.org/scholarships/private-school/fund/)

### Inferences
- **Reachability score: 4/5 for Texas.**
  - The map is a cold-email list.
  - Most of these schools are established faith-based schools, so Catholic diocesan business offices and accreditor associations (TEPSAC members, e.g. TAPPS/TCCED) are one-to-many channels.
  - The Texas Private Schools Association, from the corpus, is another.
  - Diocesan offices may act as committees, which slows sales.
- **Volume per school is real money.** 57 TEFA students × $10,474 ≈ **$597k a year** flowing through Odyssey for one school (my arithmetic from the [KBTX](https://www.kbtx.com/2026/08/04/vouchers-valley-how-tefa-funds-split-private-homeschool-families/) example). A tool at $79–149/mo is under 0.3% of that, so willingness to pay is plausible if the pain is real.
- **Microschools are a weaker first market.** At a median of 20–22 students, with only 38% ESA-funded, a microschool may have ~8 ESA students, which a spreadsheet handles.

### Gaps
- No public 2026 Reddit, Facebook or forum posts from school business managers about ESA reconciliation were found. I did not specifically search Facebook groups, and they are not indexed well.
- Florida Step Up participating-school count and Arizona private-school/microschool ESA vendor count were not found.
- The share of TEFA schools already on FACTS, Blackbaud or other tools is unknown.

---

## Q4. F06 verdict, refined wedge, price, first-30-days plan and revenue path

### Takeaway
**Verdict: BUILD-IF.** Build only after a 2–3 week sales test produces at least 8–10 paid pre-orders from Texas/Florida schools for an "ESA Receivables Ledger". The original spec needs three changes:
- Drop per-platform invoice generators, except Arizona ClassWallet.
- Lead with the parent-approval chaser and the ESA-vs-parent split ledger.
- Sell as a sidecar to FACTS or QuickBooks.

Re-score: **29/40**, down from the screen's 31–32. Base case: $5k MRR in about 9–12 months and $10k MRR in about 18–24 months.

### Cited Findings
- The facts that drive the redesign:
  - Odyssey's flow is in-portal, with bulk CSV and Stripe payout. — [Odyssey](https://support.withodyssey.com/hc/en-us/articles/40256443594395-Overview-Steps-Required-to-Receive-Tuition-Payments-Through-Odyssey)
  - Step Up's EMA invoice needs parent approval. — [Step Up](https://www.stepupforstudents.org/scholarships/private-school/fund/)
  - ClassWallet Pay Vendor requires invoice uploads. — [AZ DOE](https://azed.gov/sites/default/files/2024/06/ESA%20Newsletter_June%202024.pdf)
  - TEFA forbids charging TEFA students a different tuition. — [TEFA guidelines](https://educationfreedom.texas.gov/newsupdates/tuition-and-fee-guidelines-for-participating-private-schools/)
  - ~2,700 approved TX schools are on a public map. — [Community Impact](https://communityimpact.com/katy-fulshear/education/thousands-of-katy-area-families-apply-for-new-education-accounts/)
- Corpus price reference: GetESAPaid at $39/mo (unverified this round). — [corpus F06](https://getesapaid.com/become-an-esa-vendor)

### Inferences

**Refined wedge: an "ESA Receivables Ledger" for private schools (TX first, FL second, AZ third). Ships in 4–5 weeks:**
1. **Family roster by payer**, imported by CSV from FACTS, QuickBooks, Blackbaud or a sheet. Each student carries their programs (TEFA, Step Up FES-EO/FTC, AZ ESA, and later federal tax-credit SGO), award amount, installment schedule and the parent remainder.
2. **Expected vs received per installment** for each student. Payouts come in by CSV, from a Stripe payout export or an Odyssey/EMA status screen copy, or are marked by hand. It shows aging and shortfall alerts.
3. **Parent-action chaser:** email nudges when a parent has not confirmed TEFA tuition or approved a Step Up EMA invoice, timed to each program's cut-offs (TEFA confirmation dates; Step Up's Sep 30 / Jan 15 enrollment cut-offs; Nov 1, Feb 1 and Apr 1 releases).
4. **Parent remainder statements**: what the ESA covered and what the family owes. The school collects through its existing FACTS or Stripe; **no payment processing.**
5. **Posting export**: a per-family credit file the business office can key or import into FACTS or QuickBooks.
6. **Audit binder**: accreditation, testing roster and enrollment confirmations, with expiry reminders.
7. **Arizona-only** ClassWallet itemized invoice PDF pack.

**Explicitly cut:** an Odyssey or Step Up invoice formatter, enrollment and contracts, attendance, and the F07 vendor tier. Vendor payment mechanics are unverified and TEFA has only ~200 service providers.

**Price (judgment):**
- **School: $79/mo for up to 75 ESA students; $149/mo for up to 250.** Annual prepay: $790 / $1,490.
- **Founding offer: $49/mo locked for life for the first 20 schools**, prepaid annually ($490) to bring cash forward.
- Microschool (AZ/FL, up to 30 ESA students): $39/mo.
- Blended ARPU assumption ≈ $85/mo.

**Re-score (rubric, judgment):**

| Criterion | Score | Reason |
|---|---|---|
| Build | 4 | CRUD, CSV and email; no integrations |
| Regulatory | 4 | No funds held; financial records only |
| Self-serve | 3 | School business managers can buy by card, but some schools need diocesan or head-of-school sign-off |
| Distribution | 4 | Public TEFA map, diocesan and association channels |
| WTP | 4 | Hundreds of thousands of dollars of ESA money per school |
| Gap | 4 | No ESA receivables tool found |
| Urgency | 3 | Next TEFA installment Feb 1 or Apr 1 2027; Step Up Nov 1 / Feb 1 / Apr 1; TEFA year-2 re-enrollment in spring 2027. Pain happens quarterly, not daily |
| Support | 3 | Quarterly engagement raises churn risk in summer |
| **Total** | **29/40** | |

**First 30 days (sell before building):**
- **Days 1–3:**
  - Pull the TEFA participating-school map into a sheet with name, city, type and website.
  - Find business-office contacts for ~800 schools.
  - Draft a one-page "TEFA + parent remainder reconciliation" sheet template as the lead magnet.
- **Days 3–10:**
  - Send 40–60 personalized emails a day under CAN-SPAM rules, asking one question: "How did you post the Oct 1 TEFA installment against family tuition accounts, and what broke?"
  - Goal: **15 discovery calls**.
  - On every call, ask to screen-share the Odyssey school portal. Confirm whether payout or remittance exports exist (the biggest open question) and whether Stripe payouts are batched.
- **Days 7–20:**
  - Concierge offer: "we'll reconcile your next installment for you". Done by hand in a sheet for $490/yr prepaid, or a $49/mo founding plan.
  - Contact 3–5 Catholic diocesan school business offices and the Texas Private Schools Association as channel partners.
  - In Florida, email schools ahead of the **Nov 1** Step Up release.
- **Days 20–30:**
  - **Gate:** at least 8 paid pre-orders (or 5 annual prepays) means build. Fewer than 3 means drop F06.
  - Publish SEO pages: "TEFA installment schedule for schools", "TEFA tuition confirmation", "Step Up EMA invoice not approved".

**Revenue path (judgment):**
- **$5k MRR ≈ 60 schools** at ~$85 ARPU. **$10k MRR ≈ 120 schools.**
- **One full pass of cold email:**
  - Assume 1,500 contactable Texas schools × 5% reply × 40% to call × 30% close ≈ **9 schools**.
  - Three touches plus Florida and Arizona plus 1–2 diocesan or association partners might give 30–60 schools in the first 6–9 months.
- **Base case:** first revenue in month 1 (pre-orders); **$5k MRR in about 9–12 months; $10k MRR in about 18–24 months.**
- **Upside:** a diocesan or association deal (many schools at once) could halve these times.
- **Downside:** if Odyssey already gives clean per-student remittance reports, the reconciliation pain largely disappears, and so does the product.

**F07 vendor tier:** do not build now. Incumbents charge ~$15 [corpus F07], TEFA lists only ~200 service providers, and how vendors are paid is unverified.

### Gaps
- The key kill-or-confirm question cannot be answered from search: **does Odyssey's school portal give per-student payout and remittance reports?** It must be checked on discovery calls.
- No 2026 price list exists for FACTS or Blackbaud to anchor a "cheaper than" claim. The product is a sidecar, so this matters less.
- Conversion rates in the revenue math are my assumptions, not sourced benchmarks.

---

## Q5. I03 trigger check: WildApricot (Personify) 2025–2026 prices, the outside-processor surcharge, Personify's Jan 2026 sale and user reaction

### Takeaway
- **The 20% surcharge is real and in WildApricot's own policy.** A "Payment System Servicing Fee" equal to 20% of the plan is charged at renewal to US and Canadian accounts that use PayPal, Stripe or Authorize.net.
- **Prices:** ~$63–66/mo for 100 contacts, ~$78/mo for 250 and ~$147/mo for 500 (Aug 2026 aggregators). A small 2026 increase is suggested by $63 moving to $66, but this is unconfirmed.
- **The sale:** Momentive bought Personify on Jan 6 2026. **No WildApricot-specific changes to pricing or the roadmap had been announced** as of these searches.
- **User reaction is mixed, not uniformly hostile:** Capterra 4.4/5 (555 reviews), G2 3.8/5 (45 reviews), Trustpilot 1.3/5 (159 reviews). The recurring complaints are price hikes, tier jumps and weaker support after Personify.

### Cited Findings
- **The surcharge, in WildApricot's own policy:** "A Payment System Servicing Fee (PSSF) will apply to accounts who use PayPal, Stripe, or Authorize.net … upon renewal … The PSSF is equivalent to 20% of the current billing plan." It does not apply outside the US and Canada.
  - Monthly subscribers get no refund of the fee.
  - Annual and 2-year subscribers get a pro-rated refund if they switch to WildApricot Payments (AffiniPay), and owe a pro-rated charge if they switch to a third-party processor mid-term.
  - — [WildApricot Billing and Refund Policy](https://www.wildapricot.com/legal-center/billing-and-refund-policy)
- **WildApricot Payments:** 2.9% + $0.30 per transaction (3.5% + $0.30 for Amex). Users on it avoid the 20% fee. — [WildApricot (search summary of a WA page)](https://www.wildapricot.com/?p=6094)
- **List prices:**
  - **GetApp (Aug 2026):** $78/mo for 250 contacts and $147/mo for 500 contacts. — [GetApp pricing](https://www.getapp.com/customer-management-software/a/wild-apricot/pricing/)
  - **Fitgap:** 100-contact Personal plan $63/mo monthly, $56.70/mo on an annual contract. — [Fitgap](https://us.fitgap.com/products/wildapricot)
  - **Capterra:** starts at $63. — [Capterra](https://www.capterra.com/p/76116/Wild-Apricot/)
  - **CostBench (Aug 2026)** shows $66. — [CostBench](https://www.costbench.com/software/board-management/wildapricot/)
  - The corpus read WildApricot's pricing page ("last updated Feb 7 2026"): **$66/mo** monthly for 100 contacts. — [corpus I03](https://www.wildapricot.com/pricing)
  - A competitor reported **April 2026 annual** prices of $886 (250 contacts) and $1,663 (500), and a price history of +20% (2021), +25% (2023), a rise in 2025 and ~5% in early 2026. — [corpus I03 citing Groupable](https://www.groupable.com/blog/wild-apricot-pricing-hidden-fees)
- **No official announcement of a 2026 price increase was found.** GetApp reviews (updated Jul–Aug 2026) mention "frequent price increases and steep jumps between tiers". — [GetApp reviews](https://www.getapp.com/customer-management-software/a/wild-apricot/reviews/)
- **The Momentive sale:**
  - Momentive Software acquired Personify. The combined company serves ~**37,000 clients**. No WildApricot pricing or roadmap changes were found. — [Personify notice](https://personifycorp.com/?p=35070); [Raklet summary](https://www.raklet.com/?p=59161)
  - "Third owner in nine years" comes from a WildApricot partner and consultant who sells a rival platform. — [popsb](https://popsb.com/wild-apricot-alternatives)
- **Reviews:**
  - Capterra: 4.4/5 from 555 reviews (customer service 4.4, ease of use 4.2).
  - G2: 3.8/5 from 45 reviews.
  - A Capterra reviewer says support "became poor since Personify bought" WildApricot and is mostly email.
  - A Feb 2026 Trustpilot reviewer reports weeks-long responses and a cancelled sales call.
  - — [Capterra reviews](https://capterra.com/p/76116/WildApricot/reviews/); [G2](https://g2.com/products/wildapricot/reviews?page=2); [Trustpilot](https://es.trustpilot.com/review/wildapricot.com)
  - Trustpilot: 1.3/5 across 159 reviews (accessed Sep 24 2026). — [corpus I03 citing Trustpilot](https://www.trustpilot.com/review/wildapricot.com)
- **Wishlist:** WildApricot's own wishlist has long-running threads on card fees and a cheap (~$25) plan. — [WA wishlist: card fees](https://forums.wildapricot.com/forums/308932-wishlist/suggestions/8827999-credit-card-fees-to-be-paid-by-members?page=2); [corpus I03: low-level plan thread](https://forums.wildapricot.com/forums/308932-wishlist/suggestions/13335057-low-level-pricing-plans-e-g-25)

### Inferences
- **Where the surcharge bites:** it applies only to orgs that chose Stripe, PayPal or Authorize.net. Those orgs **already own a processor account**, so a "bring your own Stripe" product fits them exactly. If WildApricot stored their recurring payment methods in the org's own Stripe account, migration might not need members to re-enter cards. **This is a hypothesis, not verified.**
- **Timing:** the fee is charged at each org's WildApricot renewal. Renewal dates are spread through the year, so the trigger is rolling rather than one dated window.
- **Not a broad revolt:** Capterra's 4.4 means much of the base is satisfied enough to stay. The pool of active switchers is a minority of a ~10–20k customer base.
- **Personify sale:** it gives future urgency (repricing within 18–36 months, per [corpus I03 citing SmartThoughts](https://www.smartthoughts.net/post/momentive-personify-acquisition-association-impact)) but no announced 2026–27 change to sell against today.

### Gaps
- WildApricot's official 2026 pricing page (all tiers) could not be fetched, and the $63 vs $66 discrepancy is unresolved.
- Whether a 2027 increase has been announced is unknown.
- Whether WildApricot's Stripe integration stores members' cards as Stripe customers in the org's own account (for token portability) was not searched.

---

## Q6. I03 competitor sweep: ClubExpress, MemberClicks, GrowthZone, Join It, Raklet, Membership Toolkit, Zeffy, Glue Up, Novi AMS, Hivebrite, Memberplanet and cheap or free tools

### Takeaway
**The cheap end is crowded, and the "no surcharge, cheaper than WildApricot" message is already taken.**
- MembershipWorks: free up to 50 accounts, $35/mo up to 300, no transaction cut, with a "WildApricot alternative" page.
- Join It: $0–$29+ plus a 1.5–4% fee on online payments.
- Zeffy: free, funded by donor tips, with auto-renewals and a member database.
- ClubExpress: ~$0.30–0.42 per member per month, with a ~$24–30 minimum.
- Raklet: free for 100 contacts, ~$49–59 for 500.

The upper tier (MemberClicks ~$3,500/yr, GrowthZone/ChamberMaster ~$3,900/yr) is expensive, but those buyers are chambers and staffed associations that decide by committee.

### Cited Findings

| Product | Price (date / source quality) | Notes | Source |
|---|---|---|---|
| **MembershipWorks** | Free ≤50 accounts; **$35/mo ≤300**; $59 ≤600; $95 ≤1,200; $145 ≤2,500; $205 ≤5,000; $259 ≤10,000 (official pricing page via search, 2026) | Family = 1 account; no contracts; no free trial but 30-day money-back; "does not take a portion of transactions" | [MembershipWorks pricing](https://membershipworks.com/pricing/); [MembershipWorks vs WildApricot](https://membershipworks.com/wildapricot-alternative/) |
| **Join It** | Free $0; Starter $29; Growth $49; Total $99; Extra $249/mo, **plus 1.5–4% service fee** on online payments (official support article) | Stripe-based autopay; 10% nonprofit + 10% annual discounts; its own comparison page says "no transaction fees", which conflicts | [Join It pricing FAQ](https://support.joinit.com/en/articles/2772686-general-pricing-questions); [Software Advice](https://www.softwareadvice.com/membership/join-it-profile/) |
| **Zeffy** | **$0** (funded by donor tips; vendor claim) | Memberships with automated renewals, member database, import/export, emails, digital membership cards; directory not confirmed | [Zeffy membership](https://www.zeffy.com/home/membership-application-form-nonprofits-associations); [Zeffy vs WildApricot](https://www.zeffy.com/compare/zeffy-vs-wildapricot) |
| **ClubExpress** | $0.42/member/mo ≤200; $0.38 ≤300; $0.34 ≤500; $0.30 ≤1,000; min **$30/mo** (2023 vendor PDF) or $24 (Fitgap); "starts $35–50" per aggregators | Charges only active primary members | [GetApp](https://www.getapp.com/all-software/a/clubexpress/); [ClubExpress pricing PDF](https://images.g2crowd.com/uploads/pricing/file/7388/What-Is-ClubExpress---Pricing.pdf); [Fitgap](https://us.fitgap.com/products/021361/clubexpress); [ITQlick](https://www.itqlick.com/clubexpress/pricing) |
| **Raklet** | Free ≤100 contacts; Essentials $59/mo ($49 annual) ≤500; Professional $119 ($99 annual) ≤1,000 (AI-extracted third-party data, conflicting) | — | [Pulse Signal](https://getpulsesignal.com/compare/podium-vs-raklet) |
| **Memberplanet** | $50 / $100 / $175 per month, plus platform and processing fees per transaction | Trial status conflicts between sources | [Capterra](https://capterra.com/p/131768/MemberPlanet/pricing/); [TrustRadius](https://web-v2.prod.trustradius.com/products/memberplanet/pricing) |
| **MemberClicks** (Momentive) | From **$3,500/yr** (Capterra); Raklet says $3,500 MC Trade / $4,500 MC Professional | Raklet (a competitor) claims a ~20% hike in Jul 2023 and a 60-day cancellation notice with a ~80% penalty; verify | [Capterra](https://capterra.com/p/133851/MemberClicks/); [Raklet](https://www.raklet.com/?p=59161) |
| **GrowthZone / ChamberMaster** | From **$3,900/yr** (Capterra); PricingSaaS says not disclosed | — | [Capterra ChamberMaster](https://www.capterra.ca/reviews/144469/chambermaster); [PricingSaaS](https://pricingsaas.com/companies/growthzone) |
| Glue Up, Novi AMS, Hivebrite, Membership Toolkit, Groupable | **No prices found this round** | — | — |

- **"WildApricot alternative" search results** are already full of vendor content: Jotform ("5 best… 2026"), Mighty Networks, Toolradar, GetApp, MembershipWorks, Zeffy and a partner blog. — [Jotform](https://www.jotform.com/blog/wild-apricot-alternatives/); [Mighty Networks](https://www.mightynetworks.com/resources/wild-apricot-alternatives); [Toolradar](https://toolradar.com/alternatives/wild-apricot); [popsb](https://popsb.com/wild-apricot-alternatives)

### Inferences
- **Price advantage is gone.**
  - The I03 screen's $29 (≤250) / $49 (≤1,000) / $99 (≤5,000) would match or beat MembershipWorks only at some tiers (MembershipWorks is $35 at ≤300 and $95 at ≤1,200).
  - Join It and Zeffy are cheaper at the low end.
  - "No surcharge" is table stakes: MembershipWorks, ClubExpress and Zeffy all advertise it, explicitly or by design.
- **Search channel:** "WildApricot alternative" is a contested SEO term where established vendors and Jotform-scale content sites already rank. A new domain would take months to rank.
- **Remaining differentiation is thin:** import fidelity, events and directory quality, and possibly carrying Stripe autopay over without re-collecting cards (unverified). MembershipWorks and others likely offer free migration help already (judgment; not verified).

### Gaps
- Prices for Glue Up, Novi AMS, Hivebrite, Membership Toolkit and Groupable were not found.
- Whether MembershipWorks, Join It and others run WildApricot one-click importers was not checked.
- Wix and Squarespace member areas were not checked.

---

## Q7. I03 buyers, reachability and demand signals

### Takeaway
The buyer pool is large:
- roughly 10–23k WildApricot organizations (third-party estimates; ~68% US),
- ~7,000 US chambers,
- tens of thousands of 501(c)(6) and (c)(7) organizations (IRS counts dated 2003–2008).

Data access for an importer is good: a public REST API, and an open-source exporter released in May 2026. But no Reddit "WildApricot alternative" threads surfaced, and dissatisfaction is a minority view on Capterra.

### Cited Findings
- **WildApricot customer counts:**
  - "More than 32,000 organizations" by late 2022. — [Zoftware Hub](https://zoftwarehub.com/en-sa/products/wildapricot/product-details)
  - BuiltWith tracks **23,136 WildApricot sites, 10,700 live**. — [BuiltWith](https://trends.builtwith.com/cms/Wild-Apricot)
  - iDataLabs counts 9,292 companies, **68% US**. Enlyft counts 8,892. Landbase counts 1,473 verified. — [iDataLabs](https://idatalabs.com/tech/products/wild-apricot); [Enlyft](https://www.enlyft.com/tech/products/wild-apricot); [Landbase](https://data.landbase.com/technology/wild-apricot/)
- **Chambers:**
  - "Nearly 7,000 chambers of commerce" in the US. — [US Chamber accreditation](https://uschamber.com/chamber-accreditation-program)
  - ACCE serves 9,000+ leaders from **1,300 chambers**. — [ACCE about](https://secure.acce.org/pages/about-us/)
- **Associations and clubs:**
  - 501(c)(6): 69,734 registered (2008). — [Ballotpedia](https://ballotpedia.org/501(c)(6))
  - About 84,838 in 2003. — [Chronicle of Philanthropy/IRS table](https://www.philanthropy.com/news/tax-exempt-organizations-registered-with-the-irs-185613/)
  - 501(c)(7) social clubs: ~69,522 (2003). — [Chronicle of Philanthropy/IRS table](https://www.philanthropy.com/news/tax-exempt-organizations-registered-with-the-irs-185613/)
- **Data access for an importer:**
  - WildApricot's REST Contacts endpoint can return all contacts (async: you get a result ID, then fetch). — [WA developer forum](https://forums.wildapricot.com/forums/309658-developers/suggestions/48357941-get-all-data)
  - An open-source CLI (created May 2026) exports "members, events, registrations, invoices, payments, donations, audit log, config, files via the public REST API and WebDAV". — [GitHub: JustinPaoletta/wild-apricot-exports](https://github.com/JustinPaoletta/wild-apricot-exports)
  - CSV/Excel export may vary by account. — [Enterprise DNA](https://enterprisedna.co/omni/instead-of/wild-apricot)
  - A WordPress plugin ecosystem exists around WildApricot (e.g. NewPath's "Wild Apricot Press"). — [GitHub NewPath-Consulting](https://github.com/NewPath-Consulting/Wild-Apricot-Press)
- **Demand signals:**
  - GetApp reviews (Jul–Aug 2026) cite frequent price increases and steep tier jumps. — [GetApp](https://www.getapp.com/customer-management-software/a/wild-apricot/reviews/)
  - Trustpilot complaints run through Aug 2026 (email editor, site builder, support). — [corpus I03 citing Trustpilot](https://www.trustpilot.com/review/wildapricot.com)
  - **The Reddit search returned no threads.** — [search results page set](https://toolradar.com/alternatives/wild-apricot)

### Inferences
- **Prospect list:**
  - BuiltWith's ~10,700 live WildApricot sites give a usable list.
  - Sites that show Stripe or PayPal checkouts are the orgs paying the 20% fee.
  - This is the sharpest cold-email segment, but its size is unknown.
- **Importer:** the REST API plus an existing open-source exporter make the importer a few days' work. Importing is not a moat.
- **Buyers are slow:** clubs are run by volunteers who change roles yearly and decide at board meetings, which slows self-serve conversion.

### Gaps
- Search volume for "WildApricot alternative" was not available.
- The share of WildApricot customers using third-party processors (and so paying the fee) is unknown.
- Current IRS counts for 501(c)(6) and (c)(7) were not found; the data is 2003–2008.
- WildApricot user Facebook groups and the community forum's activity level were not checked.

---

## Q8. I03 verdict, refined wedge, price, first-30-days plan and revenue path

### Takeaway
**Verdict: DON'T BUILD as a standalone SaaS for this founder now.** At most it is a build-if around one narrow, unverified angle: bringing Stripe autopay across intact for orgs that already pay WildApricot's 20% fee. The category is crowded with cheap and free tools that already use the "no surcharge" message. The Jan 1 2027 renewal window is effectively missed for a build starting Oct 10. And revenue arrives slowly: ~110 customers for $5k MRR and ~220 for $10k MRR, likely 12–18 and 24–36 months. Re-score: **22/40**, down from the screen's 28–29.

### Cited Findings
- Crowding at ≤$35/mo with no transaction cut, plus free Zeffy. — [MembershipWorks](https://membershipworks.com/pricing/); [Join It](https://support.joinit.com/en/articles/2772686-general-pricing-questions); [Zeffy](https://www.zeffy.com/home/membership-application-form-nonprofits-associations); [ClubExpress PDF](https://images.g2crowd.com/uploads/pricing/file/7388/What-Is-ClubExpress---Pricing.pdf)
- The 20% fee applies only to orgs using Stripe, PayPal or Authorize.net, at renewal. — [WA billing policy](https://www.wildapricot.com/legal-center/billing-and-refund-policy)
- Capterra 4.4/5 (555 reviews). — [Capterra](https://capterra.com/p/76116/WildApricot/reviews/)

### Inferences

**Re-score (judgment):**

| Criterion | Score | Reason |
|---|---|---|
| Build | 3 | Events, directory and renewals; website expectations remain |
| Regulatory | 4 | — |
| Self-serve | 3 | Board decisions, volunteer turnover |
| Distribution | 3 | SEO saturated; BuiltWith list usable |
| WTP | 3 | Anchored by $0–35 rivals |
| Gap | 1 | Crowded, cheap, no-surcharge tools exist |
| Urgency | 2 | Jan 1 window missed; the fee is a rolling trigger; no announced 2026–27 hike |
| Support | 3 | Migrations, re-collecting cards |
| **Total** | **22/40** | Kill flag "crowded with cheap indie tools" fully applies |

**If the founder still wants it, the only wedge worth testing is a "Surcharge Exit" for orgs already paying WildApricot's 20% fee:**
- Importer through the WildApricot API covering contacts, levels, renewal dates, events and invoices.
- Renewals and autopay charged on the org's own Stripe account (Connect Standard).
- An embeddable directory and events widget.
- **Test first** whether existing WildApricot-created Stripe customers and payment methods can be reused. If they can, "switch without asking members to re-enter cards" is a real differentiator no cheap rival is known to claim. If they cannot, there is no edge.
- Price: $39/mo up to 500 members and $79/mo up to 2,000, plus a $299 done-for-you migration. The migration fee brings in cash early.

**30-day plan (only if pursued):**
1. Build a BuiltWith list of live WildApricot sites (days 1–3).
2. Flag the ones with Stripe or PayPal checkout (days 3–7).
3. Email treasurers: "you're paying a 20% servicing fee at renewal — we'll move you before it renews" (days 7–30).
4. Gate: 5 paid migrations by day 30, otherwise stop.

**Revenue path (judgment):**
- Blended ~$45 ARPU means **$5k MRR ≈ 110 orgs, $10k ≈ 220 orgs.**
- Given the crowding and board-paced decisions: **$5k MRR in about 12–18 months; $10k MRR in about 24–36 months.**
- Migration fees might add $1–3k a month of one-off cash early, but that is services revenue, and it brings support load.

### Gaps
- Whether Stripe tokens are portable from a WildApricot-connected Stripe account is unverified, and the one differentiator depends on it.
- No conversion benchmarks were found for cold email to association or club treasurers.

---

## Q9. Head-to-head: which wedge should the solo founder pursue, if either?

### Takeaway
**F06 (narrowed to an ESA Receivables Ledger) is the better bet, but only behind a sell-first gate. I03 should be dropped or parked.** F06 has a public prospect list, no product found doing the job and large dollar flows per customer. Its main risk is that the pain may be smaller than assumed, because Odyssey and Step Up already run the invoice step in their portals. I03's risk is structural: a crowded, cheap category with the screen's best message already used by competitors.

### Cited Findings
- **F06:**
  - ~2,700 TEFA schools on a public map. — [Community Impact](https://communityimpact.com/katy-fulshear/education/thousands-of-katy-area-families-apply-for-new-education-accounts/)
  - In-portal invoicing on Odyssey and Step Up. — [Odyssey](https://support.withodyssey.com/hc/en-us/articles/40256443594395-Overview-Steps-Required-to-Receive-Tuition-Payments-Through-Odyssey); [Step Up](https://www.stepupforstudents.org/scholarships/private-school/fund/)
  - No ESA feature found at FACTS or Brightwheel. — [Valley Christian FAQ](https://valleychristianaz.org/wp-content/uploads/2024/09/Tuition-Payment-FAQ-24-25.pdf); [Brightwheel billing](https://intercom.help/brightwheel/en/collections/87111-billing)
- **I03:**
  - MembershipWorks at $35 with no transaction cut. — [MembershipWorks](https://membershipworks.com/pricing/)
  - Zeffy free. — [Zeffy](https://www.zeffy.com/home/membership-application-form-nonprofits-associations)
  - The 20% fee is real. — [WA policy](https://www.wildapricot.com/legal-center/billing-and-refund-policy)

### Inferences

| | F06 ESA Receivables Ledger (refined) | I03 WildApricot escape kit |
|---|---|---|
| Verdict | **Build-if** (≥8 paid pre-orders in 30 days) | **Don't build** (park; optional surcharge-exit test) |
| Rubric (new) | 29/40 (screen: 31–32) | 22/40 (screen: 28–29) |
| Price | $79 / $149 a month (founding $49), annual prepay | $39 / $79 a month + $299 migration |
| Customers for $5k / $10k MRR | ~60 / ~120 | ~110 / ~220 |
| Months to $5k / $10k (base case) | ~9–12 / ~18–24 | ~12–18 / ~24–36 |
| Biggest unknown | Do Odyssey/EMA already give per-student remittance reports? | Can Stripe autopay tokens move off WildApricot? |
| Next dated hook | Step Up Nov 1 2026; TEFA next installment Feb 1 or Apr 1 2027 (conflict) | Each org's WildApricot renewal date (rolling); fiscal-year associations in May–Jun 2027 |

- **Neither wedge produces "fast" revenue at the $10k MRR level.** If speed to first dollars matters most, F06's concierge reconciliation (a paid, hand-done service in month 1) is the quickest way to cash and to evidence.

### Gaps
- Both revenue paths rest on assumed conversion rates. No sourced benchmarks for cold email to school business offices or club treasurers were found within the search budget.
