# Validation: three "deadline compliance kit" wedges: S1-01 NY DFS Part 500 kit, E04 med-spa compliance binder, S2-01 Delaware franchise-tax fixer

Scope and method (2026-10-10):
- **Searches:** 40 web searches (the full share of the quota) and 2 GitHub repository searches.
- **Fetches failed:** direct fetches of americanmedspa.org and dfs.ny.gov returned DNS errors (ENOTFOUND). So **every web fact below comes from search-result summaries, not from fetching the pages myself.** The summaries are machine-written and can paraphrase loosely. Exact wording, dollar amounts and dates should be re-checked on the primary page before anything goes into marketing copy.
- **Corpus inputs:** the corpus files (S1-01, E04, S2-01, written Sep 24–25 2026) and the screening notes (group 3, group 5) are referenced as [S1-01], [E04], [S2-01].
- **Labels:** "(judgment)" marks my own inference. "(unverified)" marks a claim from a vendor or aggregator, or one I could only partly confirm.

---

## Q1. Trigger check: are the dated deadlines real, unchanged and in the Oct 2026–Apr 2027 window?

### Takeaway
- **S1-01:** the trigger is real and stronger than the corpus said. The amended Part 500's final phase (universal MFA, written asset inventory) took effect **Nov 1 2025**. That makes the **Apr 15 2027** certification the first one covering a full calendar year (2026) with every amended requirement in force.
- **S2-01:** the trigger is real and unchanged for corporations: **Mar 1 2027**, a $200 penalty plus 1.5%/mo, and corporate rates unchanged by HB 400. The LLC/LP/GP tax rose from $300 to $400 under HB 400 (signed May 21 2026), and the first $400 payment is due **Jun 1 2027**.
- **E04:** the trigger is weaker than the corpus said.
  - Indiana registration does start **Jan 1 2027**. But fees, forms, renewal and the adverse-event window are still pending rulemaking or conflict between sources.
  - Texas "Jenifer's Law" as enacted covers **elective IV therapy only**, not med spas in general.
  - California SB 351 is a private-equity/MSO control law, not a filing or registration trigger.

### Cited Findings

**S1-01: NY DFS 23 NYCRR Part 500**
- **Nov 1 2025 final phase.** The final set of requirements under the amended Part 500 took effect Nov 1 2025. It expanded MFA for all covered entities (500.12) and required written procedures for keeping information-system asset inventories (500.13) — [Hogan Lovells/HLC alert](https://hlc.com/en/publications/nydfs-final-set-of-cybersecurity-requirements-under-amended-part-500-take-effect-november-1-2025); [Centraleyes dates summary](https://www.centraleyes.com/nydfs-cybersecurity-regulation-dates-facts-and-requirements/)
- **May 1 2025 phase.** An earlier phase added access-management, vulnerability-management and malicious-code requirements (per a Feb 2025 DFS e-blast) — [HSF Kramer, Mar 2025](https://www.hsfkramer.com/insights/2025-03/nydfs-updates-regulated-firms-on-upcoming-cyber-requirements)
- **Limited exemption for small entities.** The amended limited-exemption thresholds are fewer than 20 employees and independent contractors (counting affiliates), OR under $7.5M gross annual revenue, OR under $15M year-end total assets — [Privacy & Security Academy training deck, Oct 2024](https://privacysecurityacademy.com/wp-content/uploads/2024/10/NY-DFS-Amended-Cybersecurity-Regulation-Overview.pdf); [Locke Lord, Dec 2022 (proposal stage)](https://lockelord.com/newsandevents/publications/2022/12/new-york-dfs-cybersecurity-regulation-update)
  - Big I NY's Nov 29 2023 slides say the employee threshold rose "from fewer than 10 to fewer than 20" — [Big I NY Gear Up slides](https://biginy.org/discover/ac/Pages/Cybersecurity/Compliance%20Resources/20231129_Gear_Up_cyber_reg_amend_slides.pdf)
  - A secondary Q&A page still shows the **old** pre-amendment thresholds (<10 staff, <$5M revenue, <$10M assets). That page is stale, so the product must not reuse such content — [securityscientist Q&A](https://answers.securityscientist.net/q/27615/what-is-nydfs-23-nycrr-500-and-who-must-comply)
- **Duties that still apply under 500.19(a).** Entities with the limited exemption still need a program and policies, access limits, a password policy, a risk assessment, a TPSP policy, MFA, an asset inventory, training and the annual notice. This was verified by the corpus against the DFS Small Business page on Sep 24 2026 — [S1-01] citing [DFS Small Business](https://www.dfs.ny.gov/cybersecurity/small-business-resources)
- **Apr 15 annual filing.** The annual Certification of Material Compliance or Acknowledgment of Noncompliance is due Apr 15. It covers the prior calendar year and is signed by the highest-ranking executive and the CISO or senior officer. The corpus verified this on DFS Submissions on Sep 24 2026 — [S1-01] citing [DFS Submissions](https://www.dfs.ny.gov/cybersecurity/submissions)
  - Big I NY confirms the yearly Apr 15 filing on the DFS website — [Big I NY](https://www.biginy.org/tag/cybersecurity-regulation/page/2)
  - The acknowledgment path includes a remediation timeline — [Kaseya](https://www.kaseya.com/blog/ny-dfs-cybersecurity-regulation/)
- **Who files the annual certification.** Big I NY says the annual certification "applies to the business entity only; it does not apply to licensed employees of an agency." Limited-exempt entities "still must submit an annual notification" — [Big I NY, "Another Resource To Help with Cyber Reg Compliance"](https://www.biginy.org/?p=1982); [Big I NY tag page](https://www.biginy.org/tag/cybersecurity-regulation/page/2)
- **Individual licensees.** Individual licensees covered by their agency's program file a **Notice of Exemption under 500.19(b)**, not their own program.
  - DFS's July 2026 instructions have a Part 3 for "entities or individual licensees qualifying for a § 500.19(b) exemption." Licensees who change employers file an amended notice naming the new employer — [DFS, Submitting or Amending a Notice of Exemption (Jul 2026 PDF)](https://www.dfs.ny.gov/system/files/documents/2026/07/Submitting-or-Amending-a%20Notice-of-Exemption_1.pdf); [DFS exemption filing instructions](https://www.dfs.ny.gov/industry_guidance/cybersecurity/exemption_filing_instructions)
  - Notices are due within 30 days of determining the exemption — [PIA "nutshell" update, 2021](https://www.pia.org/IRC/privacy/files/nutshellupdate4.2021.pdf); the 2017 DFS FAQ answers that 500.19(b) filers must file a notice — [Orrick/Buckley InfoBytes FAQ copy, Dec 2017](https://infobytes.orrick.com/wp-content/uploads/pdf/Buckley%20Sandler%20InfoBytes%20-%20NYDFS%20Update%20to%20FAQs%20re%20Cybersecurity%20Regulations%202017.12.pdf)
- **Enforcement, 2026.**
  - Delta Dental: a consent order dated Apr 30 2026 over the 2023 MOVEit incident. Reported fine $2.25M (headline; one tracker gives only a "$1M–$10M" range) — [Data Protection Report, May 2026](https://www.dataprotectionreport.com/2026/05/nydfs-fines-delta-dental-us2-25-million-over-moveit-cybersecurity-incident/); [Board Cybersecurity tracker](https://www.board-cybersecurity.com/regulatory-actions/tracker/delta-dental-insurance-regulatory-action-3c76ceae)
  - **Order Express:** a small licensed money transmitter, fined **$250,000** for an inadequate risk assessment after a 2022 ransomware attack. The date is Aug 5 2026 per Data Protection Report; a reprint shows "05/08/2026", which is ambiguous. This resolves the corpus's "(verify)" — [Data Protection Report, Aug 2026](https://www.dataprotectionreport.com/2026/08/nydfs-levies-250000-fine-on-licensee-for-inadequate-cyber-risk-assessment/); [Mondo Visione reprint](https://mondovisione.com/media-and-resources/news/new-york-state-department-of-financial-services-secures-cybersecurity-settlement-202685/)
- **Insurance-agency precedent.**
  - DFS settled with an **insurance agency for $1.9M**. The violations included **not filing certifications for 2018 and 2019**, a false 2020 certification, MFA gaps and missing audit trails. The order required a Cyber Maturity Assessment within 120 days.
  - The search summaries did not give the agency's name or the date (likely 2021–2023, judgment) — [Polsinelli](https://www.polsinelli.com/publications/new-york-department-of-financial-services-announces-a-1-9-million-settlement-with-insurance-agency-for-violations-of-new-yorks-cybersecurity-regulation); [NatLawReview](https://natlawreview.com/article/new-york-department-financial-services-announces-19-million-settlement-insurance)
- **No small-agency action in 2026.** I found **no 2026 DFS cybersecurity action against a small (<20-person) insurance agency.**

**E04: med-spa laws**
- **Indiana enactment.** Indiana's law is Senate Enrolled Act 282 (2026), also reported as Public Law 136. It was signed in March 2026 and took effect Jul 1 2026 — [Krieg DeVault](https://www.kriegdevault.com/insights/compounding-oversightnew-regulations-for-medical-spas-and-compounding-pharmacies); [NatLawReview / Epstein Becker "Interested in opening a medical spa, Part III"](https://natlawreview.com/article/interested-opening-medical-spa-part-iii-heres-more-you-need-know); [PolicyRisk bill page](https://policyrisk.com/state-bill/IN-SB282-2026)
  - The Senate passed it 47–1 in January 2026, and lawmakers finalized it around Feb 27 2026 — [Indiana Capital Chronicle, Feb 18 2026](https://indianacapitalchronicle.com/2026/02/18/medical-spas-compounded-drugs-in-focus-as-indiana-lawmakers-hear-warnings-and-pushback/); [Indiana Capital Chronicle, Feb 27 2026](https://indianacapitalchronicle.com/2026/02/27/lawmakers-finalize-indiana-oversight-plan-for-compounded-drugs-medical-spas/)
- **Registration go-live.** The **Indiana Medical Licensing Board announced on Sep 30 2026 that med-spa registrations go live Jan 1 2027.** Businesses that meet the definition register through the state professional licensing portal. Operating unregistered risks a **fine of up to $5,000**.
  - AmSpa says the Board "has not yet issued substantive guidance" on key provisions, including the scope of the physician-office exemption — [AmSpa, "Indiana Medical Board: Med Spas to Register Beginning January 1, 2027"](https://www.americanmedspa.org/?p=21347) (seen via search summary only; the fetch failed)
- **Who is covered and who is responsible.** The law covers facilities that provide medical services or prepare, administer or dispense prescription drugs for cosmetic or lifestyle treatments. Facilities that hold another state license, and physician offices, are excluded.
  - Each spa must name a **responsible practitioner** with prescriptive authority (an Indiana physician, APRN or PA) who is on-site "sufficient" time. There is no defined minimum time on site yet — [Optimantra](https://www.optimantra.com/news/indianas-new-med-spa-law-key-details-on-sb-282); [MedSpaStandards Indiana checklist, Sep 2 2026](https://medspastandards.com/blog/indiana/indiana-med-spa-compliance-checklist)
- **Rules still pending.** Fees, forms and **renewal mechanics are still in Board rulemaking**. The statute is cited as IC 25-22.5-12.5 (secondary source) — [MedSpaStandards, Sep 2 2026](https://medspastandards.com/blog/indiana/indiana-med-spa-compliance-checklist)
- **Adverse-event deadline conflict.** Sources disagree. February 2026 coverage of the bill as introduced says "five (5) days". An AmSpa piece says 15 days, which is the corpus figure, but lists it among open questions. **Unresolved** — [Indiana Capital Chronicle, Feb 18 2026](https://indianacapitalchronicle.com/2026/02/18/medical-spas-compounded-drugs-in-focus-as-indiana-lawmakers-hear-warnings-and-pushback/); [AmSpa "SB 282 has passed"](https://americanmedspa.org/news/indiana-sb-282-has-passed-what-med-spas-need-to-know)
- **Ownership.** Indiana's corporate-practice-of-medicine doctrine means a med spa must be owned by a physician or a physician-owned group (secondary, unverified) — [Consentz](https://www.consentz.com/aesthetic-license-requirements-in-indiana/)
- **Texas HB 3749 ("Jenifer's Law").** Signed Jun 20 2025 and effective Sep 1 2025. The **final version applies to elective IV therapy only**. Broader med-spa oversight in earlier drafts was struck.
  - Only physicians, PAs, APRNs or RNs may administer, under physician supervision. Ordering and prescribing is limited to physicians, or to PAs/NPs with delegated authority. One commentator says the final version may even *lessen* some restrictions.
  - I found no TMB implementing-rule text — [Polsinelli](https://www.polsinelli.com/publications/new-texas-iv-therapy-law); [Frier Levitt](https://www.frierlevitt.com/articles/client-alert-texas-medical-spas-must-prepare-for-new-regulations-on-elective-iv-therapy-effective-september-1-2025/); [HCH Lawyers](https://www.hchlawyers.com/blog/2025/may/texas-hb-3749-what-iv-hydration-clinic-owners-ne/); [House analysis](https://capitol.texas.gov/tlodocs/89R/analysis/pdf/HB03749H.pdf)
- **California SB 351.** Effective Jan 1 2026. It bars private-equity and hedge-fund control of clinical judgment in physician and dental practices, voids contracts that give management companies control of billing, coding or clinical staffing, and limits non-competes.
  - Companion AB 1415 adds MSOs, private equity and hedge funds to the 90-day notice rule of the Office of Health Care Affordability — [Benesch](https://www.beneschlaw.com/insight/california-enacts-sb-351-new-restrictions-on-private-equity-and-hedge-fund-involvement-in-physician-and-dental-practices/pdf/); [Prospyr](https://prospyrmed.com/blog/post/californias-new-pe-mso-law-what-it-really-means-for-medical-spas-and-what-to-fix-before-jan-1-2026)
- **Other states.** Status is as of early 2026 and may be stale — [Epstein Becker Health Law Advisor](https://www.healthlawadvisor.com/interested-in-opening-a-medical-spa-part-iii-heres-more-that-you-need-to-know); [Quarles](https://www.quarles.com/newsroom/publications/med-spa-compliance-series-area-of-focus-proposed-med-spa-facility-licensure-requirements-in-iowa-and-indiana); [Nevada Medical Board agenda item 4(1), 2026](https://medboard.nv.gov/uploadedFiles/medboardnvgov/content/About/Board/2026/Agenda%20Item%204(1).pdf)
  - **Iowa HSB 591:** proposes Board of Medicine licensure; introduced Jan 20 2026.
  - **Arizona HB 4047:** proposes Pharmacy Board licensure where prescription drugs are handled; introduced Feb 10 2026.
  - **Florida:** a bill requiring an on-site responsible person was proposed (the corpus says SB 1728 failed Mar 13 2026).
  - **Nevada:** a draft med-spa registry for the 2027 session, with an effective date of Jan 1 2028.
  - **Rhode Island:** the Medical Spas Safety Act took effect Jun 30 2025.
  - **Colorado and Massachusetts** are named as states to watch.
- **Enforcement attention.** Holland & Knight published "Medical spa compliance under the microscope" on Aug 5 2026 (title only; contents not seen) — [H&K](https://hklaw.com/en/insights/publications/2026/08/medical-spa-compliance-under-the-microscope)

**S2-01: Delaware franchise tax**
- **Mar 1 deadline and penalty.** Annual reports and taxes must be received by **Mar 1** each year. The penalty is $200 plus 1.5%/mo interest. The domestic-corporation filing fee is $50 ($25 for non-profits).
  - The minimum tax is $175 under Authorized Shares or $400 under Assumed Par Value Capital (APVC). The maximum is $200,000, or $250,000 for a Large Corporate Filer.
  - Filers owing **$5,000 or more** pay quarterly installments: 40% Jun 1, 20% Sep 1, 20% Dec 1, and the remainder Mar 1 — [Delaware Division of Revenue franchise tax page](https://revenue.delaware.gov/franchise-tax/)
- **Charter voidance.** Not filing or paying for more than a year can void the charter — [Wolters Kluwer, Jan 27 2026](https://www.wolterskluwer.com/es/expert-insights/delaware-corporations-annual-franchise-report-and-tax-requirement)
- **HB 400.** Signed **May 21 2026**. It raises the **LLC/LP/GP annual tax from $300 to $400**, retroactive to Jan 1 2026, and series fees from $75 to $100. Most other filing-fee increases took effect **Aug 1 2026**.
  - The **first $400 payment is due Jun 1 2027.** The Jun 1 2026 payment for 2025 was still $300 — [Withum](https://www.withum.com/resources/delaware-businesses-face-increased-annual-taxes-and-filing-costs/); [InCorp](https://www.incorp.com/resources/knowledge-base/delaware-business-filing-fee-increase); [Bloomberg Tax](https://news.bloombergtax.com/daily-tax-report-state/delaware-increases-secretary-of-state-entity-fees-annual-taxes); [Beancount guide, Jul 20 2026](https://beancount.io/blog/2026/07/20/delaware-hb400-llc-partnership-annual-tax-300-to-400-2026-guide)
  - This resolves the corpus's "(verify)" on when the LLC tax rose.
- **HB 400 does not change corporate franchise-tax rates, minimums or maximums.** The foreign-corporation annual report fee rose from $125 to $250 and the late penalty from $125 to $200, effective Aug 1 2026 — [Delaware Inc. blog on HB 400](https://www.delawareinc.com/blog/delaware-franchise-tax-update-hb-400/); [Discern calculator page](https://www.discern.com/resources/delaware-franchise-tax-calculator); [Maples](https://maples.com/knowledge/delaware-house-bill-400-introduces-new-fee-changes); [Capitol Services](https://www.capitolservices.com/insights/alerts/e-alert-delaware-fee-and-annual-tax-changes/)
- **The $85,165 notice.** 10M authorized shares gives about **$85,165** under Authorized Shares, against **$400** under APVC. Winstead's example has 9M issued shares and $100k gross assets.
  - The state's notice defaults to Authorized Shares because Delaware lacks the gross-asset data.
  - The eCorp filing lets the filer enter gross assets and issued shares to switch methods — [Winstead alert](https://m.winstead.com/portalresource/lookup/wosid/cp-base-4-107204/overrideFile.name=/DE%20Franchise%20Tax%20Alert.pdf); [Clerky help](https://help.clerky.com/article/2796-calculate-delaware-franchise-tax); [Gust](https://gust.com/blog/delaware-franchise-taxes/)
  - Rho cites an $85,215 notice against $850 actually owed — [Rho](https://www.rho.co/blog/delaware-franchise-tax)
- **When APVC fails to save.** APVC saves money only when issued shares are a meaningful fraction of authorized shares, roughly 30–50% per one source — [Foothold America](https://www.footholdamerica.com/blog/delaware-franchise-tax-why-your-bill-says-85000-and-how-to-fix-it/)
  - Commercial formation vendors often default to 10M authorized shares — same source.
- **Statutory basis.** The statute counts authorized shares — [8 Del. C. § 503 (Justia)](https://law.justia.com/codes/delaware/title-8/chapter-5/section-503)

### Inferences
- **S1-01 marketing hook (judgment).** "Your Apr 15 2027 filing is the first one that certifies a full year under universal MFA and asset inventory." The rules for calendar 2026 are fully phased in, so an honest "Certification of Material Compliance" now needs evidence for every element. That is the strongest dated hook of the three ideas.
- **S1-01 scope correction.** Licensed *employees* of an agency do not file the annual certification; they file 500.19(b) notices. The buyer is the agency entity, plus sole-proprietor producers who are their own covered entity.
  - A small, sticky feature (judgment): an **agency roster tracker** that confirms each licensed employee's 500.19(b) notice names the agency and is amended when people join or leave.
- **E04 corrections.** The corpus's "Texas ordered-by/administered-by records" duty is tied to *elective IV therapy*, not every med-spa service.
  - California SB 351 creates contract and ownership restructuring work (lawyers' work), not a recurring filing that software can own.
  - Indiana is the only real dated registration in the window, and its renewal frequency and fee are not yet set. So nobody can yet say whether it creates *recurring* demand (judgment).
- **E04 exemption risk (judgment).** If the physician-office exemption is read broadly, and Indiana CPOM already pushes ownership to physicians, fewer Indiana businesses may have to register than the definition implies.
- **S2-01.** The deadline and the pain are both real, and both are thoroughly documented by free sources (see Q2).

### Gaps
- **Fetches failed.** I could not read the current DFS FAQ text on whether 500.19(b) individual filers must also file anything annually (the 2017 FAQ and the Jul 2026 instructions only confirm the Notice of Exemption). The dfs.ny.gov fetch failed.
- **Agency not named.** The $1.9M insurance-agency settlement's name and date were not in the summaries.
- **Indiana adverse-event window.** Whether it is 5 or 15 days, whether registration is annual or biennial, the fee, and whether the report needs patient identifiers (which decides PHI exposure) all wait on Board rules. AmSpa's Sep 30 2026 article could not be fetched.
- **Texas rules.** No TMB rule text (Rule 169.x) implementing HB 3749 was found.
- **Florida 2027 refiling.** Not checked.

---

## Q2. Competitor sweep: who already sells this, and at what price?

### Takeaway
- **S1-01:** the cheap end is free or nearly free, and the mid-market is enterprise-priced. DFS gives away a small-business Program Template and an "Am I Exempt" flowchart. Big I NY gives members a limited-exemption checklist. Template kits sell for about $249 one-time. GRC platforms (Drata now supports Part 500) cost about $10k+/yr, and MSPs quote per engagement. **I found no self-serve $30–60/mo SaaS aimed at small NY agencies.** The gap is real, but the free DFS template caps what "templates" alone can charge.
- **E04:** crowded with bundled or near-free alternatives. Moxie's Compliance Defender (protocols, standing orders, GFE alerts, protocol-expiry alerts) comes inside its med-spa platform. AmSpa Plus ($634/yr) includes a delegation table, consent templates and an attorney consult. Content sites already publish Indiana checklists.
- **S2-01:** saturated with free tools. At least 8 firms publish free calculators or how-tos, Stripe Atlas tells users how to recalculate, and accountants bundle the filing. An indie developer pushed an identical "check if you're overpaying" open-source tool on **Oct 3 2026**.

### Cited Findings

**S1-01 competitors**
- **DFS Cybersecurity Program Template (free).** Published with a **May 13 2024** industry letter. It targets small licensees with a 500.19(a) limited exemption and individually owned businesses, including insurance agencies.
  - It includes frameworks for asset inventories, risk assessments, MFA exceptions and third-party providers, plus a small-business implementation timeline.
  - DFS says completing it "does not assure compliance." DFS also publishes an "Am I Exempt" flowchart — [DFS Program Template](https://www.dfs.ny.gov/cybersecurity/Program-Template); [DFS industry letter May 13 2024](https://www.dfs.ny.gov/industry-guidance/industry-letters/il20240513-resources-cyber-small-businesses-guidance); [Big I NY "NYS DFS Offers New Cyber Program Template"](https://www.biginy.org/news/ask-tim-news/nys-dfs-offers-new-cyber-program-template/); [ResourcePro bulletin](https://www.resourcepro.com/bulletin/new-york-announces-resource-to-assist-small-businesses-with-development-of-cybersecurity-program/)
- **Big I NY (IIABNY).** A members-only limited-exemption checklist, a 7-page cyber-reg FAQ, a TPSP questionnaire (2019 metadata), and IAAC TPSP questionnaire responses for 2026 — [Big I NY](https://www.biginy.org/?p=1982); [Big I NY FAQ post](https://www.biginy.org/news/ask-tim-news/new-cyber-reg-faq-document/); [IAAC TPSP Response 2026](https://www.biginy.org/wp-content/uploads/sites/27/2026/01/IAAC-TPSP-Questionnaire-Response-2026.pdf)
  - In 2016 IIABNY warned that compliance could cost some agencies more than $100,000 — [Big I NY 2016](https://www.biginy.org/news/Pages/2016/111416.aspx)
- **Template sellers.**
  - The Art of Service sells a "NY DFS 23 NYCRR 500 Cybersecurity Evidence & Implementation Kit" for **$249** (claims "18 requirements as adopt-ready controls"; unverified) — [store.theartofservice.com](https://store.theartofservice.com/ny-dfs-23-nycrr-500/)
  - Security Scientist offers a free Word policy template behind a form — [securityscientist.net](https://www.securityscientist.net/blog/nydfs-500-cybersecurity-policy-template/)
  - ComplianceForge has a 23 NYCRR 500 explainer; its kit price was not verified — [ComplianceForge](https://complianceforge.com/what-is-23-nycrr-500)
- **GRC platforms.**
  - **Drata announced Part 500 support in Nov 2025** — [Drata update](https://drata.com/updates/drata-supports-nydfs-part-500)
  - Third-party price estimates (unverified): Drata about $15k–$100k/yr and Vanta about $10k–$80k/yr per one comparison; average SMB spend of about $34.5k (Drata) and $29k (Vanta) per another; Vanta's entry tier about $10k/yr — [Costbench](https://www.costbench.com/compare/drata-vs-vanta/); [SpendHound](https://www.spendhound.com/marketplace/vanta-pricing)
  - I found no confirmation that Vanta supports Part 500.
  - LogicManager, Saltycloud Isora GRC, Mitratech/Prevalent and Thoropass (a service model) all market Part 500 tooling with no small-agency pricing — [LogicManager](https://www.logicmanager.com/?p=113371); [Isora GRC](https://www.saltycloud.com/isora-grc/solutions/nydfs-23-nycrr-500-compliance-software/); [Mitratech checklist](https://grc.mitratech.com/nydfs-23-nycrr-500-compliance-checklist); [Thoropass](https://thoropass.com/?p=756)
- **MSPs and consultants serving agencies, none with a published price.** Kite Technology ("keeps your insurance agency compliant"), LISS Technologies (IT for insurance agencies), CCSI (assessment, vCISO, managed SIEM, training), M.A. Polce (program, CISO, pen test, risk assessment, IR plan) and Tevora (four-phase approach) — [Kite](https://www.kitetechgroup.com/?p=879); [LISS](https://lisstech.com/industry/insurance-agencies/); [CCSI](https://www.ccsinet.com/cybersecurity/nysdfs-cybersecurity-assessment/); [Polce](https://mapolce.com/?p=7507); [Tevora](https://tevora.com/?p=12622)
- **Open source.** A GitHub search for "nydfs part 500" returned 1 documentation-only repo (a control crosswalk, Sep 2026). There are no open-source agency kits — [celsoreic/capital-markets-cyber-controls](https://github.com/celsoreic/capital-markets-cyber-controls)
- **Not checked.** The brief named "Carbide" and "Cyber Guardian". I ran **no search** on them, so their presence or pricing is unknown.

**E04 competitors**
- **Moxie Compliance Defender.** Bundled in Moxie Suite. It tracks compliance across charts, protocols and "foundational documents"; supplies templated protocols and standing orders for sign-off; alerts on GFE status, overdue charts and expiring protocols; tracks injectable lots and expiry; and checks advertising language.
  - **No standalone price is published.** One source describes performance-based pricing with no fixed monthly fee, but it is unclear which offering that covers.
  - Moxie raised a $10M Series B, announced alongside the Compliance Defender launch, and reportedly a $25M Series C in Mar 2026 (aggregator; unverified) — [Moxie compliance page](https://www.joinmoxie.com/compliance); [Moxie compliance tools](https://joinmoxie.com/medspa-compliance-tools); [Moxie blog](https://joinmoxie.com/post/introducing-moxie-compliance-defender); [AmSpa news on Series B](https://americanmedspa.org/news/moxie-raises-10-million-series-b-to-scale-its-leading-medspa-management-platform-launches-compliance-defender-product); [yespress](https://yespress.io/moxie)
- **AmSpa membership (2026).**
  - Basic is **$297/yr** (list $395) and includes a free ByrdAdatto attorney consultation once per 365 days and a basic state legal summary.
  - Plus is **$634/yr** (list $845) and adds a Treatment Delegation Table and Intake & Consent Form Templates.
  - The site also lists an Injectables Practice Toolkit, an IV Therapy Toolkit, and Forms, Consents & SOPs.
  - The promo code expired Apr 12 2026 — [AmSpa Medical Spa Show 2026 membership rates](https://www.americanmedspa.org/?p=19623)
- **MedSpaStandards.com.** Publishes a 16-minute Indiana compliance checklist (Sep 2 2026) that marks items "legally required / pending rulemaking / recommended", an operations-and-compliance section, and a Jun 8 2026 medical-director cost and agreement guide. **Whether it sells software, and at what price, is unknown** — [Indiana checklist](https://medspastandards.com/blog/indiana/indiana-med-spa-compliance-checklist); [Ops & compliance](https://medspastandards.com/operations-compliance); [MD cost 2026](https://medspastandards.com/blog/med-spa-medical-director-cost-agreement-2026)
- **EHR and booking vendors.**
  - Accountable sells HIPAA med-spa scheduling, charting and versioned consents — [Accountable](https://www.accountablehq.com/post/all-in-one-medical-spa-business-compliance-solutions-to-stay-legal-and-audit-ready)
  - Optimantra (EHR) publishes Indiana SB 282 content — [Optimantra](https://www.optimantra.com/news/indianas-new-med-spa-law-key-details-on-sb-282)
  - Aesthetic Record runs a marketplace with "compliance" and "GFE" product tags — [AR marketplace compliance](https://market.aestheticrecord.com/product-tag/compliance); [AR GFE](https://market.aestheticrecord.com/product-tag/gfe)
- **GFE and medical-director services.**
  - GFEase by Docovia charges a flat rate per virtual GFE with no setup, monthly or per-location fee (the rate was not shown) — [Docovia GFEase](https://docovia.com/gfease)
  - Jevy sells GFE packs at $6,250 and $12,500 bundles — [AR marketplace GFE](https://market.aestheticrecord.com/product-tag/gfe)
  - Medical-director retainers run **$2k–$4k/mo remote** and $4k–$7k on-site, with another source saying $1.5k–$8k/mo, or $50–$200 per treatment — [inhouse.ai](https://www.inhouse.ai/med-spa-compliance/how-much-does-a-medical-director-cost)
- **A startup pitch page** claims "no existing software product addresses more than one of these domains." This is a pitch, not evidence — [liveinthefuture.org](https://liveinthefuture.org/startups/medspa-regulatory-compliance-saas.html)

**S2-01 competitors**
- **Free calculators and how-tos.**
  - Kruze Consulting has a free two-method calculator; its clients typically pay $400–$10k/yr — [Kruze](https://kruzeconsulting.com/blog/post/delaware-franchise-tax)
  - Delaware Inc. has a calculator — [delawareinc.com](https://delawareinc.com/delaware-franchise-tax-calculator)
  - Discern has a 2026 calculator — [Discern](https://www.discern.com/resources/delaware-franchise-tax-calculator)
  - Zenind has a calculator guide — [Zenind](https://www.zenind.com/help/post/delaware-franchise-tax-calculator-how-to-estimate-your-annual-tax)
  - Clerky has a help article — [Clerky](https://help.clerky.com/article/2796-calculate-delaware-franchise-tax)
  - Capbase — [Capbase](https://capbase.com/no-your-startup-doesnt-owe-thousands-of-dollars-in-delaware-franchise-tax/)
  - Gust's "Don't Panic … $85,165" — [Gust](https://gust.com/blog/delaware-franchise-taxes/)
  - Cooley GO — [Cooley GO](https://www.cooleygo.com/so-you-owe-thousands-in-delaware-franchise-tax/)
  - Mintz, Feb 13 2026 — [Mintz](https://www.mintz.com/insights-center/viewpoints/2911/2026-02-13-no-you-dont-owe-delaware-200000-de-franchise-tax-101)
  - Rho — [Rho](https://www.rho.co/blog/delaware-franchise-tax)
  - Pilot — [Pilot](https://pilot.com/blog/how-to-file-your-delaware-franchise-tax-on-time)
  - Foothold America — [Foothold](https://www.footholdamerica.com/blog/delaware-franchise-tax-why-your-bill-says-85000-and-how-to-fix-it/)
  - Vicente LLP — [Vicente](https://vicentellp.com/insights/avoiding-massive-delaware-franchise-tax-bills)
- **Stripe Atlas docs** tell Atlas companies they can recalculate on the state site and that most pay less with APVC (no tax advice) — [Stripe Atlas docs](https://docs.stripe.com/atlas/business-taxes)
- **Bundled services.**
  - Fondo markets automating Delaware franchise-tax filings with APVC inside its "TaxPass" bookkeeping and tax subscription (no price shown) — [Fondo](https://fondo.com/blog/the-indispensable-tool-for-automating-delaware-franchise-tax-filings-with-assumed-par-value)
  - **Harbor Compliance's managed Delaware annual report costs $199 per state plus state fees** — [Harbor Compliance](https://www.harborcompliance.com/delaware-annual-report)
  - Corpus figures: Harbor registered agent $99 intro → $159 renewal, Northwest $125, Stripe Atlas $100/yr after year one (fetched Sep 24 2026) — [S2-01]
- **AI and open source.**
  - An "open-agreements" Delaware franchise-tax skill is listed on Smithery — [smithery.ai](https://smithery.ai/skills/open-agreements/delaware-franchise-tax)
  - GitHub search "delaware franchise tax" returned 6 repos, including:
    - **captainchaitanya/founder-desk** (created **Oct 3 2026**: "Check if you're overpaying Delaware franchise tax. Compares both official methods.") — [GitHub](https://github.com/captainchaitanya/founder-desk)
    - alanhamlett/de-franchise-tax-payer ("Pay Delaware franchise tax from the command line", Feb 2026) — [GitHub](https://github.com/alanhamlett/de-franchise-tax-payer)
    - thatfield-916/de-corp-fee-calculator (Apr 2026) — [GitHub](https://github.com/thatfield-916/de-corp-fee-calculator)
    - two 2017 calculators — [GitHub](https://github.com/richsapien/DE-franchise-tax-calculator)
- **Source conflict on the minimum.** Pilot says the APVC minimum is $450, probably $400 tax plus the $50 fee, against $400 elsewhere — [Pilot](https://pilot.com/blog/how-to-file-your-delaware-franchise-tax-on-time); [Kruze](https://kruzeconsulting.com/delaware-franchise-tax/)

### Inferences
- **S1-01 (judgment).** The DFS template turns "policy pack" into a commodity. What sells is **doing and proving the work**: a pre-filled version of DFS's own template, MFA and asset evidence collection, training certificates, the two-signer packet, Apr 15 reminders and a receipt vault, all priced below an MSP engagement.
  - The main substitutes are an agency's existing MSP and "tick the box" self-certification.
  - Drata's Part 500 support doesn't threaten a 5-person agency; at about $10k+/yr it targets bigger buyers.
- **E04 (judgment).** A standalone "binder" sits between three players:
  - Moxie, which bundles compliance into the platform spas already pay for;
  - AmSpa, whose $634/yr membership covers templates and a lawyer;
  - GFE and medical-director services, which own the relationship and the clinical sign-off.
  - Buyers' biggest compliance spend is the medical director at $1.5k–$8k/mo, not software. The natural owner of a binder is therefore that service provider, which makes them a channel at best and a competitor at worst.
- **S2-01 (judgment).** The calculator itself is worth $0. The "full job" (prep, reminders, receipts) is a $199 service at Harbor or a free feature at startup accountants. Another indie developer shipped the same open-source idea a week ago. This meets the rubric's "crowded with cheap indie tools" kill flag.

### Gaps
- **Prices not found:** ComplianceForge NYDFS kit; NY MSP Part 500 packages (no public prices); Moxie Suite and Compliance Defender; MedSpaStandards' paid offering (if any); GFEase per-exam rate; LegalZoom annual-report service.
- **Not searched:** Carbide, Cyber Guardian, PIANY member tools, AMS-vendor modules (Applied, Vertafore), carrier or E&O cyber programs for agencies.

---

## Q3. Buyers and reachability: how many buyers, and can one person reach them?

### Takeaway
- **S1-01:** there are tens of thousands of NY licenses, but **no free bulk licensee list was found**. Agencies have to be reached through Big I NY/PIANY, MSPs, SEO or scraped directories.
- **E04:** the US has about 10–11k med spas, but **Indiana's count is unknown** and probably only in the low hundreds (estimate).
- **S2-01:** the buyer pool is huge (2.28M entities, 74,716 new corporations in 2025) and easy to reach by SEO, but it is served for free.

### Cited Findings
- **S1-01 market size.**
  - A NYSID report (year not stated) counts **117,497 licenses** issued by DFS to adjusters, agents, brokers, consultants, reinsurance intermediaries and service-contract registrants — [WorkersCompensation.com / NYSID](https://www.workerscompensation.com/sponsored-content/nysid-reports-32-m-in-consumer-recoveries/)
  - An aggregator claims over 150,000 active NY property/casualty producer licenses (unreliable) — [Gitnux](https://gitnux.org/new-york-insurance-industry-statistics/)
  - Nationally, an NAIC summary gives about 2.2M resident individual producers and **236,033 resident producer entities** (year not stated) — [insurance-forums.com NAIC summary](https://insurance-forums.com/practice-building/interesting-industry-facts-and-figures-from-new-naic-report/)
  - DFS supervises 1,900+ insurers and 1,300+ banks and financial institutions — [S1-01] citing DFS About
- **S1-01 lists.** No DFS insurance-licensee dataset turned up on data.ny.gov. NY publishes real-estate licensees there, but not insurance producers in these results. The DFS Licensing Bureau contact is licensing@dfs.ny.gov — [data.gov real estate dataset](https://catalog.data.gov/dataset/active-real-estate-salespersons-and-brokers); [NYC Business DFS licensing contact](https://ko.nyc-business.nyc.gov/nycbusiness/description/excess-line-broker-license-entity)
- **S1-01 MSP channel.** MSPs are themselves third-party service providers under 500.11, so MSPs serving agencies have their own reason to show conformity — [Secure Controls Framework blog](https://securecontrolsframework.com/blog/it-service-provider-requirements-under-ny-dfs-23-nycrr-500); [Kaseya](https://www.kaseya.com/blog/ny-dfs-cybersecurity-regulation/)
- **S1-01 confusion signal.** Trade press has long described individual-licensee filing as "administrative headaches", including DFS requiring all licensees to resubmit exemption notices when a new portal launched (2017–2018 era) — [IA Magazine](https://www.iamagazine.com/?p=4092); [Arnold & Porter, Mar 2018](https://www.arnoldporter.com/en/perspectives/publications/2018/03/nydfs-issues-guidance-for-individual-filers)
  - No Reddit or forum threads surfaced in search.
- **E04 US count.**
  - 10,488 US med spas in 2023 — [S1/E04 corpus citing AestheticHires](https://www.aesthetichires.com/med-spa-industry-statistics/)
  - A third-party report surfaced in search says about **11,200 in 2024**, with 14,400 projected for 2028 (unverified; the originating page in the results was unclear) — [Webtonic](https://www.webtonic.io/blog/med-spa-aesthetics-demand-generation-statistics)
  - AmSpa: an industry of $17B+, growing more than $1B/yr. The **2026 AmSpa survey was still collecting responses**, so there is no new official count — [AmSpa research](https://www.americanmedspa.org/med-spa-statistics); [AmSpa 2026 survey notice](https://www.americanmedspa.org/?p=21167)
- **E04 revenue.** Single-location average revenue was $1.4M in 2024, and a vendor claim puts it at $1.8–2M in 2026 — [Boulevard](https://www.joinblvd.com/blog/average-medical-spa-revenue)
- **E04 Indiana count.** **No Indiana med-spa count was found.** AmSpa's Feb 5 2026 letter to the Indiana House Public Health committee exists, but its content was not visible — [AmSpa letter](https://info.americanmedspa.org/hubfs/Legislative%20Material/Indiana/2026/AmSpa_Ltr%20to%20House%20Public%20Health.02-05-26_final.pdf)
- **S2-01 market.** More than 2.28M Delaware entities. 334,461 were formed in 2025, including 74,716 corporations and 235,393 LLCs. The corpus verified this on corp.delaware.gov/stats on Sep 24 2026 — [S2-01]
- **S2-01 default trap.** Many startups formed through commercial document vendors default to 10M authorized shares, which drives the $85k notices — [Foothold America](https://www.footholdamerica.com/blog/delaware-franchise-tax-why-your-bill-says-85000-and-how-to-fix-it/)

### Inferences
- **S1-01 buyer count (judgment).** If even 5–10% of NY licenses belong to agency entities or sole-proprietor covered entities, the buyer pool is in the low thousands to about 10k.
  - Reaching them is the binding constraint. Big I NY's "Ask Tim" column and its member checklist show the association is the trusted channel, and it already gives away a partial substitute.
- **E04 Indiana estimate (judgment, estimate only).** Indiana has about 2% of the US population. That implies roughly 200–250 med spas, plus IV-hydration and GLP-1 clinics that fit the broad definition, minus physician offices if the exemption is read broadly. That is too few buyers for a standalone product.
- **S2-01 (judgment).** Reach is easy (SEO, Show HN, accelerator perks), but the same reach is already owned by Clerky, Kruze, Pilot, Stripe and law firms ranking for the same queries.

### Gaps
- **Bulk lists.** I don't know whether DFS will provide a bulk licensee extract on request or by FOIL. I don't know Big I NY's or PIANY's member-agency counts.
- **Counts.** No Indiana (or Texas) med-spa counts and no state association list were found. No count of startup-focused CPA firms was found.

---

## Q4. Willingness to pay, pricing and demand signals

### Takeaway
- **S1-01 has the best WTP evidence of the three.** The alternatives are MSP engagements, $10k+/yr GRC platforms, or a $1.9M precedent for not filing. But the floor is the free DFS template, so $390–590/yr per agency is the credible band.
- **E04's WTP sits with services** (medical directors at $1.5k–8k/mo, AmSpa at $297–634/yr), not with standalone binder software.
- **S2-01's WTP is about zero for software.** Founders pay accountants and agents ($199/filing at Harbor) or use free calculators.

### Cited Findings
- **S1-01.** The $249 one-time kit sets a template-kit price point — [Art of Service](https://store.theartofservice.com/ny-dfs-23-nycrr-500/). GRC entry starts around $10k/yr (estimates) — [SpendHound](https://www.spendhound.com/marketplace/vanta-pricing).
  - The corpus proposed $19/mo solo, $59/mo agency, a $299 done-with-you add-on, and $15/agency/mo for MSPs — [S1-01]
  - The penalty precedent is the $1.9M agency settlement that included not filing — [Polsinelli](https://www.polsinelli.com/publications/new-york-department-of-financial-services-announces-a-1-9-million-settlement-with-insurance-agency-for-violations-of-new-yorks-cybersecurity-regulation)
  - Order Express ($250k) shows DFS will fine smaller licensees over a weak risk assessment — [Data Protection Report](https://www.dataprotectionreport.com/2026/08/nydfs-levies-250000-fine-on-licensee-for-inadequate-cyber-risk-assessment/)
- **E04.** AmSpa Basic $297/yr and Plus $634/yr — [AmSpa](https://www.americanmedspa.org/?p=19623); medical director $2k–$4k/mo remote — [inhouse.ai](https://www.inhouse.ai/med-spa-compliance/how-much-does-a-medical-director-cost).
  - The corpus proposed $49–79/mo per location or a $49 one-time Indiana kit — [E04]; group 3 screen.
  - Med spas spend about 7% of revenue on marketing (AmSpa survey cited by a marketing blog) — [Webtonic](https://www.webtonic.io/blog/med-spa-aesthetics-demand-generation-statistics)
- **S2-01.** Harbor's managed annual report is $199 plus state fees — [Harbor](https://www.harborcompliance.com/delaware-annual-report). Kruze clients typically owe $400–$10k/yr in tax — [Kruze](https://kruzeconsulting.com/blog/post/delaware-franchise-tax). The corpus proposed $49/yr per entity and $299/yr for a 25-entity firm plan — [S2-01].
  - Many law firms advise "call your lawyer before paying" — [Wyrick Ventures](https://ventures.wyrick.com/blog/delaware-franchise-tax-dont-panic)
- **Demand signals.** Search found **no Reddit or forum threads** for any of the three. That doesn't mean demand is absent, since Reddit was not indexed well in these results.
  - S2-01 draws a steady stream of "Don't panic, you don't owe $85k" articles from law firms and fintechs every Jan–Feb (Mintz Feb 13 2026; Gust; Capbase; Rho). That shows recurring search demand already being captured by free content — [Mintz](https://www.mintz.com/insights-center/viewpoints/2911/2026-02-13-no-you-dont-owe-delaware-200000-de-franchise-tax-101)

### Inferences
- **S1-01 price (judgment).** Agency (≤20 staff) at **$490/yr** prepaid, with a $39/mo option. Solo producer or sole proprietor at **$149/yr**. A "Reviewed by a cyber pro" add-on at $390, delivered through a partner MSP. The corpus's $19/mo solo tier is too low for a yearly job.
- **E04 price (judgment).** Anything above about $49/mo has to beat AmSpa Plus at $634/yr (about $53/mo), which comes with a lawyer. A software-only binder would struggle to charge more than $29–49/mo.
- **S2-01 price (judgment).** A $49/yr per-entity subscription fights $0. A firm plan has to beat accountants' existing spreadsheets.

### Gaps
- No direct WTP evidence (surveys, pre-sales, forum complaints) was found for any of the three. Pre-selling is the only way to get it.

---

## Q5. Liability: disclaimers, unauthorized practice of law (UPL) and standard limits

### Takeaway
None of the three is a UPL or licensing blocker if the product stays a "mail-merge" tool. That means it fills the regulator's own forms and templates from user answers, shows its formulas and inputs, and gives no individualized legal advice. Courts in the LegalZoom cases looked at **whether the tool exercises judgment**, not at the disclaimer. Every incumbent uses "not legal or tax advice; does not assure compliance" language. **E04 carries the most risk.** Clinical protocols and standing orders need physician and attorney sign-off, and an adverse-event log could become PHI.

### Cited Findings
- **South Carolina.** The referee report adopted by the SC Supreme Court found LegalZoom "does not exercise any judgment or discretion, but operates automatically in the same fashion as a 'mail merge' program." Commentators call the holding narrow — [ABA Journal](https://www.abajournal.com/news/article/legalzoom_business_model_okd_by_south_carolina_supreme_court); [Josh Blackman, May 2014](https://joshblackman.com/blog/2014/05/20/legalzoom-has-carolina-on-its-mind/)
- **North Carolina.** The NC Bar settled with LegalZoom: automated document services do not violate NC law **if they register and follow consumer-protection procedures** — [Wikipedia: LegalZoom](https://en.wikipedia.org/wiki/LegalZoom); [Goldberg Segalla](https://www.goldbergsegalla.com/blog/professional-liability-matters/ethics/legal-zooms-business-model-prompts-ethical-debate/)
- **Missouri.** The 1978 Missouri Supreme Court divorce-kit decision held that selling forms is not practicing law absent "personal advice as to legal remedies"; Janson v. LegalZoom rested on that line of cases — [Wikipedia: LegalZoom](https://en.wikipedia.org/wiki/LegalZoom)
- **Standard disclaimers in this space.**
  - DFS: its template completion "does not assure compliance" — [DFS Program Template](https://www.dfs.ny.gov/cybersecurity/Program-Template)
  - Big I NY's questionnaire: "the services of an appropriate, competent professional should be sought" — [Big I NY](https://www.biginy.org/?p=1982)
  - Stripe Atlas: it doesn't give tax or legal advice — [Stripe Atlas docs](https://docs.stripe.com/atlas/business-taxes)
  - Delaware Inc.'s calculator: "only an estimate" — [Delaware Inc](https://delawareinc.com/delaware-franchise-tax-calculator)
- **E04 template risk.** One law-firm blog says Texas requires written, signed, site-specific standing delegation orders. This is a single secondary source, and the search summary didn't say which result it came from; most likely it is D.J. Holt Law — [djholtlaw.com "Audit-proofing your med spa"](https://djholtlaw.com/audit-proofing-your-med-spa-before-it-becomes-necessary/) (attribution unverified)
  - The corpus itself says templates must be attorney-reviewed and that a cash-only spa "may not technically be a HIPAA covered entity" — [E04]

### Inferences (all judgment)
- **S1-01.** Low risk. The wizard should map answers to DFS's own published exemption categories and flowchart and cite the DFS text.
  - The customer, not the tool, signs and submits the certification.
  - Offer a one-click "Acknowledgment of Noncompliance" path so the tool never pushes a false certification. The $1.9M precedent included a false certification.
  - Carry tech E&O insurance.
- **E04.** Medium-high risk.
  - Standing orders and protocols are clinical-legal documents, so ship them only as "your medical director edits and signs" shells, or license attorney-drafted state packs.
  - Keep the adverse-event log free of identifiers until Indiana's rules show what the report requires.
  - North Carolina's registration rule for online document providers may also apply if sold there.
- **S2-01.** Low legal risk: it applies published state tables and the user files. The accuracy risk is real, though; a wrong APVC input such as gross assets could underpay. Show every input, require confirmation, and use "estimate, verify with your CPA" language like the incumbents.

### Gaps
- **Not researched:** current state UPL statutes for software (NC registration details, Texas's 1999 safe harbor); whether NY treats compliance-program templates as legal services; insurance costs for tech E&O.

---

## Q6. Verdicts: refined wedge, price, first-30-days sales plan, revenue path and seasonality/churn

### Takeaway
| | S1-01 NY DFS Part 500 kit | E04 Med-spa compliance binder | S2-01 Delaware franchise-tax fixer |
|---|---|---|---|
| **Verdict** | **Build-if.** Build only if ≥10 paid pre-orders, or one association/MSP partner, by ~Nov 10 2026 | **Don't build now.** Revisit only if Indiana's rules make registration recurring and 2027 sessions pass laws in more states, or if a GFE or medical-director service wants to white-label it | **Don't build** as a business. At most, a free calculator as SEO bait inside a broader entity-compliance product |
| **Updated rubric score (judgment)** | 27/40 (was 29): distribution 2, gap 3 | 24/40 (wedge; was ~29): gap 2, distribution 2, urgency 3 | 26/40 nominal (was 29), but WTP 1 and gap 1, with the CROWD kill flag confirmed |
| **Refined wedge** | "Apr 15 Filing Kit" for NY agencies under 20 staff: the DFS template pre-filled and evidenced, plus an employee 500.19(b) roster tracker | An Indiana SB 282 registration-readiness checklist plus a license and protocol-expiry tracker (non-PHI) | A two-method calculator plus a filing worksheet for startup CPAs |
| **Price** | $490/yr agency, $149/yr solo, $390 pro-review add-on | $49 one-time kit, then $29–49/mo | $299/yr firm plan, $49/yr per entity (low demand) |
| **$5k / $10k MRR needs** | ~123 / ~245 agencies at $490/yr (or ~148 / ~297 with a blended mix of agency and solo plans) | ~102 / ~204 locations at $49/mo | ~1,225 / ~2,450 entities at $49/yr, or ~201 / ~402 firms at $299/yr |
| **Realistic time to $5k MRR (judgment)** | 18–24 months (two Apr 15 seasons); $10k needs multi-framework expansion, 30+ months | Not reachable in 24 months on Indiana alone | Not reachable; Q1 cash only |
| **Seasonality and churn** | Annual cycle (Jan–Apr 15). Prepay annually. Moderate churn, softened by year-over-year evidence history | Unknown until Indiana sets the renewal cycle. One-time registration means high churn | Extreme: Dec–Feb (and May for LLCs). Near-total churn after Mar 1 |

### Cited Findings
- **S1-01 basis.**
  - Nov 1 2025 final phase — [HLC](https://hlc.com/en/publications/nydfs-final-set-of-cybersecurity-requirements-under-amended-part-500-take-effect-november-1-2025)
  - Apr 15 entity-level filing — [Big I NY](https://www.biginy.org/?p=1982)
  - 500.19(b) employee notices and employer-change amendments — [DFS Jul 2026 PDF](https://www.dfs.ny.gov/system/files/documents/2026/07/Submitting-or-Amending-a%20Notice-of-Exemption_1.pdf)
  - Free DFS template — [DFS](https://www.dfs.ny.gov/cybersecurity/Program-Template)
  - $249 kit — [Art of Service](https://store.theartofservice.com/ny-dfs-23-nycrr-500/)
  - Drata Part 500 at about $10k+/yr — [Drata](https://drata.com/updates/drata-supports-nydfs-part-500); [Costbench](https://www.costbench.com/compare/drata-vs-vanta/)
  - MSPs with no public price — [CCSI](https://www.ccsinet.com/cybersecurity/nysdfs-cybersecurity-assessment/)
  - Enforcement — [Polsinelli](https://www.polsinelli.com/publications/new-york-department-of-financial-services-announces-a-1-9-million-settlement-with-insurance-agency-for-violations-of-new-yorks-cybersecurity-regulation); [Data Protection Report](https://www.dataprotectionreport.com/2026/08/nydfs-levies-250000-fine-on-licensee-for-inadequate-cyber-risk-assessment/)
- **E04 basis.**
  - Indiana go-live Jan 1 2027, rules unsettled — [AmSpa](https://www.americanmedspa.org/?p=21347); [MedSpaStandards](https://medspastandards.com/blog/indiana/indiana-med-spa-compliance-checklist)
  - Texas narrowed to IV therapy — [Polsinelli](https://www.polsinelli.com/publications/new-texas-iv-therapy-law)
  - Moxie bundles compliance — [Moxie](https://www.joinmoxie.com/compliance)
  - AmSpa Plus $634/yr — [AmSpa](https://www.americanmedspa.org/?p=19623)
  - Nevada registry not until Jan 1 2028 — [Nevada Medical Board](https://medboard.nv.gov/uploadedFiles/medboardnvgov/content/About/Board/2026/Agenda%20Item%204(1).pdf)
- **S2-01 basis.**
  - At least 10 free calculators or explainers (see Q2)
  - Harbor $199 per filing — [Harbor](https://www.harborcompliance.com/delaware-annual-report)
  - Indie clone, Oct 3 2026 — [founder-desk](https://github.com/captainchaitanya/founder-desk)
  - Corporate rates unchanged by HB 400 — [Delaware Inc](https://www.delawareinc.com/blog/delaware-franchise-tax-update-hb-400/)
  - LLC $400 first due Jun 1 2027 — [Withum](https://www.withum.com/resources/delaware-businesses-face-increased-annual-taxes-and-filing-costs/)

### Inferences (all judgment unless cited)

**S1-01: Build-if. This is the best of the three.**
- **Refined wedge, shippable by about Dec 1 2026:**
  1. An exemption wizard mirroring DFS's 500.19 categories and "Am I Exempt" flowchart, with the post-amendment thresholds (<20 staff and contractors, <$7.5M revenue, <$15M assets).
  2. A **pre-filled DFS Program Template**, so the pitch is "DFS's own template, done for you", plus AI-drafted policies with staff e-acknowledgment.
  3. A checklist of MFA and asset inventory items (email, AMS, carrier portals, bank, remote access), each with a screenshot or attestation upload. These are the requirements that took effect Nov 1 2025.
  4. A 20-minute training module with certificates.
  5. An **agency roster tracker for licensed employees' 500.19(b) notices**, including employer-change amendments.
  6. The two-signer Apr 15 packet, a choice between the Certification and the Acknowledgment of Noncompliance (with a remediation plan), and a receipt vault.
  - **Cut:** integrations, incident clock and vendor portal.
- **Price:** agency $490/yr (founding price $390 for the first 25); solo producer $149/yr; MSP wholesale $15/agency/mo.
- **First 30 days (Oct 10–Nov 9 2026):**
  - **Days 1–3:** landing page plus a free "What do I owe DFS by Apr 15, 2027?" wizard that captures email, and Stripe pre-orders delivered Dec 1 with a refund guarantee.
  - **Days 3–14:** build a list of about 1,000 NY independent agencies from public directories (Google Maps; agent locators such as Trusted Choice and Big I NY, whose availability is unverified). Send a 3-step plain email whose hook is "first certification covering a full year under the Nov 2025 MFA and asset-inventory rules."
  - **Days 5–15:** pitch Big I NY (the "Ask Tim" column) and PIANY on a January webinar and a member discount; ask whether CE credit is possible (unverified). Email about 20 NY MSPs that serve agencies (e.g., Kite, LISS, CCSI, M.A. Polce) with the wholesale offer.
  - **Days 15–30:** write SEO pages ("23 NYCRR 500 small agency checklist", "500.19(b) notice of exemption employee", "DFS April 15 certification agency"), post in agent communities, and run 10 discovery calls.
  - **Go/no-go on ~Nov 10:** at least 10 paid pre-orders, or one association/MSP partner. Otherwise shelve before building.
- **Revenue path:**
  - At $490/yr (about $41/mo MRR-equivalent), $5k MRR needs about 123 agencies and $10k MRR needs about 245.
  - At $59/mo list: about 85 and about 170.
  - **Season 1 (to Apr 15 2027):** 25–60 customers, about $1–2.5k MRR-equivalent, cash collected up front.
  - **$5k MRR:** around Apr 2028 (18–24 months), if renewals are ≥75% and an association or MSP channel works.
  - **$10k MRR:** needs the corpus's V2. The FTC Safeguards Rule (tax preparers, auto dealers) and NAIC model-law states reuse the same evidence engine. 30+ months.
- **Seasonality and churn:** demand is annual. Sell annual prepay only. Retention rests on the year-over-year evidence binder and the roster tracker. The biggest risk is "tick-the-box" agencies that self-certify for free with DFS's template.

**E04: Don't build now.**
- **Why:**
  1. Indiana, the only dated registration in the window, has unsettled fees, renewal and adverse-event rules, and probably only low hundreds of buyers.
  2. Texas's law is IV-only.
  3. California SB 351 is lawyers' work.
  4. Moxie bundles compliance into its platform, and AmSpa Plus ($634/yr) includes templates and a lawyer.
  5. Clinical documents raise liability, and the adverse-event log risks PHI.
- **If tested anyway (≤1 week):**
  - An Indiana "SB 282 registration-readiness checklist" at $49 one-time.
  - Plus a $29/mo license and protocol-expiry tracker.
  - Sold through 10 medical-director-as-a-service and GFE vendors (e.g., Docovia GFEase) as a white-label.
  - **Go only if:** one channel partner commits, or 20 pre-sales arrive by Nov 10.
- **Revenue path:** at $49/mo, $5k needs about 102 locations and $10k about 204. That is not reachable from Indiana alone. It would need Iowa, Arizona, Florida or Nevada laws to pass in 2027–2028, so 24+ months.
- **Seasonality and churn:** if registration is one-time, churn after Jan 2027 would be high.

**S2-01: Don't build.**
- **Why:**
  1. The pain is real, but at least 10 free calculators and explainers exist.
  2. Stripe Atlas documents the fix.
  3. Startup accountants (Kruze, Pilot, Fondo) bundle the filing, and Harbor files it for $199.
  4. An indie developer open-sourced the same comparator on Oct 3 2026.
  5. Corporate rates didn't change under HB 400, so there's no new shock. The only new hook is the LLC tax's first $400 payment on Jun 1 2027, and that is a flat fee with no calculation to fix.
- **Revenue path:** at $49/yr per entity, $5k MRR needs about 1,225 entities. At $299/yr per firm, about 201 firms. Expect a Jan–Feb 2027 one-time spike of perhaps $2–8k and near-zero MRR afterwards.
- **Use it only as a lead magnet** if the founder builds a broader entity- or license-compliance product (e.g., the corpus's J06). A 2-day free calculator in January could also feed SEO.

### Gaps
- **Untested assumptions.** All the revenue and timeline figures above are untested assumptions. No pre-sale, conversion-rate or churn data exists for any of the three.
- **S1-01 channel.** The biggest unknown is whether Big I NY or PIANY would promote a third-party tool, given that it already gives members a free checklist. The other is whether a bulk DFS licensee list can be obtained.
- **E04 rules.** The verdict should be revisited once the Indiana Medical Licensing Board publishes its registration rules (fee, renewal, adverse-event window and form) and the 2027 legislative sessions (IA, AZ, FL, NV) resolve.
