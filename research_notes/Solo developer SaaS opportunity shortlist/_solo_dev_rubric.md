# Solo-developer screening rubric

**Founder profile:** one developer who builds and ships with Claude as the team. No sales staff, no outside capital, no compliance team. Goal: recurring revenue from US small-business (or prosumer) buyers as fast as possible. Today is October 2026.

The corpus (`SaaS-Opportunity-Research`) scored ideas for "replace a bloated incumbent". This rubric re-scores them for "one person can build it, sell it and support it".

## Criteria (score each 1–5, 5 = best for a solo developer)

| # | Criterion | 5 means | 1 means |
|---|---|---|---|
| 1 | **Solo build scope** | A sellable MVP that customers would switch to ships in 6 weeks or less: CRUD, forms, documents, notifications, simple integrations | Needs broad feature parity before anyone switches (POS, EHR, PMS, payroll, accounting, field-service suite), hardware, offline mobile apps, or many deep integrations |
| 2 | **Regulatory and liability burden** | None beyond normal SaaS terms | HIPAA/PHI, PCI scope beyond Stripe Checkout, money transmission, SOC 2 required to sell, or the product gives legal/tax determinations where an error costs the customer real money |
| 3 | **Self-serve sale** | Owner-operator or individual decides alone, pays by card, converts from a free trial without a demo, onboards in under an hour | Committees, RFPs, procurement, multi-month cycles, or mandatory demos and data migration services |
| 4 | **Solo-reachable distribution** | Buyers cluster in places one person can reach: an app marketplace (Shopify, Chrome, WordPress, Zapier, QuickBooks), large subreddits/Facebook groups, "X alternative" search intent, public lists for cold email | Buyers are only reachable through field sales, paid ads at high CPC, or channel partners |
| 5 | **Willingness to pay and ARPU** | $49+/month per customer is credible; $10k MRR needs 200 or fewer customers | Under $15/month, or buyers expect free |
| 6 | **Gap versus cheap indie tools** | No good $0–30 tool already does the wedge; incumbents are expensive or hated | Already crowded with cheap, good indie tools (e.g., Tally for forms, Cal.com for scheduling) |
| 7 | **Urgency in the next 6 months** | A dated switching window between Oct 2026 and Apr 2027 (price hike, sunset, forced migration, law deadline, season) | No trigger; buyers can wait forever |
| 8 | **Support load and retention** | Low-touch support; data accumulates so customers stay; not seasonal one-shot | Heavy support (telephony, payments disputes, migrations), seasonal churn, one-time use |

**Total: /40.**

## Kill flags (list any that apply; two or more usually rules an idea out for a solo founder)

- Requires HIPAA/PHI handling
- Core value depends on payment processing or holding funds
- Core value depends on telephony/SMS carrier registration (A2P 10DLC) at scale
- Hardware or offline-first mobile app required
- Buyer is enterprise, government or a committee
- Must encode 50-state legal rules where a wrong answer creates customer liability
- Feature-parity monster (customer won't switch until most of the incumbent's features exist)
- Market is crowded with cheap indie tools

## Wedge rule

For every promising idea, define the **narrowest sellable wedge**: the smallest product a solo developer could ship in 4–6 weeks that a specific buyer would pay for on its own (for example, "a CoConstruct-to-X importer plus client portal" rather than "full construction PM").
