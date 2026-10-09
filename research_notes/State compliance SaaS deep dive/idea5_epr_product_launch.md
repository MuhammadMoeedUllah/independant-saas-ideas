# Idea 5: Packaging EPR fee simulator sold through converters. Product/technical feasibility and go-to-market (as of 2026-10-09)

> Method note (read first): These notes come from web-search excerpts gathered on 2026-10-09. Direct page fetches failed. The egress proxy blocked circularactionalliance.org, calrecycle.ca.gov, sustainablepackaging.org, packagingdive.com, useforesight.io and others, and the shared web-search budget ran out partway through. So the CAA fee PDFs, CalRecycle lists and trade articles were read only through search-engine excerpts and summaries, never as full documents. Numbers marked "via search excerpt" should be checked against the primary PDF before anyone builds on them. Some questions were never searched. They are listed under each Gaps section, sometimes with background from model knowledge, clearly marked UNVERIFIED.

---

## 1. Data inputs: what converters hold, in which systems, and what EPR reports need

### Takeaway
EPR reports need, for each state, the weight in pounds of every packaging component by that state's covered-material category, multiplied by the units supplied into that state. California also needs a count of plastic components. Converters hold the per-unit half of this: material structure, weight or gauge, inks and adhesives, PCR content, and dimensions. That data sits in packaging ERP/MIS systems (Kiwiplan, Radius, Label Traxx) and in spec platforms (Specright). Brands hold the other half: units sold per state, components bought from other suppliers, and producer and exemption status. A converter-side tool can therefore produce a credible fee per 1,000 units per state. It can only produce a total fee per state once the brand supplies volumes or accepts an apportionment assumption.

### Cited Findings
**What CAA / states require**
- CAA says producers report the quantities of covered materials they supply into each state program, including sales and packaging weights, the brands in the report, and any affiliated or associated producers that are also obligated. — [CAA Producer Reporting page](https://circularactionalliance.org/producer-reporting) (via search excerpt)
- CAA's portal training (Jan 2025) lists the items a submission needs: Associated Producers with Tax ID (EIN) and legal name, a written methodology for how supplied volumes were calculated, a list of brands, and supplied material weights in pounds. — [CAA 201 Producer Portal Training PDF](https://static1.squarespace.com/static/64260ed078c36925b1cf3385/t/678960407cb9213f6566aeb1/1737056320669/201_Portal+Training_PDF.pdf) (via search excerpt)
- Composite rule:
  - Components made of the same material are reported together.
  - If components are different materials and cannot be separated, the whole item goes in the category of the material that makes up the majority of the combined weight, and the full combined weight is reported.
  - Small-format rule: packaging with two or more sides of 2" or less goes in the "small format" category within the matching covered-material category.
  - In Oregon and California, producers must report both B2B and consumer packaging, including secondary, tertiary and shipping materials that appear on the material lists.
  - — [CAA Covered Materials & Producer Definitions (OR & CO), rev. June 2025](https://static1.squarespace.com/static/64260ed078c36925b1cf3385/t/683dfa7823960e3fa03725bc/1748892281594/Covered+Materials+%26+Producer+Definitions+%28OR%26CO%29+-+June+2025.pdf) and [CAA Producer Resource Center](https://circularactionalliance.org/producer-resource-center) (via search excerpt; the exact source document within CAA's materials is uncertain)
- California, Colorado and Oregon require full reporting of supply data. Minnesota, Maryland and Washington use a "simplified reporting" approach with broader material categories. — [CAA Producer Reporting page](https://circularactionalliance.org/producer-reporting) (via search excerpt)
- CAA publishes state-specific Excel workbooks, for example the "Oregon 2025 Report Preparation Workbook", that let producers simulate a portal submission. CAA also publishes a material-categories guidance document with definitions, examples and reporting tips for each category. — [CAA Producer Reporting page](https://circularactionalliance.org/producer-reporting) (via search excerpt). These are the best templates for an import schema and should be obtained directly.
- California: a producer joining the PRO had to submit 2023 supply data by covered material category, covering (a) total weight sold, distributed or imported into the state and (b) the total number of plastic components. — [California Grocers Assn, SB 54 Producer Reporting Requirements, 4 May 2026](https://www.cagrocers.com/wp-content/uploads/2026/05/SB-54-Producer-Reporting-Requirements-5.4.26.pdf)
- Oregon and Colorado Annual Supply Reports for CY2025 were due 31 May 2026. — [Holland & Knight, Apr 2026](https://www.hklaw.com/en/insights/publications/2026/04/are-you-ready-to-report-your-packaging-data-next-month)
- Colorado's 2026 dues are based on CY2024 supply data, and the CY2025 reports due 31 May 2026 set 2027 dues. One source says otherwise (that 2025 data informed 2026 rates). — [Personal Care Products Council, Colorado EPR Summary, May 2026](https://www.personalcarecouncil.org/wp-content/uploads/2026/06/Colorado-EPR-Summary_May-2026.pdf); conflict noted via [rePurpose 2026 deadlines guide](https://www.repurpose.global/blog/2026-epr-deadlines-complete-guide)

**Converter vs. brand knowledge**
- Packaging World reports that producers must report detailed portfolio data, "possibly including materials used, weights, units sold, recyclability, recycled content, and compostability profile", and that "that information often resides with converters, not brand owners." — [Packaging World, "Data, Integrated Systems Driving Change"](https://www.packworld.com/sustainable-packaging/recycling/article/22974672/data-integrated-systems-driving-change) (via search excerpt; may instead be from the sister article below)
- According to Packaging World, brand owners and retailers may need component-level data on material type, weight, color, clarity, composition, separability, format, recycled content, and whether the material is bio-based or fossil-based. These attributes affect recyclability classification, regulatory status and EPR fees. — [Packaging World](https://www.packworld.com/sustainable-packaging/recycling/article/22952828/brands-and-converters-align-on-epr-data-demands) (via search excerpt)
- Scott Byrne (VP Global Sustainability, Sonoco) said converters are taking a central role in helping brand owners gather data. Earlier reporting was about tonnages; the next questions are recycled content, the materials involved and likely end-of-life yields. He described most producers and converters as still in "the data stage." — [Packaging World, "Brands and Converters Align on EPR Data Demands"](https://www.packworld.com/sustainable-packaging/recycling/article/22952828/brands-and-converters-align-on-epr-data-demands)
- Converters are not legally "producers," but they provide the data and packaging information brands need to comply and to lower fees (from a FlexForward 2025 discussion between the FPA CEO and the CAA CEO). — [Packaging World, 7 Nov 2025, "EPR at the Intersection Between Brands and Converters"](https://www.packworld.com/flexibles/article/22954427/epr-at-the-intersection-between-brands-and-converters)
- Domino's guidance for converters: the required information includes material declarations on composition and weight, plus compliance documentation for the inks and adhesives used. Converters should make sure they can get documentation from their material and ink suppliers, and may compile it into compliance assessments for customers. — [Domino Printing, US Packaging EPR 2026 for converters](https://www.domino-printing.com/en-us/blog/dp-us-packaging-epr-2026-for-converters)
- A vendor guide says that even when converters or packaging suppliers are not the legal "producer," they must provide high-resolution material, weight and PCR data so the brand can register, report and calculate eco-modulated fees. — [Zenpack US EPR guide (2026 update)](https://www.zenpack.us/blog/us-packaging-epr-compliance-guide/) or [PlantSwitch EPR guide](https://www.plantswitch.com/blog/epr-compliance-guide-packaging-producers) (search excerpt; exact attribution between these two uncertain)
- Many states exempt purely B2B or transport packaging used inside the supply chain and not sold at retail. — vendor guide as above (Zenpack/PlantSwitch). Note the conflict: CAA says OR and CA do require B2B packaging to be reported (see above).

**Systems where converter data lives**
- **Kiwiplan** (Advantive) is a packaging ERP/MES aimed at corrugated, folding carton and specialty plants. Its reporting/analytics product is "DART". — [Advantive Kiwiplan](https://www.advantive.com/products/kiwiplan/); [Advantive blog](https://www.advantive.com/blog/how-kiwiplan-outperforms-generic-erp-systems/)
- **Radius** (ePS, formerly EFI) is a packaging/converting ERP for label, flexible packaging, converting and folding carton businesses. Modules: estimating, scheduling, inventory, tooling management, DMI, shop-floor data collection, shipment planning and BI. — [EFI/ePS Radius](https://go.efi.com/packaging-ERP-software-solution.html); [Capterra ePS Radius](https://www.capterra.com/p/220090/ePs-Radius/)
- Radius in EFI Packaging Suite 4.0 added "better recording and tracking of weights throughout" for extrusion and lamination. — [Printing News, EFI Packaging Suite 4.0](https://www.printingnews.com/software-workflow/workflow-automation/product/12234523/efi-efi-packaging-suite-40)
- **ePS has a landing page titled "Radius EPR Solutions."** The retrievable text covered only general ERP features. This signals that the ERP vendor is positioning around EPR, as a potential partner or competitor. — [ePS Radius EPR Solutions LP](https://go.epackagingsw.com/Packaging_LP_Radius_EPR_Solutions)
- **Label Traxx** (now under Amtech Software) is an ERP for label and flexible packaging converters with "500 customers and more than 10,000 users worldwide since 1993". It offers a Cloud API and a Data Warehouse for external apps and BI. — [Amtech Label Traxx ERP](https://www.amtechsoftware.com/solutions/label-traxx-erp/); [Label Traxx blog](https://blog.labeltraxx.com/label-traxx-enterprise)
- No source confirmed a native, dedicated EPR module in Kiwiplan, Radius or Label Traxx. The likely route is reports or APIs feeding an external EPR tool. — synthesis of the above sources (search excerpt)
- **Specright** is a spec-data platform. Its "EPR Report Generator" is powered by Lorax EPI under a partnership announced 3 Aug 2022. Specright claims reporting time falls "from 3 to 5 weeks per jurisdiction down to minutes" and that reports auto-refresh as specs change (vendor claims). — [Specright partners with Lorax EPI](https://www.specright.com/press-releases/specright-partners-with-lorax-epi-to-streamline-sustainability-reporting-compliance-d/); [Specright EPR page](https://www.specright.com/epr/)
- Recyda advertises automatic API integration with ERP, PLM and SAP systems for packaging data. — [rePurpose packaging compliance page / Recyda via search excerpt](https://repurpose.global/packaging-compliance) (attribution via search summary)

### Inferences
- **What the converter can reliably fill (per SKU / per component):** substrate or structure (layer-by-layer for laminates); gauge or basis weight and finished weight per unit; dimensions (drives the small-format flag); inks, coatings and adhesives; PCR % (from resin or board supplier certificates); color and clarity; whether layers can be separated; and quantities shipped to each brand. Most of this lives in ERP estimating/BOM records (Radius, Kiwiplan, Label Traxx), prepress/spec files, and supplier certificates. A CSV template matching CAA's workbook columns is the realistic MVP import. A direct ERP connector is a phase-2 item.
- **What the converter usually does not know:** units sold into each state; which SKUs ship where; other components on the pack (closures, labels, cartons from other suppliers); whether the packaging is primary, secondary or B2B for the brand; the brand's producer status, exemptions and revenue thresholds; and the producer hierarchy (brand owner vs. licensee vs. importer). The product therefore needs (a) a "per 1,000 units sold in state X" view the converter can produce alone, and (b) a brand-side input for state volumes, or a clearly labeled population-share apportionment default. That default is an assumption, and no source here confirms CAA accepts it.
- The composite rule (non-separable mixed materials go in the majority-weight category, at full weight) is the most important classification logic for flexible laminates and lined cartons. It must be implemented exactly, and separability needs to be an explicit field.
- California's per-plastic-component fee means the data model must count plastic components per unit, not just weight.
- CAA's per-state Report Preparation Workbooks are effectively the canonical schema. The MVP should mirror them so a converter's output can be handed to the brand as near-ready report input. That gives a concrete value proposition beyond simulation.

### Gaps
- The CAA workbook column layout and the full material-category list per state could not be read (CAA domain blocked). Download the OR, CO and CA workbooks plus the material-category guidance directly.
- **Not researched (search budget exhausted):** EFI/ePS Pace, Cerm, PrintVis, Amtech's corrugated ERP, and Esko WebCenter (only an Esko partners page surfaced: [Esko partners](https://www.esko.com/en/company/partners)). UNVERIFIED background from model knowledge:
  - Pace is ePS's print MIS, mainly commercial print.
  - Cerm is a Belgian label/packaging MIS.
  - PrintVis is built on Microsoft Dynamics 365 Business Central.
  - Siegwerk is an ink manufacturer, not an ERP/MIS vendor, but it could be a data source for ink compositions.
- No public data was found on what share of converters run each ERP, apart from Label Traxx's "500 customers" claim.
- Several guides mention "SKU-specific BOM preferred; average BOM or apportionment only temporarily" as a state preference. The search excerpt was not cleanly attributable to a primary source, so verify it with CAA's Reporting Policy ([CAA Reporting Policy v1, June 2025](https://static1.squarespace.com/static/64260ed078c36925b1cf3385/t/6864694fc0ba851a2cd78dd4/1751411023446/CAA+Reporting+Policy+-+Version+1+-+June+2025.pdf)).
- No source was found on converter/brand data-confidentiality norms, for example whether converters will share structures and weights with a third-party SaaS. FPA's only surfaced EPR policy document dates from 2020 ([FPA EPR Policy, CT DEEP](https://portal.ct.gov/-/media/DEEP/waste_management_and_disposal/CCSMM/EPR-Working-Group/AK-FPA-EPR-for-PPP.pdf)).

---

## 2. Fee calculation logic: public schedules, inputs, eco-modulation, calculators, change frequency

### Takeaway
CAA publishes per-state fee schedules as public PDFs in cents per pound by material category. They are public but not machine-readable: no API or CSV was found. They change every year, with new schedules around 1 October for the next program year, plus mid-year instruments such as California's July 2026 early fee. The core math is simple: Σ (component weight × category rate), then eco-modulation bonuses or maluses, reserve drawdowns, low-volume flat fees and California's plastic add-ons. The hard parts are category mapping, version control and preliminary-vs-final status. California's fees for 2027 are still preliminary and non-binding as of 9 Oct 2026.

### Cited Findings
**Oregon (CAA is the PRO)**
- The 2026 Oregon schedule is in ¢/lb. Excerpted rates:
  - Paper for general use, newsprint and magazines: 5.0
  - Corrugated: 8.0
  - Paperboard: 8.0
  - Aseptic and gable-top cartons: 17.0
  - Polycoated paperboard: 48.0
  - Glass bottles and jars: 10.0
  - Aluminum containers: 6.0
  - Steel containers: 10.0
  - — [CAA OR 2026 Fee Schedule PDF](https://circularactionalliance.org/s/OR-2026-Fee-Schedule-Public.pdf) (via search excerpt)
- Secondary sites quote 2026 Oregon plastics rates of clear PET bottles 25¢/lb, HDPE #2 bottles 9¢/lb, flexible film 43¢/lb and EPS containers 138¢/lb. These were not confirmed against the CAA PDF. Other aggregators list OR PET/HDPE at $0.03–0.08/lb, which conflicts with the CAA figures. — [EPR Fee Check comparison](https://eprfeecheck.com/blog/epr-fee-rates-by-state); [EPR Atlas fees by state](https://epratlas.com/epr-fees-by-state/) (aggregators; treat as unreliable)
- Oregon's schedule has roughly 60 material categories (per a search summary; not verified against the PDF). — [EPR Atlas Oregon](https://epratlas.com/oregon/)
- **The 2027 Oregon schedule was published 1 October 2026** (file "OR-2027FeeSchedule_100126.pdf"). Invoices: 50% in January 2027 and 50% in July 2027. CAA says 88¢ of every $1 goes to collection, processing and education/outreach (processing 40¢). Eco-modulation bonuses sit in a 1¢ "All other" bucket. — [CAA OR 2027 Fee Schedule PDF](https://circularactionalliance.org/s/OR-2027FeeSchedule_100126.pdf); [CAA OR 2027 Producer Fees page](https://circularactionalliance.org/or-2027-producer-fees); [Foresight news](https://www.useforesight.io/news/oregon-2027-packaging-epr-fee-schedule) (all via search excerpt)
- The 2027 Oregon schedule returns about $80M in program reserves and $3M in previously collected Specifically Identified Material (SIM) fees to producers through reduced rates. Each line therefore runs base rate, then adjustments, then final rate. Excerpted rows (column headers not visible; last value read as the final ¢/lb):

  | Category | Values | Final ¢/lb |
  |---|---|---|
  | Polycoated paperboard | 0.47 / −0.01 / −0.12 | 0.34 |
  | PET lids | 0.61 / 0.00 / −0.22 | 0.39 |
  | Other rigid PET | 0.62 / 0.00 / −0.14 | 0.48 |
  | Flexible HDPE/LDPE film | 0.29 / 0.00 / −0.17 | 0.12 (column reading uncertain) |

  Other examples: newspapers and some printing papers $0.01/lb, ceramics $0.83, aluminum foil and molded containers $0.11, glass bottles and jars $0.00 final. — [CAA OR 2027 Fee Schedule PDF](https://circularactionalliance.org/s/OR-2027FeeSchedule_100126.pdf) (via search excerpt; **must verify column meaning**)
- Oregon low-volume producers (≤10 metric tonnes into OR) pay graduated flat fees, starting at $700 for 1–2.5 tonnes. — search summary citing CAA OR materials ([CAA Oregon](https://circularactionalliance.org/oregon))
- Under Oregon's statute and DEQ framing:
  - Fees for materials on the Uniform Statewide Collection List (USCL) should be proportional to the PRO's costs for processing commingled recyclables (the processor commodity risk fee).
  - Fees for non-accepted materials recover the PRO's costs.
  - Average base rates for non-recyclable materials must be higher than for recyclable ones.
  - The schedule must consider a material's recycling rate relative to other covered products.
  - — [Oregon DEQ HB2065 section summary](https://www.oregon.gov/deq/recycling/Documents/recHB2065sectionSum.pdf); [ORS 459A.875](https://oregon.public.law/statutes/ors_459a.875) (via search excerpt; DEQ docs are 2022–2023 vintage)
- PRO-to-processor rates in Oregon's rules:
  - Processor commodity risk fee: $200 (2025–26), $286 (2027), $245 (2028+)
  - Contamination management fee: $341 (2025–26), $432 (2027), $418 (after 2027)
  - These are cost inputs to the PRO, presumably per ton, not producer rates. — [OAR 340-090-0640 via Justia](https://regulations.justia.com/states/oregon/chapter-340/division-90/section-340-090-0640/) (via search excerpt)
- Draft-plan era estimate: average base fee $345/ton (low scenario) to $457/ton (high scenario). — [EG Counsel on Oregon program plan](https://www.egcounsel.com/post/epr-packaging-laws-oregon-s-program-plan-provides-roadmap-for-compliance-and-producer-fees) (attribution via search summary; superseded by actual schedules)
- **Oregon LCA eco-modulation (bonuses only, no maluses this plan cycle):**
  - Bonus A: LCA disclosure for up to 10 SKUs; 10% discount on base fees for all materials in the SKU, capped at $20,000; must follow DEQ standards and be peer reviewed.
  - Bonus B: impact-reducing redesign, from program year 2027; tiered at about 2.0–2.5× Bonus A; capped at $50,000 per SKU and $500,000 per producer.
  - Bonus C: switching single-use plastic to reusable or refillable; added by a DEQ-approved amendment on 12 Sep 2025 (per one aggregator).
  - One bonus type per SKU per year.
  - — [EPR Atlas Oregon](https://epratlas.com/oregon/); [Packaging School: Unpacking Oregon's Ecomodulation Bonuses](https://packagingschool.com/lessons/unpacking-oregons-ecomodulation-bonuses); [Eunomia on Oregon LCAs](https://eunomia.eco/insights/extended-producer-responsibility-and-lcas-unpacking-the-oregon-approach/)
  - Bonus A submission timing conflicts across sources: due 15 Aug 2025 for 2026 fees, vs. 31 May annually, vs. 31 May 2026 for 2027 credits. — same sources
- **Oregon litigation:** NAW sued, and a narrow preliminary injunction was issued in Feb 2026, with a hearing set for July 2026. A later aggregator item mentions a lapsed DEQ pre-enforcement pause and a 16 Oct 2026 joint status report. Status as of 9 Oct 2026 is unclear. — [CAA Oregon page](https://circularactionalliance.org/oregon) (via search excerpt)

**Colorado (CAA is the PRO)**
- The 2026 Colorado Dues Schedule was published 13 Oct 2025, in ¢/lb. Excerpted rates:
  - Paper for general use: 6.0
  - Aseptic and gable-top cartons: 13.0
  - Glass bottles and jars: 4.0 (after a bonus from 4.2)
  - Aluminum containers: 2.0
  - Steel containers: 7.0
  - Aluminum foil and molded containers: 34.0
  - Colored EPS (#6): 172 (from 160.2 after a malus)
  - — [CAA CO 2026 Dues Schedule PDF](https://circularactionalliance.org/s/CO-2026-Dues-Schedule-Public.pdf) (via search excerpt); [Colorado PIRG summary](https://pirg.org/colorado/foundation/articles/what-is-colorados-extended-producer-responsibility-program-and-how-will-it-benefit-you/)
- Colorado eco-modulation:
  - The statute requires the plan to reward source reduction, high recycling and refill rates, reuse/refill design, high PCR use and recyclability or commodity-value innovations, and to discourage materials not on the Minimum Recyclable List (MRL) and designs that disrupt recycling.
  - CAA's proposal had 5 bonuses and 3 maluses.
  - CDPHE's draft proposed up to 10% reductions for MRL packaging with clear sorting instructions and locally sourced recycled content.
  - The first eco-mod rules were adopted 18 Nov 2025. CDPHE approved two mass-balance methods for PCR attribution (rolling average; proportional credit), and a third is under evaluation.
  - CDPHE required an eco-mod dispute-resolution process. Bill SB26-192, on eco-mod appeals, has unconfirmed status.
  - — [PCPC Colorado EPR Summary May 2026](https://www.personalcarecouncil.org/wp-content/uploads/2026/06/Colorado-EPR-Summary_May-2026.pdf); [Packaging School: Colorado ecomodulation](https://packagingschool.com/lessons/exploring-colorados-proposed-ecomodulation-bonuses); [H2 Compliance](https://h2compliance.com/eco-modulation-in-colorado/); [Certivo](https://www.certivo.com/blog-details/colorado-packaging-epr-producer-fees-are-live-in-2026)
- CDPHE approved the plan on 9 or 10 Dec 2025 (sources differ). Dues are paid in two installments (January and July). Penalty figures conflict ($5,000 on day 1 then $1,500/day, vs. "up to $25,000/day"). — [PCPC summary](https://www.personalcarecouncil.org/wp-content/uploads/2026/06/Colorado-EPR-Summary_May-2026.pdf); [CDPHE program page](https://cdphe.colorado.gov/hm/epr-program)
- Colorado's small-producer exemption threshold appears as "<1 ton OR <$5,632,843 global revenue (1 Jul 2025 figure, CPI-adjusted each 1 Jul)" in one table and as "<$5.5M" in another. — [EPR Fee Check](https://eprfeecheck.com/blog/epr-fee-rates-by-state); [EPR Atlas Colorado](https://epratlas.com/colorado/) (aggregators)

**California (SB 54; CAA is the PRO)**
- CalRecycle withdrew its proposed SB 54 regulations on 9 Jan 2026, reissued them (15-day comment period ended 13 Feb 2026), and the final regulations were approved and effective on 1 May 2026. Producers had about 30 days (to roughly 1 Jun 2026) to register, join the PRO or seek independent compliance. — [Resource Recycling, 12 Jan 2026](https://resource-recycling.com/recycling/2026/01/12/calrecycle-withdraws-proposed-regs-for-sb-54/); [Resource Recycling, 2 May 2026](https://resource-recycling.com/plastics/2026/05/02/calrecycle-approves-sb-54-regulations/); [Holland & Knight, May 2026](https://www.hklaw.com/en/insights/publications/2026/05/californias-final-epr-regulations-now-in-effect)
- CAA program plan timeline:
  - Revised plan posted June 2026 ([CAA CA Program Plan REVISED 2026-06-18](https://circularactionalliance.org/s/CAA_California_Program_Plan_REVISED_20260618_ADA.pdf))
  - Advisory Board review 14 Aug 2026
  - **Final draft to CalRecycle 13 Oct 2026**
  - CalRecycle approval and program start on or before 1 Jan 2027
  - First Plastic Pollution Mitigation Fund (PPMF) remittance 1 Mar 2027
  - First administrative fees to CalRecycle 1 Jul 2027
  - — [CAA California page](https://circularactionalliance.org/california); [EPR Group Consulting, June 2026](https://www.eprgroupconsulting.com/post/caa-s-california-program-plan-and-sb-54-implementation-update-june-2026); [DLA Piper, June 2026](https://www.dlapiper.com/en-us/insights/publications/2026/06/californias-epr-program-plan)
- **California 2026 Early Fee Schedule** (published 20 Jul 2026) sets six flat rates in ¢/lb: glass and ceramics 0.3, metal 0.8, paper/fiber 0.4, plastic rigid 1.3, plastic flexible 2.5. The sixth category was not visible in the excerpt. — [EPR Atlas update, 3 Aug 2026](https://epratlas.com/updates/2026-08-03-caa-publishes-california-s-2026-early-fee-schedule-six/)
- CAA's "Illustrative Fees" (May 2026) include a reuse/refill add-on of 4¢/lb (low scenario) or 10¢/lb (high scenario) on plastic. — [CAA California Illustrative Fees, 1 May 2026](https://static1.squarespace.com/static/64260ed078c36925b1cf3385/t/69f519e5cb74e00622fe25f5/1777670630296/California+Illustrative+Fees+20260501.pdf); [Adept Packaging on reading them](https://adeptpackaging.com/blog/california-sb-54-illustrative-fees-are-out-how-to-read-them/); [EPR Group Consulting](https://www.eprgroupconsulting.com/post/caa-publishes-ilustrative-fees-for-california-s-epr-program)
- **California preliminary 2027 schedule (1 Oct 2026):** a base fee per covered material category, plus on plastic components 3¢/lb for reuse investment, 26¢/lb for the PPMF and 0.1¢ per plastic component. Non-binding until CalRecycle approves the plan. — [CAA CA 2027 Producer Fees page](https://circularactionalliance.org/ca-2027-producer-fees) as summarized by [EPR Atlas California](https://epratlas.com/california/) / [EPR Fee Check California](https://eprfeecheck.com/states/california) (third-party tracker; verify)
- SB 54 requires the PRO to pay a $500M per year environmental mitigation surcharge into the PPMF starting in calendar year 2027. — [UCLA Luskin SB 54 FAQ](https://innovation.luskin.ucla.edu/understanding-senate-bill-54-in-california-what-do-we-know-about-the-plastic-pollution-prevention-and-packaging-producer-responsibility-act/) (via search excerpt)
- Sources conflict on whether California fees could be invoiced as early as fall 2026 or only from 2027. — [Waste Dive](https://www.wastedive.com/news/california-sb54-program-plan-timeline-circular-action-alliance/810500/); [Packaging Dive](https://www.packagingdive.com/news/california-sb54-preparation-progresses-circular-action-alliance/815398/) (via search summary)
- On 22 Jun 2026, 17 states led by Nebraska, together with NAW, sued CalRecycle and CAA, arguing SB 54 is unconstitutional. — third-party tracker summary (not verified with a primary docket)

**Other states / landscape**
- Seven states have packaging EPR laws: CA, CO, ME, MD, MN, OR, WA. Status by state:
  - Maine: stewardship-organization selection stage as of June 2026; one source says first fees in September 2026.
  - Minnesota: full implementation 2029–2032.
  - Maryland: registration opened 31 Mar 2026; plans due 1 Jul 2028.
  - Washington: designated CAA as PRO in March 2026; full program around 2030.
  - New bills introduced in 2026 in NH and WI; pending in MA, NJ, NY, RI and VA. No 2026 enactment confirmed.
  - — [Holland & Knight, Jan 2026](https://www.hklaw.com/en/insights/publications/2026/01/the-latest-pandoras-box-what-you-need-to-know-now-about-state-epr-laws); [Mayer Brown, Feb 2026](https://www.mayerbrown.com/en/insights/publications/2026/02/epr-packaging-laws-moving-from-concept-to-compliance); [O'Melveny 2026 update](https://www.omm.com/insights/alerts-publications/2026-plastics-epr-packaging-rules-update-what-sb-54-sb-343-state-reporting-deadlines-prc-laws-the-eu-ppwr-mean-for-producers-retailers/); [SPC Policy Roundup, May 2026](https://sustainablepackaging.org/2026/05/21/packaging-policy-news/) (dates differ slightly across sources)

**Public calculators (none official from CAA found)**
- **EPR Atlas Per-Unit Calculator** (free): per-unit fee = Σ (component weight × material rate) × eco-modulation multiplier. It covers 7 states, supports side-by-side redesign modeling, prices every component as covered and does not model exemptions. — [EPR Atlas unit calculator](https://epratlas.com/unit-calculator/)
- Other free estimators:
  - [rePurpose 2026 EPR fee calculator](https://www.repurpose.global/blog/how-to-estimate-your-2026-epr-fees-introducing-repurposes-new-epr-fee-calculator)
  - [EPR Fee Check](https://eprfeecheck.com/): a portfolio tonnage-by-material estimator with a second scenario for material shifts
  - [eprfeecalculator.com](https://eprfeecalculator.com/): UK plus CA, ME, OR, CO
  - [LAPPA EPR Fee Calculator](https://lappa.org/epr-fee-calculator/)
  - [PPWR Atlas EU fee tables](https://ppwratlas.com/fee-calculator/)
- Supplier-run calculators:
  - Paper Tube Co. offers a free calculator comparing current packaging to paper-tube alternatives, and cites multilayer flexibles at $0.74–1.02/lb vs. paper tubes at $0.08/lb (vendor claim). — [Paper Tube Co. fee calculation](https://papertube.co/blogs/down-the-tubes/epr-packaging-fees-calculation)
  - Specright offers an ROI calculator claiming a "28% average savings on annual sustainability fees" (vendor claim). — [Specright sustainable packaging](https://www.specright.com/sustainable-packaging/)
- No CAA, Oregon DEQ, AMERIPEN or SPC fee calculator surfaced in searches. CAA's official tools are the Report Preparation Workbooks and the "Illustrative Fees" document. — [CAA Producer Resource Center](https://circularactionalliance.org/producer-resource-center) (absence of evidence, not confirmed absence)

### Inferences
- **The fee engine is technically small; the rate data layer is the moat and the maintenance burden.** Each state × program year × schedule status (illustrative, preliminary, final, early fee) needs a versioned table. Each table needs:
  - Category codes
  - Base rate, adjustment columns (reserve drawdown, SIM) and final rate
  - Bonus and malus factors and eligibility rules
  - Low-volume flat-fee tiers (Oregon)
  - Exemption thresholds (Colorado's is CPI-indexed)
  - Per-component add-ons (California's 0.1¢ per plastic component; 3¢ reuse and 26¢ PPMF on plastics)
- Because there is no machine-readable feed, rates must be transcribed from PDFs every year (around 1 Oct for OR, CA and CO) and whenever CAA issues mid-year instruments. Budget about 2–4 analyst-days per state per release for transcription and QA, plus a second-person check. This is an estimate, not sourced.
- Rates moved sharply between years. Oregon polycoated paperboard went from 48¢ (2026) to about 34¢ (2027), and Oregon film appears to have fallen after reserve drawdowns. So a converter-facing "swap simulator" must always show the program year and status. Otherwise a conversation started on 2026 numbers will be wrong by 2027.
- California is the biggest fee driver but the least certain. As of 9 Oct 2026, the only firm instrument is the tiny six-rate early fee. The 2027 rates are preliminary and litigation is pending. The MVP should present California as scenario bands (illustrative low/high or preliminary), not as a point estimate.
- Free calculators (EPR Atlas, EPR Fee Check, rePurpose) already cover the "Σ weight × rate" use case for brands. Differentiation has to come from converter-side spec ingestion, laminate classification logic, a white-labeled customer report and swap comparisons tied to the converter's real product catalogue, not from the arithmetic.

### Gaps
- The full category list and final rates for OR 2026/2027 and CO 2026 could not be read. The CO 2027 dues schedule, which would be expected around October 2026, was not found in searches. Verify whether it is out.
- No evidence was found of any CAA API, CSV or JSON export of fee schedules. Ask CAA directly.
- Washington, Maryland, Minnesota and Maine fee structures: not researched in detail. Maine's stewardship organization and fee timing conflict across sources.
- Whether CAA accepts per-unit estimates multiplied by apportioned volumes as a "methodology": not confirmed.

---

## 3. Simulation: modeling material swaps credibly, recyclability lists, and liability risk

### Takeaway
A credible swap simulator has to do two things: reclassify the new structure into each state's fee category, and check each state's recyclability or acceptance determinations (Oregon USCL/PRO acceptance lists and SIMs; Colorado's Minimum Recyclable List; California's Covered Material Categories List with recyclability determinations and recycling rates). Each of these is published by a different body and updated on its own cadence. Fee outputs should be framed as indicative and versioned. Recyclability outputs carry extra legal risk because of California SB 343, which applies to products manufactured after 4 Oct 2026 but is partly enjoined. The tool should therefore never generate a "recyclable" claim.

### Cited Findings
- **Oregon lists:** the EQC defines two material-acceptance lists, one that local governments must collect and one the PRO must collect (for example at depots). The USCL combines the EQC list with any additional materials in an approved producer plan. A material can be designated a Specifically Identified Material (SIM) under four statutory criteria, including whether adding it to collection would increase costs. — [Oregon DEQ RMA technical workgroup on materials lists](https://www.oregon.gov/deq/recycling/Documents/recTWGm071922.pdf); [Oregon DEQ background, Oct 2022](https://www.oregon.gov/deq/recycling/Documents/orsacm3Background.pdf); [ORS 459A.887](https://oregon.public.law/statutes/ors_459a.887) (older documents; via search excerpt)
- **California CMC List:** on 31 Dec 2025, CalRecycle published an updated Covered Material Categories List. It included updated recyclability and compostability determinations for each covered material category and the first recycling-rate determination for each category. Updates are required at least annually. CalRecycle says these determinations are "for purposes of SB 54 only" and not for determining liability under other laws. — [CalRecycle SB 54 program page](https://calrecycle.ca.gov/packaging/packaging-epr/); [CalRecycle CMC List](https://calrecycle.ca.gov/packaging/packaging-epr/cmclist) (via search excerpt). A UCLA guide references a "January 2026" CMC list posting. — [UCLA Luskin SB 54 FAQ](https://innovation.luskin.ucla.edu/understanding-senate-bill-54-in-california-what-do-we-know-about-the-plastic-pollution-prevention-and-packaging-producer-responsibility-act/)
- **SB 343 (truth in recyclability labeling):**
  - Restrictions apply to products and packaging *manufactured* after 4 Oct 2026 (18 months after the Final Findings Report).
  - A federal court issued a preliminary injunction on 14 Jul 2026 in *California League of Food Producers v. Bonta* (No. 3:26-cv-01675, S.D. Cal.). CalRecycle says it blocks enforcement of SB 343; how far it reaches is described differently across sources.
  - CalRecycle updated Table 2 of the Final Findings Report on 24 Jun 2026. A full report update is expected in 2027 and every 5 years after.
  - A workshop on 29 Sep 2026 scoped a new MRF-based characterization study.
  - Criteria cited by guides: collected by curbside programs covering at least 60% of the California population and sorted by facilities serving at least 60% of those programs.
  - — [CalRecycle SB 343 page](https://calrecycle.ca.gov/wcs/recyclinglabels/); [Waste Dive, Oct 2026](https://www.wastedive.com/news/navigating-california-truth-in-labeling-sb-343/832396/); [Nixon Peabody, 6 Apr 2026](https://www.nixonpeabody.com/insights/alerts/2026/04/06/californias-sb-343-restricts-common-recyclability-claims-on-products-and-packaging); [Procopio, "Mislabel It, Pay for It"](https://www.procopio.com/resource/mislabel-it-pay-for-it)
- **Colorado:** eco-modulation maluses target materials not on the Minimum Recyclable List and designs that disrupt recycling. Draft bonuses reward MRL packaging with clear sorting instructions and locally sourced PCR. — [PCPC Colorado summary](https://www.personalcarecouncil.org/wp-content/uploads/2026/06/Colorado-EPR-Summary_May-2026.pdf); [Packaging School](https://packagingschool.com/lessons/exploring-colorados-proposed-ecomodulation-bonuses)
- Oregon and Colorado both use eco-modulation, but with different rate structures, units and bonus/malus criteria. A format that earns a reduction in one state won't automatically qualify in the other. — [Packfora, eco-modulation explained](https://packfora.com/blog/epr-packaging-fees-eco-modulation-explained) (via search summary)
- More than a 20-fold gap separates the cheapest and most expensive categories. Oregon 2025 base rates were about $0.06/lb for paper, $0.24/lb for rigid plastic and $0.34/lb for flexible plastic. — [Paper Tube Co.](https://papertube.co/blogs/down-the-tubes/epr-packaging-fees-calculation) / [EPR Fee Check](https://eprfeecheck.com/blog/epr-fee-rates-by-state) (via search summary; vendor/aggregator)
- Flexible-specific technical risk: multilayer structures may need advanced recycling to separate, and even mono-material films are hard to collect and sort. Film suppliers, converters and resin producers may influence brands' recyclability outcomes more than suppliers of other materials. — [Packaging World, 7 Nov 2025](https://www.packworld.com/flexibles/article/22954427/epr-at-the-intersection-between-brands-and-converters)
- Ink and material choices can downgrade otherwise recyclable packaging and raise fees. — [Domino article republished in trade press, Sep 2026](https://spnews.com/packaging-supplier-to-strategic-brand/); [Ink World](https://www.inkworldmagazine.com/exclusives/packaging-epr-from-packaging-supplier-to-strategic-brand-partner/)
- APR has launched a tool for "full packaging recyclability assessment", which is a potential reference or integration point for design-for-recycling checks. — [APR announcement](https://plasticsrecycling.org/resources/apr-unveils-new-tool-for-full-packaging-recyclability-assessment/) (title only; details not retrieved)
- Recyda positions itself as a packaging-design specialist (recyclability assessment, EPR fee calculation, PPWR readiness; 20+ countries). Lorax "is a reporting and data engine, not a design-for-recycling scorer." — [Repax, Recyda alternatives](https://www.repax.io/blog/recyda-alternatives); [Repax, Lorax alternatives](https://www.repax.io/blog/lorax-epi-alternatives) (competitor-authored; bias)
- Calculator-design guidance from search synthesis:
  - Results should be labeled indicative.
  - Actual invoices depend on exact material classification, eco-modulation profile and state rule interpretation.
  - Each state needs one documented rate source with date and status.
  - The exemption check should be a separate step.
  - A supplier-run tool should disclose that it is a sales aid.
  - — [EPR Atlas unit calculator](https://epratlas.com/unit-calculator/); [EPR Fee Check](https://eprfeecheck.com/) (via search summary)
- Regulators can audit producer data submissions and require documentary support. — [Adams and Reese, US Packaging EPR guide](https://www.adamsandreese.com/insights/us-packaging-epr-what-producers-need-to-know-now) (via search summary)
- Colorado has a formal eco-modulation dispute-resolution path, which shows that factor assignments can be contested. — [PCPC Colorado summary](https://www.personalcarecouncil.org/wp-content/uploads/2026/06/Colorado-EPR-Summary_May-2026.pdf)

### Inferences
- **Swap-simulator logic (MVP):**
  1. Take the baseline structure and components.
  2. Take a candidate structure from the converter's catalogue, for example a PET/PE laminate vs. mono-PE vs. paper-based.
  3. Reclassify each component into each state's category, applying the composite and small-format rules.
  4. Compute weight delta × rate delta and the change in plastic component count (California).
  5. Flag list status per state: OR USCL/PRO list/SIM, CO MRL, CA CMC recyclable yes/no and recycling rate.
  6. Show eco-mod eligibility as "potential bonus" without netting it in by default.
  7. Show fee ranges for California.
- Keep "recyclability status" informational and sourced (for example "CalRecycle CMC list dated 31-Dec-2025 shows category X as not recyclable"), and never output a consumer-facing claim. SB 343, the FTC Green Guides and the state list rules put claim liability on the brand, and a converter's tool generating claims creates exposure.
- **Liability mitigation:**
  - A version stamp on every number (rate table, program year, preliminary or final status).
  - "Estimate, not an invoice" disclaimers in the white-label report.
  - Terms that make the brand responsible for its CAA submission.
  - An audit trail of assumptions (weights, PCR certificates, volume apportionment).
  - E&O insurance.
  - These are unsourced recommendations. No case of a fee-estimate vendor being sued was found.
- Oregon's LCA bonuses (up to $20k/SKU, Bonus B up to $50k/SKU) suggest an upsell: flag SKUs where an LCA or redesign could earn a bonus. The tool should not perform the LCA, since peer review is required.

### Gaps
- Oregon's current USCL contents, the PRO acceptance list and the current SIM list were not retrieved (DEQ pages not fetched).
- Colorado's MRL contents and final eco-mod factor table: not found.
- California's 2032 targets (100% recyclable or compostable; 65% plastic recycling rate; 25% plastic source reduction). Only the 25% source-reduction figure surfaced in this search set ([Domino/SPNews](https://spnews.com/packaging-supplier-to-strategic-brand/)). The other two are UNVERIFIED (model knowledge) and should be checked against PRC 42050–42057.
- How2Recycle's role, and whether its assessments can be licensed or integrated: not researched.
- No precedent was found for liability claims against EPR estimate tools.

---

## 4. Build effort: MVP components and comparable tools

### Takeaway
Two layers make up a converter-channel MVP. One is a thin calculation core: per-state versioned rate tables, a classification ruleset, and per-unit and per-scenario math. The other, where most of the work goes, is data plumbing: a CSV/workbook importer modeled on CAA's templates, a material-taxonomy mapper for laminates and coatings, an optional ERP connector (Label Traxx API, Radius/Kiwiplan reports), and a white-labeled PDF/HTML customer report. The comparable tools range from free single-page calculators (EPR Atlas, EPR Fee Check) to enterprise platforms (Lorax EPI, Specright+Lorax, Recyda). None is specifically a converter-channel, white-label product. That niche looks open, though the ePS "Radius EPR Solutions" page suggests ERP vendors are circling.

### Cited Findings
- **Lorax EPI:**
  - Covers more than 200 schemes worldwide (packaging, WEEE, batteries, textiles).
  - Fee modeling is delivered as an Excel model with a tab per jurisdiction, plus a consultant session.
  - Pricing is sales-led with no public price (as of July 2026).
  - "ENVI Lite" is updated monthly with unlimited internal users on one annual license.
  - Described as a reporting engine, not a design scorer.
  - — [Repax: best EPR software 2026](https://www.repax.io/blog/best-epr-software); [Repax: Lorax EPI alternatives](https://www.repax.io/blog/lorax-epi-alternatives); [Repax: Lorax EPI vs Assent](https://www.repax.io/blog/lorax-epi-vs-assent-epr-reporting-chain) (competitor-authored)
- **Specright + Lorax:** Specright centralizes spec data, while Lorax calculates fees by local legislation and region-specific categories and generates reports. A PPWR connector pushes spec data to Lorax. Pricing is modular and quote-only. — [Specright partnership PR](https://www.specright.com/press-releases/specright-partners-with-lorax-epi-to-streamline-sustainability-reporting-compliance-d/); [Specright PPWR](https://www.specright.com/ppwr/); [Specright EPR](https://www.specright.com/epr/)
- **Recyda:** packaging-focused (recyclability, EPR fees, PPWR), 20+ countries, demo-only, with API integration to ERP, PLM and SAP. — [Repax: Recyda alternatives](https://www.repax.io/blog/recyda-alternatives); [rePurpose compliance page](https://repurpose.global/packaging-compliance) (via search summary)
- **Packgine:** "calculates current and projected EPR fees for every SKU in your portfolio" and markets EPR-driven redesign and conversions. — [Packgine EPR](https://packgine.ai/epr); [Packgine EPR-driven conversions](https://packgine.ai/blog/epr-driven-packaging-conversions)
- **rePurpose:** done-for-you compliance. The client provides packaging and sales data, and rePurpose handles the process, including fee forecasting. — [rePurpose packaging compliance](https://repurpose.global/packaging-compliance)
- **Self-serve, low price:** EPR Insights from about $15/month; Repax free tier at €0 with plans from €29/month. — [Repax best EPR software](https://www.repax.io/blog/best-epr-software) (competitor-authored)
- **Free calculators:** EPR Atlas per-unit BOM calculator, $0, 7 US states. — [EPR Atlas](https://epratlas.com/unit-calculator/)
- **Other multi-program compliance vendors seen in results:**
  - Certivo ("manage six programs in one system") — [Certivo](https://www.certivo.com/blog-details/us-state-packaging-epr-how-to-manage-six-programs-in-one-system)
  - FoodChain ID EPR product — [FoodChain ID](https://www.foodchainid.com/products/extended-producer-responsibility/)
  - Foresight — [useforesight.io](https://www.useforesight.io/news/oregon-2027-packaging-epr-fee-schedule)
  - PCX Markets EPR compliance — [PCX](https://www.pcxmarkets.com/epr-packaging-compliance)
  - For-Sure EPR software — [for-sure.net](https://for-sure.net/pages/epr-software)
- **ERP integration hooks:** Label Traxx Cloud API and Data Warehouse ([Amtech](https://www.amtechsoftware.com/solutions/label-traxx-erp/)); Kiwiplan DART reporting ([Advantive](https://www.advantive.com/products/kiwiplan/)); Radius BI and reporting ([Capterra](https://www.capterra.com/p/220090/ePs-Radius/)).
- Specright claims reporting falls "from 3 to 5 weeks per jurisdiction to minutes" with structured spec data (vendor claim). This is a useful benchmark for the manual effort a converter-supplied dataset could save the brand. — [Specright EPR](https://www.specright.com/epr/)

### Inferences
- **Proposed MVP scope** (estimates are author judgment, not sourced):
  1. **Spec import:** a CSV/XLSX template mirroring CAA workbook fields, with SKU → component → layer, weight per unit, dimensions, PCR %, color/clarity, separability, ink/adhesive notes and plastic-component count. About 2–3 weeks.
  2. **Taxonomy mapper:** a rules table from converter vocabulary (for example "48ga PET / 2mil LLDPE adhesive lam") to each state's category, with composite, small-format and B2B flags. Human review queue for ambiguous items. About 3–4 weeks, plus ongoing work.
  3. **Fee engine:** versioned rate tables for OR, CO and CA (early, illustrative, preliminary), low-volume tiers, CA plastic add-ons and eco-mod flags. About 2 weeks for code; rate entry and QA are recurring.
  4. **Scenario simulator:** side-by-side baseline vs. alternative structures per state, per 1,000 units, and at brand-entered or apportioned volumes. About 2 weeks.
  5. **White-label report:** converter logo, brand-customer view, PDF export, assumptions and version stamp. About 2 weeks.
  6. **Multi-tenant auth:** converter as tenant, brand customers as guests. About 1–2 weeks.
  - Total: roughly 3–4 months for 1–2 engineers plus a part-time EPR analyst.
- A phase-2 ERP connector (Label Traxx API first, because it is documented and label/flex-focused) would add 4–8 weeks per system and requires vendor partnership.
- The bigger risk is not build time but category-mapping accuracy for laminates, coated board and labels, and keeping pace with annual rate changes in three or more states.
- Competitive positioning: Specright+Lorax target brands' spec teams (enterprise, quote-based). Free calculators target brands' self-serve research. A converter-paid, white-labeled tool that turns the converter's own spec library into per-customer fee and swap reports is a distinct wedge. ERP vendors (ePS Radius) are the most likely fast followers or acquirers.

### Gaps
- No public data was found on how long comparable tools took to build, team sizes, or funding.
- No direct verification of Lorax, Specright or Recyda pricing. All are quote-only, and the Repax descriptions are competitor-authored.
- Whether ePS "Radius EPR Solutions" is a real module, a partner integration or marketing only: unresolved.

---

## 5. Go-to-market via converters: industry structure, associations and events, converter EPR services, partnership and pricing models, distributors and PROs

### Takeaway
US flexible packaging alone is about a $42.6B (2024) industry with roughly 600 converters. It is concentrated at the top (top 25 hold about 54% of revenue), which leaves a long tail of several hundred mid-size converters as the natural first customers. The trade press shows converters are being pushed into an "EPR data partner" role through 2025–2026: Sonoco, FPA/CAA at FlexForward, Domino's converter guidance, and Global Pouch Forum 2026. Smaller suppliers already use EPR content and calculators as sales tools (Paper Tube Co., EcoEnclose, PakFactory). Veritiv is the one distributor with documented EPR guidance services. No evidence was found of a white-label EPR tool sold through converters, which suggests the channel is unproven but also uncontested.

### Cited Findings
**Industry structure**
- FPA's 2025 State of the Industry report:
  - US flexible packaging reached $42.6B in 2024 (+2.9% from $41.4B).
  - The value-added segment (printing, laminating, coating, extrusion, bag and pouch making) was about $34.1B.
  - Flexibles are about 20% of the US packaging market, second only to corrugated.
  - Members expected 4.8% growth in 2025, to about $44.6B.
  - — [FPA press release](https://www.flexpack.org/news/fpa-publishes-2025-state-of-the-us-flexible-packaging-industry-report); [Packaging World](https://www.packworld.com/leaders-new/materials/news/22964554/fpa-publishes-2025-state-of-the-us-flexible-packaging-industry-report)
- About 600 flexible packaging converters; the top 5 hold 36% of revenue, the top 10 45% and the top 25 54%. — [Converting Quarterly](https://convertingquarterly.com/?p=8790) (secondary to FPA)
- The flexible packaging industry supports about 398,780 FTE jobs, of which 98,000+ are direct manufacturing (John Dunham & Associates with FPA). — via search summary of FPA coverage ([Label & Narrow Web](https://www.labelandnarrowweb.com/breaking-news/fpa-announces-2025-state-of-the-us-flexible-packaging-industry-report/))
- **ProAmpac completed its acquisition of TC Transcontinental Packaging in March 2026 for about $1.51B** (25 plants; extrusion, printing, lamination, converting and recycling). — [ProAmpac press release](https://www.proampac.com/en-us/media-center/941/proampac-completes-acquisition-of-tc-transcontinental-packaging/); [Packaging Dive](https://www.packagingdive.com/news/proampac-acquires-tc-transcontinental-packaging/807249/); [TC Transcontinental IR, 8 Dec 2025](https://tctranscontinental.com/sites/default/files/00%20Investors/2025-12-08/2025_12_08_TC_Transcontinental_IR_Presentation.pdf)
- Major converted-flexibles players: ProAmpac, Amcor, Sealed Air, Sonoco, Constantia Flexibles. — [Mordor Intelligence](https://www.mordorintelligence.com/industry-reports/converted-flexible-packaging-market)
- Label Traxx alone claims about 500 converter customers, a rough proxy for the size of the US/NA label and flex converter base on one ERP. — [Amtech Label Traxx](https://www.amtechsoftware.com/solutions/label-traxx-erp/)

**Evidence of converters and suppliers moving into EPR advisory**
- Sonoco's VP of global sustainability described converters as central to helping brands gather EPR data. — [Packaging World](https://www.packworld.com/sustainable-packaging/recycling/article/22952828/brands-and-converters-align-on-epr-data-demands)
- At FlexForward 2025, the FPA CEO and the CAA CEO discussed the converter's role. — [Packaging World, 7 Nov 2025](https://www.packworld.com/flexibles/article/22954427/epr-at-the-intersection-between-brands-and-converters)
- Global Pouch Forum 2026 had a session on how converters handle state EPR mandates. — [Packaging Strategies, "Converting Trends: Flexible Packaging Readies for EPR", July 2026](https://www.packagingstrategies.com/articles/106475-converting-trends-flexible-packaging-readies-for-epr)
- Domino (a coding and digital printing equipment supplier) published "Packaging EPR: From Packaging Supplier to Strategic Brand Partner" (Sep 2026, syndicated widely). It argues converters can add value by working with brands, designers and material suppliers on recyclability. — [SPNews](https://spnews.com/packaging-supplier-to-strategic-brand/); [WhatTheyThink](https://whattheythink.com/news/131980-packaging-epr-packaging-supplier-strategic-brand-partner/); [Paper Asia, 21 Sep 2026](https://www.paperasia.com.my/2026/09/21/packaging-epr-from-packaging-supplier-to-strategic-brand-partner/)
- Trade framing: providing detailed packaging specifications "isn't an optional value-add, it's an essential service," and standardized-format data spares brands duplicate work across jurisdictions. — [Packaging Strategies, July 2026](https://www.packagingstrategies.com/articles/106475-converting-trends-flexible-packaging-readies-for-epr) / related Packaging World coverage (via search summary)
- Organized packaging data makes suppliers "more attractive" to environmentally conscious customers. — [Strategic Packaging Partners](https://strategicpackagingpartners.com/how-smart-companies-are-using-packaging-data-to-reduce-epr-costs/)
- Avery Dennison (a label materials supplier) has published "EPR Fees: What converters need to know and how to prepare," which is EU-focused. — [Avery Dennison](https://label.averydennison.com/eu/en/home/news-and-insights/EPR-Fees-What-converters-need-to-know-and-how-to-prepare.html)
- Suppliers using EPR as sales content or tools:
  - Paper Tube Co.: a free EPR fee calculator vs. paper tubes ([link](https://papertube.co/blogs/down-the-tubes/epr-packaging-fees-calculation))
  - EcoEnclose: an EPR FAQ ([link](https://www.ecoenclose.com/blog/epr-faq))
  - PakFactory: a US/Canada EPR guide ([link](https://pakfactory.com/blog/epr-for-packaging))
  - GV Printing: a state guide ([link](https://www.gv-printing.com/us-packaging-epr-laws-by-state/))
  - Zenpack ([link](https://www.zenpack.us/blog/us-packaging-epr-compliance-guide/))
  - Berlin Packaging: SB 343 insights ([link](https://www.berlinpackaging.com/insights/sustainability/california-regulation-to-restrict-recyclability-claims-on-packaging))
  - Atlantic Packaging: an EPR deep dive ([link](https://www.atlanticpkg.com/deep-dive-extended-producer-responsibility-epr-for-packaging-explained/))
  - KM Packaging ([link](https://www.kmpackaging.com/knowledge/library/epr-around-the-world))
  - AJ Adhesives ([link](https://www.ajadhesives.com/packaging-epr-laws-2026/))
- Searches found **no** EPR data services or tools specific to Amcor, ProAmpac, Sonoco or TC Transcontinental. Those searches returned only corporate news (absence of evidence).

**Distributors and PROs**
- Veritiv advertises a Sustainable Design Lab offering packaging design, LCAs and "EPR guidance", plus an "EPR & Regulations" page. — [Veritiv home](https://www.veritiv.com/home)
- Veritiv sold its rigid containers business to TricorBraun (closed early 2025) and its Canadian business to Imperial Dade (May 2022). No EPR service was found for TricorBraun or Imperial Dade. — [Veritiv IR](https://ir.veritiv.com/newsroom/Press-Release-Details/2025/Veritiv-Closes-the-Sale-of-its-Rigid-Containers-Business-to-TricorBraun/default.aspx); [PR Newswire](https://www.prnewswire.com/news-releases/veritiv-closes-sale-of-canadian-operations-to-imperial-dade-301537582.html)
- CAA is the PRO in OR, CO and CA, and was designated in WA in March 2026. It publishes workbooks, illustrative fees and webinars, but no producer-facing estimator was found. — [CAA Producer Resource Center](https://circularactionalliance.org/producer-resource-center); [CAA California Program Update webinar, 19 Feb 2026](https://static1.squarespace.com/static/64260ed078c36925b1cf3385/t/69a9efe13916851c3f44ef67/1772744673430/CAA+California+Program+Update+Webinar+-+Feb.+19+2026.pdf)

**Pricing benchmarks and value framing**
- Enterprise tools (Specright, Lorax, Recyda) are quote-only. Self-serve tools run from €0 to €29/month (Repax) and about $15/month (EPR Insights). — [Repax](https://www.repax.io/blog/best-epr-software); [Specright](https://www.specright.com/sustainable-packaging/)
- One guide suggests brands budget 0.5–1% of annual sales for PRO fees, equal to a 20–40% increase in packaging spend. Oregon averages are cited at about $0.076–0.77/lb. — search summary of supplier blogs ([EcoEnclose EPR FAQ](https://www.ecoenclose.com/blog/epr-faq) / [Paper Tube Co.](https://papertube.co/blogs/down-the-tubes/epr-packaging-compliance-checklist-what-your-business-needs-to-do-right-now)); exact attribution uncertain; vendor-sourced

### Inferences
- **Beachhead:** mid-size flexible packaging and label converters, roughly the long tail outside the top 25 of the ~600 flexibles converters, plus label shops on Label Traxx or Radius. Their customers are mid-market CPG brands that lack Specright or Lorax. Fees per pound are highest for flexibles and multilayer structures, so the swap story (laminate to mono-PE or paper) is most compelling there. That cuts both ways: converters selling non-recyclable laminates may resist a tool that shows their product in a poor light. Pitch it as "retain the account by offering the redesign before the competitor does."
- The top 25 (Amcor, ProAmpac+TCP, Sealed Air, Sonoco, Constantia and others) will likely build in-house or use Specright/Lorax. Treat them as later enterprise deals or data partners, not the beachhead.
- **Partnership models to test** (no public benchmarks found):
  - (a) Converter pays a platform fee tiered by number of brand customers or SKUs, white-labeled.
  - (b) Per-brand-customer seat, so the converter can pass through or bundle the cost.
  - (c) Revenue share on brand-side upgrades, for example when a brand graduates to full reporting.
  - (d) An OEM/embedded deal with an ERP vendor (ePS Radius, Amtech Label Traxx, Advantive Kiwiplan) to reach their installed bases. Label Traxx's ~500 customers is a concrete channel size.
- **Distributors:** Veritiv's existing "EPR guidance" offering makes it the most plausible distributor partner or competitor. Distributors' customers are many smaller brands, which could make a self-serve variant viable there.
- **Timing hooks:**
  - Oregon and California 2027 rates published 1 Oct 2026, Colorado presumably similar.
  - California plan approval around 1 Jan 2027.
  - OR and CO invoices in Jan and Jul 2027.
  - Next supply reports due around 31 May 2027.
  - These dates create natural Q4 2026 to Q2 2027 selling moments for converter-to-brand conversations.

### Gaps (search budget exhausted before these were researched)
- **Counts of folding carton converters (PPC), label converters (TLMI), and corrugated plants and independents (AICC/FBA):** not researched. UNVERIFIED model knowledge:
  - AICC represents several hundred independent corrugated and packaging companies.
  - The Paperboard Packaging Council represents folding carton converters.
  - TLMI is the North American label association.
  - PRINTING United Alliance covers printers broadly.
  - Verify all counts.
- **Event dates for 2026–27** (PACK EXPO International, Labelexpo Americas, PRINTING United Expo, FPA Annual Meeting/FlexForward, AICC meetings, SPC Engage/Impact, Global Pouch Forum): not verified. Only FlexForward 2025 and Global Pouch Forum 2026 are evidenced above.
- **Amcor–Berry merger and Smurfit Westrock:** UNVERIFIED model knowledge says the Amcor–Berry all-stock merger closed around 30 Apr 2025, and Smurfit Kappa–WestRock combined as Smurfit Westrock in July 2024. Verify. No converter EPR offerings were found for Graphic Packaging, Smurfit Westrock or Huhtamaki (not searched).
- No pricing benchmarks were found for white-label or OEM packaging software deals or rev-share norms.
- No direct evidence of any converter paying for an EPR tool for its customers. This is the core channel hypothesis and needs customer discovery.

---

## 6. Expansion paths: Canada, EU PPWR, UK pEPR fee engines

### Takeaway
International expansion is technically the same pattern (versioned rate tables, category mapping, eco-modulation), but these markets are already served by Lorax EPI (200+ schemes), Recyda (20+ countries), Repax (EU/UK) and free EU/UK fee tables. Treat international as follow-on modules for converters whose brand customers sell cross-border, not as a primary wedge. The EU PPWR started applying on 12 Aug 2026, which raises demand for recyclability-grade data that the same spec ingestion pipeline can serve.

### Cited Findings
- The EU Packaging and Packaging Waste Regulation entered into force on 11 Feb 2025 and applies from 12 Aug 2026. — [EUROPEN EPR page](https://www.europen-packaging.eu/policy-area/extended-producer-responsibility/) (via search summary; exact source among results uncertain)
- Existing multi-jurisdiction tools:
  - Lorax EPI: 200+ schemes
  - Recyda: 20+ countries, PPWR readiness
  - Specright: PPWR connector via Lorax
  - Repax: EU/UK tools from €0 to €29/month
  - Remedy EPR: UK comparison of six platforms
  - PPWR Atlas: EU fee tables by country
  - eprfeecalculator.com: UK plus US states
  - — [Repax best EPR software for EU](https://www.repax.io/blog/best-epr-software-for-eu-compliance); [Repax best UK packaging EPR software](https://www.repax.io/blog/best-uk-packaging-epr-software); [Remedy EPR UK comparison](https://www.remedy-epr.com/blog-best-epr-software); [Specright PPWR](https://www.specright.com/ppwr/); [PPWR Atlas](https://ppwratlas.com/fee-calculator/); [eprfeecalculator.com](https://eprfeecalculator.com/); [Coolset PPWR tools](https://www.coolset.com/academy/best-6-ppwr-compliance-tools-for-importers-and-distributors-2026)
- EU fee calculators often exclude registration fees, membership fees, minimum contributions and administrative charges, and point users to official national platforms. — [PPWR Atlas / similar](https://ppwratlas.com/fee-calculator/) (via search summary)
- Canada: a supplier guide covers "EPR for Packaging in Canada & the U.S." (2026), but its content was not retrieved. — [PakFactory](https://pakfactory.com/blog/epr-for-packaging)

### Inferences
- **Sequencing:** first deepen US coverage (OR, CO and CA now; WA, MD, ME and MN as their schedules arrive in 2026–2030). Then Canada, because North American converters such as ProAmpac+TCP have cross-border customers and Canadian provincial programs have published per-material fee schedules. Then the UK, then the EU, where incumbents are strongest.
- PPWR recyclability grading and the UK's recyclability-based modulation both reward the same component-level data the US MVP collects (layers, inks, adhesives, separability). That makes the spec-ingestion layer the reusable asset, with each fee engine as a plug-in.

### Gaps (not researched; search budget exhausted)
- **Canada:** UNVERIFIED model knowledge:
  - Ontario moved to full producer responsibility for Blue Box by 1 Jan 2026, with Circular Materials as the main PRO.
  - BC (Recycle BC) and Quebec (Éco Entreprises Québec, with eco-modulation) publish annual per-material fee schedules.
  - Verify current schedules and eco-modulation.
- **UK pEPR:** UNVERIFIED model knowledge:
  - First pEPR invoices for base fees came in 2025–26.
  - Modulated fees using the Recyclability Assessment Methodology (red/amber/green) are slated to begin with the 2026–27 assessment year.
  - Verify exact dates and the published PackUK fee tables.
- **EU PPWR:** recyclability performance grades and the timing of modulated fees under PPWR were not researched. National EPR fee schedules (France CITEO, Germany LUCID/dual systems, etc.) were not reviewed.
