# Screen group 1: horizontal SMB tools (A01–A06, B01–B07, L01–L06) re-scored for a solo developer

*Method note: corpus-only screen, no web search (quota reserved). Corpus root: `/tmp/claude-0/-home-user-independant-saas-ideas/092925a7-1f05-56f0-9077-35fc33825fa0/scratchpad/corpus/SaaS-Opportunity-Research/`. Every link like `ideas/A03-….md` is relative to that root. The URL after "citing" is the source the idea file itself gives. The corpus was written Sep 24–25 2026 and today is Oct 10 2026. Scores, kill-flag calls, wedges and competitor names that the corpus does not mention are my judgment, and they are labeled that way in the Inferences sections. Rubric: `research_notes/Solo developer SaaS opportunity shortlist/_solo_dev_rubric.md` (8 criteria, 1–5 each, /40; 8 kill flags; wedge rule).*

## Key question 1: the 8 rubric scores (/40), kill flags, and the evidence for each of the 19 ideas

### Takeaway
None of the 19 horizontal tools is a clean win. Most score 23–28/40 because they are easy to sell self-serve online. Crowding by cheap indie tools (kill flag K8) or telephony (K3) caps nearly all of them. The ones that survive the kill flags are **B07 StudioDesk (28)**, **B04 FirstCall (27)**, **A06 Coursehouse (27)**, **A03 LocalLoop (24, only as a module on the B04 codebase)** and **L04 ClipSOP (28, conditional)**. B06, L05 and L06 (17 each) are clearly out. A05, B01, B02, L01, L02 and L03 each carry two or more kill flags. A01, A02, A04 and B03 have one flag but low ARPU in a crowded field, so they are better treated as components of a shortlisted product.

### Cited Findings

**Corpus-wide context**
- Corpus scores use five criteria (Pain, Price gap, Build ease, Sales speed, Market size), each 1–5, for a total out of 25. "Priority" adds 0.1 for each state that ranks the idea top-3 — [INDEX.md §intro](INDEX.md)
- The corpus's own 6-month switching-window calendar (Oct 2026–Apr 2027) lists **none** of the A, B or L ideas. Every dated trigger in it belongs to compliance or vertical ideas (J01, K02, K03, C05, S2-01 and others) — [INDEX.md §3](INDEX.md)
- The Sep 24 fact-check pass covered only the top 12 ideas. Among my 19, only A03, A06, B01, B04, B07 and L03 have a "Verification" section. A01, A02, A04, A05, B02, B03, B05, B06, L01, L02, L04, L05 and L06 were not fact-checked — [INDEX.md §8](INDEX.md); confirmed by reading each idea file.
- How many state files mention each ID (grep of `states/`): B04 50 (top-3 in 40 states), A03 35 (top-3 in 24), A04 8, B06 6, B01 5, L03 5, A01 4, B07 4, L05 4, L06 3, B05 2, L02 2, A06 1, and 0 for A02, A05, B02, B03, L01, L04 — [_states_summary.csv](_states_summary.csv), [states/](states/)
- The state law hooks that matter for this group are: Wisconsin §134.49, which makes business auto-renewals unenforceable without a signed disclosure and a 15–60-day notice; NY GOL §5-903 (verify); FL FTSA, under which automated texts need prior express written consent, at $500 per violation; OK and MD mini-TCPAs; NV SB 370 and WA MHMDA, which bring consumer-health-data consent to small businesses; and the CA home-improvement down-payment cap of $1,000 or 10% — [states/WI-wisconsin.md](states/WI-wisconsin.md), [states/NY-new-york.md](states/NY-new-york.md), [states/FL-florida.md](states/FL-florida.md), [states/NV-nevada.md](states/NV-nevada.md), [states/WA-washington.md](states/WA-washington.md), [states/CA-california.md](states/CA-california.md)
- California's AB 2863 auto-renewal amendments apply to consumer contracts only. "B2B SaaS is not covered" — [states/CA-california.md](states/CA-california.md). This undercuts the CA auto-renewal angle that B03 and B06 propose.

**A01 FormFlare (forms; corpus 19)**
- Typeform Basic is $29/mo for 100 responses, and HIPAA is available only on Enterprise. Jotform puts HIPAA on Gold ($99–129). **Tally is free with unlimited forms and submissions, Pro is $24/mo, and Fillout is "in the same price band"** — [ideas/A01](ideas/A01-forms-typeform-jotform-alternative.md), citing [Typeform](https://www.typeform.com/pricing), [Zite](https://www.zite.com/blog/jotform-pricing), [Tally](https://tally.so/pricing)
- The corpus's own honest read: "Everything Google Forms does + themes + custom domain is already sold by Tally for $0–24/mo, so it is not a moat." INDEX adds that "the free and cheap tier is crowded" and suggests bundling it as an intake layer rather than launching it alone — [ideas/A01](ideas/A01-forms-typeform-jotform-alternative.md), [INDEX.md §2](INDEX.md)
- The MVP includes form-by-text over SMS ("Twilio, 10DLC registration done for the customer") and a kiosk/offline PWA. HIPAA mode is V2 and needs BAA hosting. Phishing abuse of form builders is a named risk — [ideas/A01](ideas/A01-forms-typeform-jotform-alternative.md)
- Proposed prices: Pro $19, Health $39, Agency $49, Event Pass $15 per 30 days — [ideas/A01](ideas/A01-forms-typeform-jotform-alternative.md)
- Triggers are Jotform renewals reportedly at up to 3x (Trustpilot, Aug 31 and Sep 1 2026) and response caps. There is no dated window. NV and WA rank A01 #2 for SB 370 / MHMDA consent intake — [ideas/A01](ideas/A01-forms-typeform-jotform-alternative.md), citing [Trustpilot](https://www.trustpilot.com/review/www.jotform.com); [states/NV-nevada.md](states/NV-nevada.md), [states/WA-washington.md](states/WA-washington.md)

**A02 BookFlat (scheduling; corpus 16)**
- Calendly Standard is $10/$12 per seat, and the new Standard Plus is $18/$24 (AI tiers added Aug 19 2026). Acuity Starter ($20) is email-only, and SMS starts at $34. Setmore is free, with Pro from $5/user. Cal.com and free Google Calendar booking pages are named as the low end — [ideas/A02](ideas/A02-scheduling-acuity-calendly-alternative.md), citing [UseCarly](https://www.usecarly.com/blog/calendly-standard-plus-pricing/), [Fractal Apps](https://www.fractalapps.dev/blog/acuity-scheduling-alternatives-for-sms-reminders/)
- The corpus's honest read: "A standalone scheduler is a weak business." Calendly is 4.1/5 and Acuity 3.7/5 on Trustpilot, so complaint volume is moderate. Proposed prices are $9 Solo and $29 Team — [ideas/A02](ideas/A02-scheduling-acuity-calendly-alternative.md)

**A03 LocalLoop (reviews + texting; corpus 22)**
- Podium Core is about $399 and Pro about $599, with a real single-location bill of **$450–600/mo**, 12-month auto-renew contracts, and early exit costing the remaining balance. Birdeye is $299/$349/$449 per location with **90-day written notice**, an ~8% renewal "Innovation Fee" and $500–1,500 onboarding. All of this is **verified in the corpus** — [ideas/A03](ideas/A03-reviews-texting-podium-birdeye-alternative.md), citing [Astucia](https://astucia.io/blog/podium-pricing-2026-what-smbs-actually-pay), [Contractor ToolStack](https://contractortoolstack.com/software/birdeye/pricing/)
- Podium is rated 1.5/5 on Trustpilot against 4.6 on G2, with 62 BBB complaints in 3 years. Birdeye has 108 BBB complaints — [ideas/A03](ideas/A03-reviews-texting-podium-birdeye-alternative.md), citing [BBB](https://www.bbb.org/us/ut/lehi/profile/sales-lead-generation/podium-1166-90023083/complaints)
- The MVP needs done-for-you 10DLC registration, missed-call text-back, an SMS inbox, and GBP review replies ("needs GBP API access approval"). Named cheaper rivals: NiceJob, and GoHighLevel at about $97 with agency white-label — [ideas/A03](ideas/A03-reviews-texting-podium-birdeye-alternative.md)
- Price: $79/location; $129 with AI. GTM: a "technographic cold email" that crawls sites for the Podium or Birdeye webchat script — [ideas/A03](ideas/A03-reviews-texting-podium-birdeye-alternative.md)

**A04 SignFlat (e-sign + quote + deposit; corpus 19)**
- DocuSign Personal is $10–15 for 5 envelopes/mo (1.3/5 on Trustpilot across 1,247 reviews). PandaDoc reviewers report new $2/document fees (2.2/5) — [ideas/A04](ideas/A04-esign-docusign-pandadoc-alternative.md), citing [Verdocs](https://verdocs.com/blog/docusign-pricing), [Trustpilot](https://www.trustpilot.com/review/docusign.com)
- The corpus names a "crowded cheap market (SignWell, BoldSign, Zoho Sign, and Acrobat bundles)". It plans SOC 2 Type I within 6 months. Proposed prices are Free (3 docs), Solo $12 and Team $29 — [ideas/A04](ideas/A04-esign-docusign-pandadoc-alternative.md)
- State contract rules make it a component in 8 state files: the CA down-payment cap, VT written contracts for jobs of $10k+, and PA HICPA — [states/VT-vermont.md](states/VT-vermont.md), [states/PA-pennsylvania.md](states/PA-pennsylvania.md), [states/CA-california.md](states/CA-california.md)

**A05 Quietdesk (helpdesk + AI; corpus 16)**
- Intercom Fin costs $0.99 per outcome, Zendesk AI adds $50/agent, and Help Scout AI Answers is $0.75 per resolution. **Help Scout is free up to 5 users, and Freshdesk is free.** "Gorgias owns Shopify helpdesk mindshare." Intercom has only 12 Trustpilot reviews, and the pain is "not public fury." Proposed prices are $29 and $79 — [ideas/A05](ideas/A05-helpdesk-zendesk-intercom-alternative.md), citing [GetMacha](https://www.getmacha.com/blog/intercom-pricing-explained)

**A06 Coursehouse (courses + community; corpus 20)**
- Kajabi went Basic $149→$179, Growth $199→$249 and Pro $399→$499, dropped the $89 tier, and cut Basic contacts from 10,000 to 2,500. The change applies from the first billing on or after **Jan 13 2026**, with no grandfathering. **Verified** — [ideas/A06](ideas/A06-courses-community-kajabi-teachable-alternative.md), citing [Ruzuku](https://www.ruzuku.com/learn/articles/kajabi-2025-price-increase), [Kajabi](https://kajabi.com/pricing)
- "Annual renewals keep landing through Jan 2027" — [ideas/A06](ideas/A06-courses-community-kajabi-teachable-alternative.md)
- The MVP spans a course builder, video (Mux/Bunny), checkout with subscriptions, payment plans and order bumps, community, email broadcasts, landing pages, migration and a PWA. Risks: Kajabi Payments subscriptions "can't be moved without card re-entry", and "creator churn (launch-cycle businesses)." Thinkific, Mighty and Skool were not re-verified. The market size is a "rough estimate, unverified." Proposed prices are $49 and $99 — [ideas/A06](ideas/A06-courses-community-kajabi-teachable-alternative.md)

**B01 ListFair (email + SMS; corpus 20)**
- Mailchimp's free plan was cut to 250 contacts and 500 sends (Feb 17 2026), and legacy plans rose 11–13% (Apr 13 2026). Klaviyo has billed on active profiles since Feb 18 2025. All of this is verified. The "25% cap" on Klaviyo increases is unverified — [ideas/B01](ideas/B01-email-sms-mailchimp-klaviyo-alternative.md), citing [Audienceful](https://www.audienceful.com/blog/mailchimp-price-increase), [Klaviyo FAQ](https://help.klaviyo.com/hc/en-us/articles/33136281415451)
- Named risks: deliverability reputation ("new senders get throttled"), abuse/KYC, and Klaviyo's Shopify data depth. Prices: $15/$39/$79. The only cheaper rival the corpus mentions is SendX, in a Capterra quote. Constant Contact and ActiveCampaign were not priced — [ideas/B01](ideas/B01-email-sms-mailchimp-klaviyo-alternative.md)

**B02 OwnerCRM (corpus 19)**
- HubSpot Starter is $15–20/seat. Marketing Pro is $890/mo plus $3,000 onboarding. GHL is $97/$297/$497 plus metered add-ons. The corpus itself says "There are dozens of 'simple CRMs'". The MVP spans CRM, two-way Gmail/Outlook sync, a shared inbox, AI automations, booking, forms and a landing builder — [ideas/B02](ideas/B02-smb-crm-hubspot-gohighlevel-alternative.md), citing [TinyCommand](https://tinycommand.com/blogs/hubspot-pricing-explained), [Apexure](https://www.apexure.com/blog/gohighlevel-pricing)

**B03 PostFlat (social scheduling; corpus 17)**
- Hootsuite is $99/user/mo. Buffer is $5–10 per channel. The corpus: "Crowded category: Buffer, Metricool, Publer and Later already sit at low prices"; "we don't win on price there" against Buffer. Most complaint evidence comes from one aggregator (StartupOwl). Platform API dependency is a risk (Meta, TikTok and LinkedIn app review; X is expensive). Prices: $15/$39/$99 — [ideas/B03](ideas/B03-social-scheduling-hootsuite-sprout-alternative.md), citing [Hootsuite](https://www.hootsuite.com/plans), [SaaSPricePulse](https://www.saaspricepulse.com/blog/social-media-management-pricing-comparison-2026)

**B04 FirstCall (owned lead capture + AI text-back; corpus 23, #1 overall)**
- Angi: about $300/yr membership, per-lead costs of $35–120+ by trade, and 1-year contracts that auto-renew unless cancelled 60+ days ahead, with a **35% early-termination fee**. Google LSA averages $53/lead. Manual LSA disputes were removed in Jul 2024, and the **$2k Google Guarantee was eliminated Nov 7 2025**. All of this is verified — [ideas/B04](ideas/B04-owned-lead-capture-home-services-angi-thumbtack-lsa.md), citing [LeadTruffle](https://www.leadtruffle.co/blog/complete-guide-angi-leads-home-service-contractors-2026/), [Footbridge Media](https://www.footbridgemedia.com/marketing-tips/5-changes-google-local-service-ads-contractors-should-know), [Valley Marketing Group](https://thevalleymarketinggroup.com/blog/google-local-services-ads-cost-per-lead-2026/)
- "35–50% of jobs go to the first contractor to respond." The Oct–Feb HVAC and plumbing season "is when missed calls cost the most" — [ideas/B04](ideas/B04-owned-lead-capture-home-services-angi-thumbtack-lsa.md)
- The MVP core is a phone number or forwarding layer with missed-call text-back in 5 seconds and an AI qualifier that texts every lead within 60 seconds. Prices: $49/$99/$199, with texts at cost + 10%. Named crowding: "GoHighLevel agencies, Podium, Jobber and LeadTruffle-type tools" — [ideas/B04](ideas/B04-owned-lead-capture-home-services-angi-thumbtack-lsa.md)
- Top-3 in 40 of 51 states — [INDEX.md §1](INDEX.md)

**B05 ListingKeep (local listings; corpus 16)**
- In the Whitespark Yext-cancellation test, 25% of listings disappeared and 35% reverted. Yext has only 11 BBB complaints in 3 years, and the corpus says the pain is "structural... more than high-volume anger." Competing prices: BrightLocal from $39, **Moz Local $129/yr**, Semrush Local $139.95 + $20/location. Build ease is 2 because "scraping and directory claim flows vary widely and break often." Proposed price: $15 for a single location — [ideas/B05](ideas/B05-local-listings-reputation-yext-brightlocal-alternative.md), citing [Whitespark](https://whitespark.ca/blog/what-happens-when-you-cancel-yext/), [Surferstack](https://surferstack.com/guides/local-seo-tools-comparison-2026-brightlocal-vs-semrush-local-vs-moz-local)

**B06 RingFlat (business phone + call tracking; corpus 18)**
- The MVP needs "Mobile, desktop and web apps via WebRTC", porting, and E911/CNAM/STIR-SHAKEN/10DLC. "Phones are mission-critical", with "24/7 support for outages." Two-party recording consent applies. Quo starts at $15–19/user. RingCentral has 541 BBB complaints, with a cluster in Jul–Aug 2026 — [ideas/B06](ideas/B06-business-phone-call-tracking-ringcentral-callrail-alternative.md), citing [BBB](https://www.bbb.org/us/ca/belmont/profile/telecommunications/ringcentral-inc-1116-65952/complaints), [CallRail blog](https://www.callrail.com/blog/quo-review)

**B07 StudioDesk (HoneyBook/Dubsado alternative; corpus 19, cut from 20)**
- HoneyBook's own page (Sep 24 2026), billed yearly: Starter $29, Essentials $49, Premium $109. Monthly billing: Essentials $59, Premium $129. Card fees start at 2.7% + 10¢; ACH is 1.5%. The corpus concludes that moving to the creative's own Stripe "does not save on card fees" — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md), citing [HoneyBook pricing](https://www.honeybook.com/pricing)
- The Feb 4 2025 hike was +51–89%. The 20% loyalty discount "expired Feb 4 2026", but that claim comes **only from a competitor blog** (Talleflow) — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md), citing [Fstoppers](https://fstoppers.com/business/honeybooks-price-hike-coming-heres-what-need-know-and-how-save-690584), [Talleflow](https://www.talleflow.com/blog/why-honeybook-users-are-switching-in-2026-and-what-to-look-for-instead)
- BBB complaints describe fund holds and dispute withdrawals (Sep and Nov 2025). The totals are only 17 BBB complaints in 3 years, and Trustpilot is 4.0/5, so "anger is concentrated on price and payments" — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md), citing [BBB](https://www.bbb.org/us/ca/san-francisco/profile/records-management/honeybook-inc-1116-878229/complaints?page=1)
- Named crowding: "Dubsado, 17hats, Bonsai, Studio Ninja, Sprout Studio, Táve/VSCO Workspace, Plutio." Payments run through Stripe Connect Standard ("We never hold funds"). The off-season (Nov–Feb) is "the next window." Proposed prices: $19 Solo, $39 Studio — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md)
- GA, NV, SC and TN list B07 for their wedding hubs — [states/NV-nevada.md](states/NV-nevada.md), [states/GA-georgia.md](states/GA-georgia.md)

**L01 FlatFlow (Zapier/Make alternative; corpus 18)**
- Zapier Professional is $19.99–29.99 for 750 tasks (1.3/5 on Trustpilot). Make "typically saves $200–400/mo versus Zapier at 5,000+ tasks". n8n and Activepieces are free or cheap. The MVP needs 25 connectors, plus "Google restricted scopes need a CASA security assessment" and Microsoft publisher verification ("budget 4–8 weeks"). "Reliability is the product" — [ideas/L01](ideas/L01-automation-flat-price-zapier-make-alternative.md), citing [Automation Atlas](https://automationatlas.io/answers/zapier-pricing-changes-2025-2026/)

**L02 Studioboard (flat-price PM; corpus 19)**
- monday.com sells seats in blocks ("a team of six buys ten"). ClickUp is $7/user plus AI at $9–28/seat. Basecamp already sells a flat plan. The two monday pricing sources conflict. The corpus: "the market is crowded, and ClickUp is already cheap per seat." It also expects SOC 2 questionnaires from agency clients — [ideas/L02](ideas/L02-project-management-flat-price-monday-asana-clickup-alternative.md), citing [Rock](https://www.rock.so/blog/monday-pricing), [PricePulse](https://www.getpricepulse.com/blog/monday-price-increase-2026.html)

**L03 StackSaver (Shopify all-in-one; corpus 20)**
- Prices verified Aug 2 2026: Judge.me $15, Loox $49.99 for 300 orders, Smile $15 for 500 orders, and Yotpo's useful tiers from $129. "Vitals and similar '40+ apps in one' bundles already exist." Each module "must match the core of a specialist app." The App Store ranking moat is held by Judge.me, Klaviyo and Yotpo. The trigger is the "app bill audit in Q4 prep (Sept–Oct, ahead of BFCM)" — [ideas/L03](ideas/L03-shopify-app-bundle-reviews-upsell-popup-loyalty-alternative.md), citing [PandaCodeGen](https://www.pandacodegen.com/blog/shopify-app-costs-real-monthly-bill)

**L04 ClipSOP (Loom alternative + auto-SOP; corpus 18)**
- Loom Business is $18/user and Business + AI $24/user. The Creator Lite role is being discontinued: existing users are auto-promoted to paid at the next billing date after the Atlassian integration, and it is deprecated for net-new users after Feb 2026. The "$240/yr to $24,000/yr" anecdote comes from secondary and competitor sources — [ideas/L04](ideas/L04-async-video-sop-loom-alternative.md), citing [Atlassian Support](https://support.atlassian.com/loom/docs/loom-customer-integration-with-atlassian-pricing-billing-and-role-changes/), [Supademo](https://supademo.com/blog/loom-pricing)
- Cheap challengers already exist: Cap.so (open source, $9 hosted), Tella, Screen Studio and CleanShot X. "Scribe and Tango sell SOP capture." The corpus: "pure 'cheap Loom' is crowded"; "Validate that no competitor already ships this exact combination." The Chrome Web Store is a listed channel — [ideas/L04](ideas/L04-async-video-sop-loom-alternative.md)

**L05 Harbor (Jira/Confluence DC exit; corpus 13)**
- DC timeline: no new licenses after Mar 30 2026, last renewals Mar 30 2028, read-only Mar 28 2029, and ~15% price rise Feb 17 2026. Buyers are IT managers at 50–1,000-person orgs (defense, government, regulated industries). "This is not a card-swipe buyer"; expect security review. Market: "low thousands of US organizations" (estimate) — [ideas/L05](ideas/L05-self-hosted-wiki-tracker-jira-confluence-data-center-alternative.md), citing [The Register](https://www.theregister.com/2025/09/09/atlassian_will_go_cloudonly_customers/), [ONES](https://ones.com/blog/atlassian-data-center-pricing-increase-2026/)
- CMMC Phase II was suspended Jul 13 2026, which removes a near-term forcing function — [states/AL-alabama.md](states/AL-alabama.md)

**L06 OfficeKeys (office password manager; corpus 14)**
- Bitwarden Teams is $4/user. The corpus: "weak on price gap... writing new vault crypto is a liability"; "the MSP is often the real decision-maker"; and the licensing of Bitwarden server components "varies by component" — [ideas/L06](ideas/L06-office-password-manager-lastpass-1password-alternative.md), citing [TeamPassword](https://teampassword.com/blog/1password-alternatives) (competitor source)

### Inferences

**Full score table (all scores are my judgment, applying the rubric to the evidence above)**

Columns: 1 Build scope · 2 Regulatory · 3 Self-serve · 4 Distribution · 5 WTP/ARPU · 6 Gap vs cheap indie · 7 Urgency Oct 2026–Apr 2027 · 8 Support/retention. Kill flags: K1 HIPAA · K2 payments/holding funds · K3 telephony/SMS 10DLC at scale · K4 hardware/offline mobile · K5 enterprise/government/committee · K6 50-state legal liability · K7 feature-parity monster · K8 crowded with cheap indie tools. "(c)" = conditional, meaning the flag applies only if the corpus's full scope is built.

| ID | Product | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | **/40** | Kill flags | Corpus /25 | Verdict |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| B07 | StudioDesk (HoneyBook alt.) | 3 | 4 | 5 | 4 | 3 | 2 | 4 | 3 | **28** | K8 (partial) | 19 | **Shortlist #1** |
| L04 | ClipSOP (Loom alt. + SOP) | 4 | 4 | 5 | 5 | 3 | 1 | 3 | 3 | **28** | K8 | 18 | **Shortlist #5 (conditional)** |
| A06 | Coursehouse (Kajabi alt.) | 2 | 4 | 4 | 4 | 5 | 2 | 4 | 2 | **27** | K7; K8 (partial) | 20 | **Shortlist #3 (narrowed only)** |
| B04 | FirstCall (lead capture + text-back) | 3 | 3 | 3 | 4 | 5 | 3 | 4 | 2 | **27** | K3; K8 (partial) | 23 | **Shortlist #2** |
| A04 | SignFlat (e-sign + deposit) | 4 | 3 | 5 | 4 | 2 | 2 | 2 | 4 | **26** | K8 | 19 | Component inside B07; not standalone |
| L03 | StackSaver (Shopify bundle) | 2 | 4 | 5 | 4 | 3 | 2 | 2 | 3 | **25** | K7, K8 | 20 | Out for now (BFCM 2026 window missed) |
| A03 | LocalLoop (reviews + texting) | 3 | 2 | 3 | 4 | 5 | 2 | 3 | 2 | **24** | K3; K8 (partial) | 22 | **Shortlist #4, as a module on B04's codebase** |
| A05 | Quietdesk (helpdesk) | 2 | 4 | 4 | 4 | 3 | 2 | 2 | 3 | **24** | K7, K8 | 16 | Out |
| B03 | PostFlat (social scheduler) | 3 | 4 | 5 | 4 | 2 | 1 | 2 | 3 | **24** | K8 | 17 | Out (low ARPU + platform API risk) |
| B05 | ListingKeep (listings) | 2 | 4 | 5 | 4 | 2 | 2 | 2 | 3 | **24** | K8 | 16 | Out |
| A01 | FormFlare (forms) | 3 | 2 | 5 | 4 | 2 | 2 | 2 | 3 | **23** | K8; K1 (c); K3 (c) | 19 | Out standalone; use as intake component |
| A02 | BookFlat (scheduling) | 4 | 3 | 5 | 4 | 1 | 1 | 2 | 3 | **23** | K8 | 16 | Out; component only |
| L02 | Studioboard (flat PM) | 2 | 4 | 3 | 3 | 4 | 1 | 2 | 4 | **23** | K7, K8 | 19 | Out |
| B01 | ListFair (email/SMS) | 2 | 3 | 5 | 4 | 3 | 1 | 2 | 2 | **22** | K8, K7 (partial); K3 (c, SMS V2) | 20 | Out |
| B02 | OwnerCRM | 2 | 3 | 4 | 3 | 4 | 1 | 1 | 3 | **21** | K7, K8 | 19 | Out |
| L01 | FlatFlow (automation) | 1 | 2 | 4 | 4 | 3 | 2 | 2 | 2 | **20** | K7, K8 | 18 | Out |
| B06 | RingFlat (phone + call tracking) | 1 | 1 | 3 | 3 | 4 | 2 | 2 | 1 | **17** | K3, K4, K7 | 18 | Out (3 flags) |
| L05 | Harbor (Jira DC exit) | 1 | 2 | 1 | 2 | 5 | 2 | 2 | 2 | **17** | K5, K7 | 13 | Out |
| L06 | OfficeKeys (password mgr) | 2 | 1 | 3 | 3 | 3 | 1 | 2 | 2 | **17** | K8 (+ vault security liability, MSP channel) | 14 | Out |

**How I applied the WTP column (judgment):** 5 = $49+/mo is credible as the typical price; 4 = $35–49; 3 = $25–35; 2 = $15–25; 1 = under $15. Each score uses the buyer's current spend and the corpus's proposed price.

**Per-idea reasoning (judgment, based on the cited evidence)**
- **B07 (28).** The core is CRUD, documents and Stripe Connect Standard, with no fund-holding. It is ESIGN/UETA only, so regulation is light. The owner buys alone by card and is reachable through very large photographer Facebook groups, educators and WPPI. The Nov–Feb off-season is a dated window that falls inside the next 6 months. The weaknesses are the subscription gap, which the corpus cut to $120–480/yr, and a crowded field of $15–40 rivals (Dubsado, 17hats, Bonsai, Studio Ninja, Plutio). Most of those are not $0 tools, so K8 is only partial. The pitch has to be "your money never touches us, plus a simpler flow," not price.
- **L04 (28).** It scores high on build (browser extension plus hosted video) and on distribution (the Chrome Web Store and r/sysadmin's Loom-migration threads), but it scores **1 on the gap**. Cap.so at $9, Tella, Scribe and Tango are in the corpus. Other video-to-guide tools that the corpus does not list may also exist (judgment, needs verification). Its total is inflated by easy-to-sell criteria, and K8 is firm, so it stays a cheap, conditional experiment.
- **A06 (27).** It has the best ARPU here ($49–99 against Kajabi's $179–499). The dated window runs until Kajabi's last annual renewals land, which the corpus puts at "through Jan 2027", so roughly mid-Jan 2027. Kajabi sites can be found and cold-emailed. But matching Kajabi's all-in-one scope is a K7 problem, and migration (videos, Kajabi Payments subscriptions needing card re-entry) is support-heavy, with launch-cycle churn on top. It is viable only as a narrowed course-first wedge.
- **B04 (27).** It has high ARPU ($49–199), owner-operator card buyers, the strongest state-level demand (40 top-3s), and a pain season that is happening now (Oct–Feb). The core value, text-back within seconds, depends on SMS and 10DLC, so K3 is firm. Telephony support load scores 2. Missed-call text-back is already commoditized by GHL agencies, so K8 is partial. What differentiates it is the lead-source ROI board, the cost per booked job, and parsing of Angi/Thumbtack/LSA lead emails.
- **A04 (26).** It is easy to build and low on support, but at $12–29 the ARPU is low and the space is crowded (SignWell, BoldSign, Zoho Sign). It works best as the signing engine inside B07, which needs ESIGN/UETA signing anyway.
- **L03 (25).** The Shopify App Store distribution is excellent, but the bundle concept is K7 (5–8 modules that each have to match a specialist app) and K8 (Vitals, and Judge.me at $15). Its only dated trigger is the pre-BFCM audit in Sept–Oct. Black Friday 2026 is Nov 27, so merchants freeze changes in early November (judgment), and a 4–6-week build started today (Oct 10) ships Nov 7–21. **The 2026 window is effectively missed.**
- **A03 (24).** It has the best price gap in the group ($450–600 down to $79), very solo-friendly technographic cold email, and a contract-escape lead magnet. But SMS/10DLC sits at the core (K3), onboarding is not under an hour (10DLC vetting plus number forwarding), and GHL agencies sell the same bundle at $97. It shares about 70% of its infrastructure with B04 (inbox, SMS, review requests), so it should be built as B04's second module.
- **A05, B01, B02, L01, L02** each carry two or more flags. Helpdesk, ESP, CRM, automation and PM are all categories where buyers expect parity, and each has free or cheap tiers. For B01 the cheap-ESP crowding is my judgment, because the corpus never lists low-cost ESPs (see Q3 verification asks).
- **B03, B05, A02, A01** each have one flag, but ARPU is ≤$25 and the field is crowded, which is a bad combination when you need revenue fast. A01 and A02 make sense only as components: intake forms inside B07 and B04, and booking inside B07.
- **B06, L05, L06** are out on structural grounds. B06 needs telecom, mobile apps and 24/7 support. L05 sells to enterprise and government with on-prem fidelity demands. L06 carries vault-security liability against $4/user Bitwarden.

**Switching-window dates that have already passed (as of Oct 10 2026)**
- These passed but still drive *rolling* renewals: Kajabi hike (Jan 13 2026; annual renewals through ~Jan 2027), HoneyBook loyalty-discount expiry (Feb 4 2026), Loom Creator Lite deprecation for new users (after Feb 2026; existing users promoted at the next billing date), monday Service +18% (Feb 10 2026, at renewal), monday AI credits (May 6 2026), Mailchimp legacy hike (Apr 13 2026).
- These passed and are now stale as hooks: Mailchimp free-plan cut (Feb 17 2026), Atlassian DC new-license cutoff (Mar 30 2026) and its 15% rise (Feb 17 2026), 1Password hike (Mar 2026), Calendly AI tiers (Aug 19 2026), Google Guarantee removal (Nov 7 2025), LastPass ICO fine (Dec 14 2025), Teachable restructure (Jun 2025), Klaviyo active-profile billing (Feb 18 2025), NAR buyer agreements (Aug 17 2024), Dropbox Sign breach (May 2024).
- These are effectively missed for 2026: the L03 pre-BFCM audit window (Sept–Oct). The next one is a post-holiday cost review (judgment) or Sept 2027.
- These still lie ahead within Oct 2026–Apr 2027: the B07 wedding off-season (Nov–Feb), the B04 heating and plumbing season (Oct–Feb), the last Kajabi annual renewals at the hiked price (to ~mid-Jan 2027), and A03's rolling Podium/Birdeye 90-day notice deadlines (renewals in Jan–Apr 2027 have notice deadlines in Oct 2026–Jan 2027).
- This lies outside the window: L05's Mar 2028 last renewal and Mar 2029 read-only date.

### Gaps
- No web verification was done, so scores rest on Sep 24–25 2026 corpus prices. Thirteen of the 19 files never had a fact-check pass (see above).
- The cheap-indie competitor density is under-researched in the corpus for B01 (no low-cost ESPs are named), A06 (Thinkific, Mighty and Skool not re-verified), B07 (rival prices "not verified this pass"), L04 ("validate that no competitor already ships this exact combination") and L03 (Vitals "verify"). My K8 calls for B01 and L04 rest partly on general knowledge and need confirmation.
- Market sizes for all 19 are labeled estimates in the corpus. None gives a verified count of reachable buyers in a solo channel, such as the number of HoneyBook users or Kajabi sites.
- The 10DLC ISV registration time and cost in Oct 2026, which drive the K3 severity for B04 and A03, are not in the corpus.

## Key question 2: where the corpus's /25 score disagrees with the solo-developer view, and why

### Takeaway
The corpus ranks B04 > A03 > A06/B01/L03 at the top of this group. The solo view ranks B07 ≈ L04 > A06 ≈ B04 > A04. The biggest disagreements come from three things the corpus scores do not measure: crowding by cheap indie tools (the corpus measures price gap against the *expensive* incumbent), support and regulatory load (telephony, SMS, HIPAA, vault security), and the feature parity customers need before switching (corpus "Build ease" measures coding effort, not switching parity). The corpus also rewards total market size, which matters little to a founder who needs 100–500 customers.

### Cited Findings
- The corpus criteria are Pain, Price gap, Build ease, Sales speed and Market size, with a state-weighted Priority on top. There is no criterion for indie competition, support load or regulatory burden — [INDEX.md](INDEX.md)
- Corpus scores for this group: B04 23, A03 22, A06 20, B01 20, L03 20, A01 19, A04 19, B02 19, B07 19, L02 19, B06 18, L01 18, L04 18, B03 17, A02 16, A05 16, B05 16, L06 14, L05 13 — [_scoreboard.csv](_scoreboard.csv)
- The corpus gives Market size 5 to A01, A03, B01, B02, B04, B06, L01 and L02 — [ideas/A01](ideas/A01-forms-typeform-jotform-alternative.md), [ideas/A03](ideas/A03-reviews-texting-podium-birdeye-alternative.md), [ideas/B01](ideas/B01-email-sms-mailchimp-klaviyo-alternative.md), [ideas/B02](ideas/B02-smb-crm-hubspot-gohighlevel-alternative.md), [ideas/B04](ideas/B04-owned-lead-capture-home-services-angi-thumbtack-lsa.md), [ideas/B06](ideas/B06-business-phone-call-tracking-ringcentral-callrail-alternative.md), [ideas/L01](ideas/L01-automation-flat-price-zapier-make-alternative.md), [ideas/L02](ideas/L02-project-management-flat-price-monday-asana-clickup-alternative.md)
- The corpus gives L02 Build ease 4 while admitting "the market is crowded, and ClickUp is already cheap per seat" — [ideas/L02](ideas/L02-project-management-flat-price-monday-asana-clickup-alternative.md)
- The corpus gives B01 a Price gap of 4, measured against Mailchimp ($100/mo at 5,000 contacts against ListFair's $39). No low-cost ESP is priced — [ideas/B01](ideas/B01-email-sms-mailchimp-klaviyo-alternative.md)
- The corpus gives B06 Sales speed 4 and Market size 5 while listing E911, porting, STIR/SHAKEN, mobile apps and "24/7 support for outages" as requirements — [ideas/B06](ideas/B06-business-phone-call-tracking-ringcentral-callrail-alternative.md)
- The corpus gives L03 Sales speed 5 because of the App Store and the Sept–Oct BFCM audit timing — [ideas/L03](ideas/L03-shopify-app-bundle-reviews-upsell-popup-loyalty-alternative.md)
- The corpus cut B07's Price gap from 4 to 3 after HoneyBook's own page showed $29/$49/$109 billed yearly and card fees from 2.7% + 10¢ — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md)
- The corpus scores B07's and A06's Market size at 3, below most horizontal tools — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md), [ideas/A06](ideas/A06-courses-community-kajabi-teachable-alternative.md)
- The corpus's INDEX itself warns that A01's "free and cheap tier is crowded" (Tally) — [INDEX.md §2](INDEX.md)

### Inferences
**Rank comparison (judgment; solo totals from the Q1 table)**

| ID | Corpus /25 (rank in group) | Solo /40 (rank in group) | Direction | Main reason for the gap |
|---|---|---|---|---|
| B07 | 19 (6–10) | 28 (1–2) | ▲ big | The corpus penalizes Market size (3), which doesn't matter for a solo founder needing about 350 customers. The solo view rewards the simple build, card-paying owner, Facebook-group distribution and the Nov–Feb dated window. |
| L04 | 18 (11–13) | 28 (1–2) | ▲ big, but flagged K8 | The Chrome Web Store and a browser-only build score high on the solo rubric. The corpus underrates distribution. The solo rubric still flags the crowding (gap 1). |
| A04 | 19 (6–10) | 26 (5) | ▲ | Low support and an easy build help solo. Low ARPU and crowding keep it as a component. |
| B03 | 17 (14) | 24 (7–10) | ▲ total, but still out | Self-serve and distribution are easy, yet ARPU ≤$25 plus Buffer/Metricool/Publer crowding kill it. |
| A06 | 20 (3–5) | 27 (3–4) | ≈ agree | Both views like the pain, price gap and urgency. They disagree on build: corpus 3, solo 2, because creators expect Kajabi-level breadth (K7), and migration and churn add support load. |
| B04 | 23 (1) | 27 (3–4) | ▼ slightly | The corpus's Build ease 4 and Sales speed 5 ignore 10DLC onboarding delay, TCPA exposure and telephony support (K3). Still shortlisted. |
| A03 | 22 (2) | 24 (7–10) | ▼ | The same telephony and SMS burden as B04, plus GHL agencies selling the identical bundle at $97. The corpus Price gap of 5 is real, but cheap substitutes exist below Podium. |
| L03 | 20 (3–5) | 25 (6), with 2 flags | ▼ effectively | A bundle is a parity problem across 5–8 specialist apps, and the BFCM window is missed for a build that starts today. |
| B01 | 20 (3–5) | 22 (14) | ▼ big | The corpus measures the gap against Mailchimp and Klaviyo, not against low-cost ESPs (judgment). Deliverability and abuse policing carry heavy support load. |
| A01 | 19 (6–10) | 23 (11–13) | ▼ | Tally (free/$24) and Fillout. The differentiators the corpus picks (HIPAA tier, SMS forms, offline kiosk) are exactly the regulated or hard parts. |
| L02, B02, L01 | 19, 19, 18 | 23, 21, 20 | ▼ | Corpus Market size 5 and Build ease 3–4 hide parity and integration expectations in PM, CRM and automation (K7). Each is crowded with cheap or free tools (K8). |
| B06 | 18 (11–13) | 17 (17–19) | ▼ big | Telecom (K3, K4, K7) and 24/7 support. The corpus's Market size 5 and Sales speed 4 hide this. |
| A02, A05, B05 | 16 each | 23, 24, 24 | ≈ agree (weak) | Both views agree these are weak, and both see the cheap or free competition. |
| L05, L06 | 13, 14 | 17, 17 | ≈ agree (out) | Both views put them at the bottom. Enterprise buyer and on-prem fidelity for L05; vault liability and Bitwarden at $4 for L06. |

- **Systematic bias 1 (judgment):** The corpus "Price gap" compares against the incumbent named in the title (Typeform, Hootsuite, Mailchimp, Zapier, monday), not against the cheapest good alternative. For a solo founder, the relevant competitor is the $0–30 indie tool the buyer finds in the same Google search.
- **Systematic bias 2 (judgment):** The corpus "Build ease" counts lines of code for an MVP. The solo rubric's criterion 1 asks whether customers would *switch* to that MVP. Helpdesk, CRM, PM, ESP, automation and all-in-one course platforms fail that test even when the code is easy with Claude.
- **Systematic bias 3 (judgment):** Telephony and SMS ideas (B04, A03, B06) get high Sales speed in the corpus because owners buy fast. The corpus does not price in 10DLC brand and campaign vetting for each customer, TCPA and FL FTSA exposure, or call-quality support. This makes the corpus's "Bet 1: home-services front office" riskier for a solo developer than the INDEX suggests.
- **Systematic bias 4 (judgment):** The state-weighted Priority favors ideas with many local law hooks (B04 at 40 states, A03 at 24). For horizontal tools sold online, state hooks matter mostly as marketing angles: WI §134.49 for A03, NV/WA health-data consent for A01, CA/VT/PA contract rules for A04.
- **Source-quality caveat (from the corpus's own labels):** Several key claims rest on competitor or vendor blogs. These include Talleflow for B07's loyalty-discount expiry, Screenify and Supademo for L04's $24k claim, TeamPassword for L06, and ONES for L05. LeadTruffle, the main Angi-pricing source for B04, sells the kind of tool the B04 file lists as a competitor ("LeadTruffle-type tools"). The corpus scores do not discount for this.

### Gaps
- The corpus gives no reasoning for its per-criterion numbers beyond the evidence bullets, so I can't tell whether its raters considered indie competition and simply weighed it differently.
- I have no fresh data on cheap-tool prices (MailerLite-class ESPs, Cap/Tella, Dubsado and similar), so the size of disagreement on criterion 6 is judgment that needs the validation round.

## Key question 3: the 3–5 best for this founder, their narrowest sellable wedges, and what to verify on the web

### Takeaway
Shortlist, ranked for "solo, built with Claude, revenue fast in the US":
1. **B07 StudioDesk**, as a HoneyBook exit kit for wedding and portrait photographers.
2. **B04 FirstCall**, as speed-to-lead plus cost per booked job for HVAC and plumbing owners who buy marketplace leads.
3. **A06 Coursehouse**, as a Kajabi renewal escape for course-first creators.
4. **A03 LocalLoop**, as a Podium/Birdeye contract-escape module on B04's codebase.
5. **L04 ClipSOP**, conditional, as a cheap experiment for Creator Lite refugees.

B07 and A06 have dated windows that end by ~Jan–Feb 2027, so build speed matters: ship by mid-November. A04, A01 and A02 are not standalone bets, but their engines (e-sign, intake forms, booking) are reused inside B07 and B04.

### Cited Findings
- B07 buyers: solo and 2–5-person creatives who buy by card, "influenced by peer Facebook groups and educators". The off-season (Nov–Feb) is when "wedding pros rebuild their systems." The corpus launch offer is "Bring your HoneyBook invoice, get 12 months at $9/mo", timed to the Nov–Feb off-season. Educators get a 30% recurring affiliate share for 12 months — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md)
- B07 MVP items the corpus lists: an importer (HoneyBook, Dubsado and 17hats CSVs, with AI conversion of contract PDFs), an inquiry form with a 60-second auto-reply, a one-link proposal → contract → invoice flow, Stripe Connect Standard with payment schedules, and plain reports — [ideas/B07](ideas/B07-client-management-creatives-honeybook-dubsado-alternative.md)
- A04's MVP audit trail (ESIGN/UETA consent, IP, timestamp, SHA-256 hashed PDF, certificate) and its "quote, sign and deposit in one link" are the same engine B07 needs — [ideas/A04](ideas/A04-esign-docusign-pandadoc-alternative.md)
- B04 MVP items: missed-call text-back in 5 seconds, a unified lead inbox that parses forwarded Angi/Thumbtack/LSA lead emails, an AI qualifier within 60 seconds, and a lead-source ROI board ("Angi cost you $1,340 for 2 jobs this month"). Mitigation: "conversational texts only (responding to inbound inquiries)." Launch metros: DFW, Tampa Bay, Phoenix, Atlanta — [ideas/B04](ideas/B04-owned-lead-capture-home-services-angi-thumbtack-lsa.md), [INDEX.md §2](INDEX.md)
- B04's GTM includes "Scrape Angi/LSA-listed pros per metro and text them" — [ideas/B04](ideas/B04-owned-lead-capture-home-services-angi-thumbtack-lsa.md). FL's FTSA requires prior express written consent for automated sales texts, at $500 per violation — [states/FL-florida.md](states/FL-florida.md)
- A06 GTM: "find creators whose sites are on Kajabi (mykajabi.com subdomains or Kajabi-hosted checkout) and email them a personalized savings estimate before their renewal". Kajabi experts and launch agencies get a 30% recurring referral. Migration is easy "when the creator used their own Stripe" — [ideas/A06](ideas/A06-courses-community-kajabi-teachable-alternative.md)
- A03 GTM: scan local-business websites for the Podium or Birdeye webchat script. The "Contract escape kit" calculates the notice deadline and generates the non-renewal letter. "Free until your contract ends" covers up to 60 days of overlap — [ideas/A03](ideas/A03-reviews-texting-podium-birdeye-alternative.md). Wisconsin §134.49 gives a statutory exit when the disclosure or notice is missing — [states/WI-wisconsin.md](states/WI-wisconsin.md)
- L04 MVP items: a browser recorder, free Contributors (up to 10 videos/mo each), Auto-SOP (transcript plus key frames, exported to Google Docs/Notion/Confluence/PDF), and a Loom MP4 importer. Prices are $29 Team and $79 Company, flat — [ideas/L04](ideas/L04-async-video-sop-loom-alternative.md)

### Inferences

**#1 B07: "HoneyBook Exit Kit" for wedding and portrait photographers (judgment)**
- **Ships in 4–6 weeks:**
  - an importer for HoneyBook client and project CSVs, plus AI conversion of uploaded contract PDFs into merge-field templates
  - a branded inquiry form with a 60-second auto-reply that sends the pricing guide
  - one link per booking: package choice → ESIGN/UETA signature (A04 engine) → retainer payment through Stripe Connect Standard
  - a payment schedule (retainer, then balance due N days before the event) with auto-reminders
  - a pipeline board and income/outstanding report with CSV export
- **Deferred:** the scheduler (link out to the user's existing booking tool at first), workflows, client portal, galleries and a mobile app.
- **Buyer:** a solo wedding or portrait photographer (or videographer) on HoneyBook Essentials ($49 yearly / $59 monthly) or Dubsado who is angry about the 2025 hike or a fund hold.
- **Price:** **$29/mo month-to-month, or $290/yr.** Launch offer: first 3 months at $9 for anyone who uploads a HoneyBook invoice. At $29, $10k MRR needs about 345 customers. The corpus's $19 would need about 525, which is too many to be "fast." The corpus's pricing shows HoneyBook Starter at $29 billed yearly, so the pitch is "Essentials-level features at Starter price, month-to-month, your money never held," not "cheapest."
- **Channel:** wedding-photographer business Facebook groups and r/WeddingPhotography (answer HoneyBook price and payout threads), 2–3 photography-business educators on a 30% recurring affiliate deal, and "HoneyBook alternative for photographers" / "HoneyBook funds held" SEO pages, all timed to Nov–Feb.
- **Why #1:** fewest flags, no telephony, an owner card buyer, and a live seasonal window. It also reuses A01, A02 and A04 engines that can be sold to adjacent creatives later.

**#2 B04: speed-to-lead plus cost per booked job for HVAC and plumbing shops (judgment)**
- **Ships in 4–6 weeks:**
  - a forwarding address that parses Angi, Thumbtack, LSA and website-form lead emails into job cards (AI extraction)
  - an auto-text within 60 seconds from a local number registered through the CPaaS's ISV 10DLC flow, sent only to inbound leads (conversational)
  - a missed-call text-back via call forwarding
  - a mobile-web "mark booked / $ amount" tap, feeding a per-source ROI board (cost per lead and per booked job, using the owner's entered lead spend)
  - **Fallback while 10DLC vetting is pending:** a push or email alert carrying a prefilled `sms:` link, so the owner texts from their own phone in one tap. This avoids carrier registration in week one.
- **Deferred:** the AI voice receptionist, the dispute helper (LSA manual disputes no longer exist, so its value is limited), Jobber/Housecall Pro sync, and review requests (that becomes the A03 module).
- **Buyer:** the owner of a 1–10-truck HVAC or plumbing shop spending $1k+/mo on Angi, LSA or Thumbtack.
- **Price:** $99/mo Crew, $49 Solo, SMS at cost + 10%. $10k MRR needs about 100–200 customers.
- **Channel:** r/HVAC, r/Plumbing and r/sweatystartup; owner Facebook groups; **cold email (not cold text)** to pros listed on Google LSA or Angi in DFW and Phoenix. The corpus's "text them" suggestion risks FTSA and TCPA exposure (judgment).
- **Why #2:** highest ARPU among the low-parity ideas, and the pain season is happening now. K3 is the real cost, so budget about 2 weeks for 10DLC ISV setup and expect carrier rejections.

**#3 A06: "Kajabi Renewal Escape" for course-first creators (judgment)**
- **Ships in about 6 weeks (tight):**
  - a course player (modules, lessons, drip) with video on Bunny Stream or Mux at cost
  - checkout in the creator's own Stripe (one-time, subscription, payment plan, coupons) at 0% platform fee
  - a member area with progress tracking
  - CSV member import with course access, plus Claude-scripted done-for-you video and course migration
  - always-free full export
- **Scope cuts:** **no** native community (link to the creator's Discord or Circle), **no** ESP (sync contacts to Kit or MailerLite by API), only a simple sales-page template, and no affiliates or apps. This avoids the K7 trap by saying "we replace Kajabi's course + checkout, keep your favorite email tool."
- **Buyer:** Kajabi Basic or Growth creators whose revenue comes mainly from 1–5 courses and who are either over the 2,500-contact cap or have an annual renewal between now and ~mid-Jan 2027. Creators on their own Stripe come first, because they need no card re-collection.
- **Price:** $49/mo Creator, $99/mo Pro. $10k MRR needs about 100–200 customers.
- **Channel:** identify Kajabi-hosted sites (mykajabi.com subdomains, Kajabi checkout) and cold-email a personalized savings estimate before each creator's renewal; a "Kajabi price increase 2026" calculator page; freelance Kajabi experts as paid migration partners.
- **Why #3:** best ARPU and a dated window, but the riskiest build and support profile among the top three. Treat it as an alternative to B07 rather than a parallel bet.

**#4 A03: Podium/Birdeye "Contract Escape + Reviews" as module 2 on the B04 codebase (judgment)**
- **Ships in about 3–4 weeks on top of B04's infrastructure:**
  - the contract-escape kit (start date → notice deadline → non-renewal letter → reminders at 100/95/91 days), with WI §134.49 and NY GOL §5-903 checks marked "verify"
  - review requests by SMS and email after a job completes (CSV, Zapier, or a B04 "booked/done" tap)
  - webchat-to-SMS and a shared inbox
- **Deferred:** GBP AI replies until API access is approved, and text-to-pay.
- **Buyer:** 1–5-location home-service owners paying Podium ($450–600 real) or Birdeye ($299–449 + 8%).
- **Price:** $79/location flat.
- **Channel:** a technographic crawl for the Podium/Birdeye widget → cold email "your contract renews around X; here is the letter + $79 flat"; "how to cancel Podium" SEO.
- **Why only #4:** it shares B04's K3 burden, and revenue arrives only at each customer's contract end. It is a strong second product, not a first one.

**#5 L04 (conditional): "Creator Lite refugee pack" (judgment)**
- **Ships in 4–5 weeks:**
  - a Chrome extension recorder (screen, camera, mic) with instant share links on Cloudflare Stream or Mux
  - free contributors and unlimited viewers, with $29 flat for 5 power creators
  - Auto-SOP export to Google Docs or Notion
  - an MP4 folder importer for Loom libraries
- **Buyer:** ops leads at 5–100-person SMBs whose Loom bill rose when Creator Lite users were auto-promoted.
- **Price:** $29 Team / $79 Company.
- **Channel:** Chrome Web Store, r/sysadmin Loom/Atlassian threads, a Loom-renewal calculator.
- **Go/no-go condition:** proceed only if web checks show that no $0–30 tool already combines free occasional recorders, video-to-SOP and a flat team price. Otherwise drop it.

**Not shortlisted, with reasons (judgment):**
- A04, A01 and A02 are components (engines inside B07 and B04).
- L03: the BFCM 2026 window is missed and the bundle is a parity problem. Revisit with a single "no order-volume tiers" reviews/loyalty migration app before Sept 2027.
- B01, B02, A05, L01, L02, B03, B05: crowded categories or parity problems.
- B06, L05, L06: structural kills (telecom, enterprise buyer, vault liability).

**Sequencing suggestion (judgment):** Start B07 now so it ships by ~Nov 21, inside the off-season. Start B04 in parallel only if the founder accepts the SMS/10DLC work. Otherwise do B04 second, in Jan 2027, while heating season continues, then add A03 as its module. Choose between A06 and B07 rather than doing both, because both demand migration concierge work in the same Nov–Jan window.

**Claims that most need fresh web verification (by shortlist item)**
- **B07:**
  - HoneyBook's current prices and fees ($29/$49/$109 yearly; $59/$129 monthly; card fees from 2.7% + 10¢; ACH 1.5%), and whether any new hike or plan change came after Sep 24.
  - Whether the 20% loyalty discount really expired Feb 4 2026 (the only source is the competitor Talleflow).
  - What HoneyBook lets users export (clients, projects, contract PDFs), because that decides how feasible the importer is.
  - 2026 prices and features of Dubsado, 17hats, Bonsai, Studio Ninja, Sprout Studio, Táve and Plutio, plus any **cheap indie HoneyBook alternatives the corpus missed** (search "HoneyBook alternative" listicles and r/WeddingPhotography threads from 2026).
  - Stripe Connect Standard onboarding friction and Stripe ACH pricing (the corpus marks this "background knowledge; verify").
  - The size and self-promotion rules of the top wedding-photographer Facebook groups.
  - WPPI 2027 dates.
  - Whether the Nov–Feb off-season claim actually holds (it is unsourced in the corpus).
- **B04:**
  - Angi's current contract terms (35% ETF, 60-day auto-renew notice), because the source, LeadTruffle, is itself a competitor.
  - The current Google LSA credit and dispute process as of Oct 2026.
  - The LSA $53/lead benchmark.
  - Competitor density for "missed call text back" and "speed to lead" tools and their prices, including LeadTruffle's own price, GHL snapshot resellers, and **whether Jobber and Housecall Pro now bundle AI text-back or receptionists** (judgment: this is likely, and the corpus does not cover it).
  - Twilio/Telnyx ISV 10DLC brand and campaign fees and vetting times in Oct 2026.
  - Whether Angi and Thumbtack lead emails or APIs can be parsed or forwarded under their terms.
  - The Vermont AG settlement (Oct 2025, "not re-checked").
- **A06:**
  - Kajabi's current prices and whether annual subscribers on pre-Jan-13 pricing really keep renewing into the hike through Jan 2027.
  - Kajabi's export capabilities: video download, member CSV, and Kajabi Payments subscription portability.
  - The single "$179 to retrieve client data" Trustpilot claim.
  - Current prices for Thinkific, Teachable, Podia, Skool, Mighty and Circle, plus **cheaper course hosts the corpus missed**. Note that Ruzuku, the main Kajabi-hike source, is itself a course platform (judgment).
  - How many live Kajabi sites can be found through mykajabi.com subdomains or BuiltWith.
- **A03:**
  - Podium and Birdeye prices and terms (third-party sources: Astucia, Contractor ToolStack).
  - NiceJob's price ("not re-verified").
  - Prices of cheap review-request tools.
  - The approval process and timeline for GBP API access.
  - The text and applicability of WI §134.49 and NY GOL §5-903.
  - How many sites show detectable Podium or Birdeye widgets (BuiltWith counts).
- **L04:**
  - Loom's current pricing and when Creator Lite auto-promotion happens for annual customers.
  - The primary source for the $240 → $24,000 anecdote (an unverified Hacker News post).
  - Prices of Cap.so, Tella, Scribe and Tango, and **whether any video-to-guide tool (for example Guidde-class products, judgment, not in the corpus) already offers free contributors and flat pricing**.
  - Whether Loom still allows bulk MP4 export.

### Gaps
- None of the wedges has been tested with buyers. Build-time estimates of 4–6 weeks are judgment for a Claude-assisted solo developer and assume Stripe, Twilio/Telnyx and Mux/Bunny as managed providers.
- The corpus gives no buyer counts reachable through each named channel, such as Facebook group sizes, the number of Kajabi sites, or the number of Podium/Birdeye widget sites. The size of the first-100-customers funnel is therefore unknown.
- Seasonality claims (the wedding off-season as a switching window, and heating season as buying rather than "too busy" season) are asserted in the corpus without sources. I treated them as plausible but unverified.
- Whether the founder is willing to run SMS/10DLC operations decides whether B04 and A03 rank #2 and #4 or drop out. That preference is not known.
