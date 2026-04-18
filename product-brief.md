# Product Brief: CreditStack

**Author:** Alex (Product Manager Agent) | **Date:** 2026-04-18 | **Version:** 1.0
**Status:** Draft — Ready for Engineering + Design Kickoff

---

## 1. Product Overview

**Name:** CreditStack
**Tagline:** *Every IRA bonus credit. Fully documented. Zero surprises at audit.*

**Core Value Proposition:**
CreditStack is the only affordable SaaS platform purpose-built for independent renewable energy developers to maximize, stack, and document IRA tax credits. It tracks prevailing wage compliance, domestic content (BABA), energy community bonuses, low-income qualifiers, and FEOC restrictions across an entire project portfolio — and auto-generates audit-ready reports for IRS submissions and investor due diligence. Developers currently do this in spreadsheets and lose 10–30% of available credit value through missed qualifiers and documentation gaps. CreditStack closes that gap.

---

## 2. The Opportunity: Why This, Why Now

### Problem Evidence
- **1,400 GW of renewable projects** are active in US interconnection queues. Every project starting before July 2026 must navigate IRA bonus credit stacking rules simultaneously.
- IRA bonus credits add **10–30% incremental value per project** (prevailing wage, domestic content, energy community, low-income, FEOC). Getting all five right can mean $10–30M+ in additional tax equity on a 50 MW solar project.
- No pure-play SaaS solution exists below **$100k/yr enterprise tier** (Enverus, KPMG advisory). Developers earning $5–20M/project are managing this in Excel.
- 45Q carbon capture credit begins inflation indexing in **2026**, unlocking new project economics and compliance requirements.
- OBBBA is rewriting some IRA provisions in 2025–2026 — every time rules change, developers scramble. There is no system of record.

### Why This Opportunity Scores Highest (9.5/10)
| Dimension | Assessment |
|-----------|-----------|
| TAM | $800M+ addressable software layer (5,000+ US developers) |
| Feasibility | High — knowledge/data product, no hardware dependency |
| Defensibility | Medium — regulatory update moat; proprietary outcome database |
| Speed to Revenue | Fast — transactional model ($500–2k/project) enables immediate sales |
| Competitive Gap | No affordable solution; only enterprise ($100k+) or consultants ($300/hr) |

---

## 3. Ideal Customer Profile (ICP)

### Primary ICP: Independent Solar/Wind Developer (SMB-Mid)
| Attribute | Description |
|-----------|------------|
| **Company size** | 10–200 employees; $5M–$100M annual revenue |
| **Project pipeline** | 1–50 MW individual projects; 5–200 MW total active portfolio |
| **Geography** | US-based; projects across ERCOT, CAISO, PJM, MISO, SPP |
| **Deal trigger** | New project start or financing round requiring tax equity documentation |
| **Budget authority** | VP Finance, CFO, or Director of Project Finance |
| **Current tools** | Excel, Google Sheets, QuickBooks, some Procore for construction |
| **Willingness to pay** | $15–60k/yr platform; $500–2k per project transactional |
| **Pain statement** | "We're leaving credits on the table and our tax equity investor wants audit-ready docs we can't produce without 80 hours of manual work." |

### Secondary ICP: Tax Equity Investors & Law Firms
| Attribute | Description |
|-----------|------------|
| **Segment** | Banks, family offices, and law firms doing IRA tax credit due diligence |
| **Use case** | Verify developer compliance claims before committing capital |
| **Value prop** | Standardized audit trail reduces DD cycle from 6 weeks to 1 |
| **WTP** | $5–15k per deal review; or enterprise seat license |

### Personas

**"Project Finance Paul"** — VP Finance, 45-person solar developer in Texas
- Manages 8–12 active projects; 3 in tax equity negotiations at any time
- Spends 15 hrs/project manually verifying prevailing wage payroll records
- Has missed domestic content bonus twice due to incomplete supplier documentation
- Primary buyer; signs software contracts under $50k without board approval

**"Deal Counsel Dana"** — Associate at renewable energy law firm in DC
- Reviews IRA compliance for 20+ developer clients annually
- Currently builds custom checklists for each client from scratch
- Wants a platform clients can self-serve so she can focus on interpretation, not data collection
- Key influencer; recommends tools to developer clients

---

## 4. Feature List with Priorities

### P0 — MVP (Must ship at launch; without these, no product)

| # | Feature | User Story | Success Criteria |
|---|---------|------------|-----------------|
| P0-1 | **Credit Eligibility Analyzer** | As Paul, I want to input a project's location, technology type, and procurement data so I know which bonus credits I qualify for and the estimated dollar value | System correctly identifies all applicable bonus categories for 95%+ of standard US solar/wind/storage projects |
| P0-2 | **Prevailing Wage Tracker** | As Paul, I want to upload weekly certified payroll records and have the system flag non-compliant pay rates by trade classification and county | Detects wage non-compliance before it becomes an IRS penalty; exports corrective action report |
| P0-3 | **Domestic Content (BABA) Calculator** | As Paul, I want to enter my equipment procurement list (manufacturer, component, COO) and get a BABA percentage score vs. the 40/45/55% thresholds | Accurate BABA % calculation with confidence rating; flags borderline components for manual review |
| P0-4 | **Audit-Ready Report Generator** | As Paul, I want to generate a PDF/Excel package containing all credit documentation formatted for IRS Form 3800 and tax equity investor due diligence | Report passes review by at least 3 pilot tax equity investors without requiring supplemental requests |
| P0-5 | **Project Dashboard** | As Paul, I want a single view of all active projects showing credit status, compliance gaps, and deadline alerts | All P0 features accessible from unified project view; <3 click depth to any critical action |

### P1 — Launch + 60 Days (Ship within first two sprints post-MVP)

| # | Feature | User Story | Notes |
|---|---------|------------|-------|
| P1-1 | **Energy Community Qualifier** | Overlay IRS energy community shapefile on project address to determine 10% bonus credit eligibility | IRS publishes updated energy community maps annually — must stay current |
| P1-2 | **Low-Income Community Bonus Tracker** | Track Section 48E low-income applications (annual program caps; competitive allocation) | Requires DOE allocation data integration |
| P1-3 | **FEOC Compliance Checker** | Flag battery/component manufacturers on the FEOC restriction list (Treasury updates quarterly) | Critical for storage projects post-2024 |
| P1-4 | **IRA Rule Change Alerts** | Push notifications and changelog when IRS/Treasury guidance updates affect active project calculations | Becomes primary retention hook; regulatory volatility makes this essential |
| P1-5 | **Multi-Project Portfolio View** | Aggregate credit exposure, compliance risk scores, and revenue at risk across all active projects | Needed for developers with 5+ concurrent projects |

### P2 — Quarter 2 (Roadmap; do not commit engineering resources yet)

| # | Feature | Description | Unlock Condition |
|---|---------|------------|-----------------|
| P2-1 | **Tax Equity Investor Portal** | Shareable, read-only project room for investors to review compliance docs without email chains | Validate with 3 investor design partners post-MVP |
| P2-2 | **Prevailing Wage Payroll API Integration** | Direct integration with ADP, Gusto, and certified payroll processors to auto-ingest payroll data | 5+ customers requesting it; reduces friction from manual upload |
| P2-3 | **45Q Carbon Capture Credit Module** | Extend platform to 45Q credit documentation (inflation indexing begins 2026) | Tax equity market signal; Q3 2026 |
| P2-4 | **Interconnection Queue Integration** | Layer FERC/ISO queue status onto project records for holistic project health view | Potential bridge to second product line (see Opportunity #3 in research) |
| P2-5 | **AI Credit Optimization Assistant** | Natural language Q&A on "How do I improve my BABA score?" or "What's the fastest path to prevailing wage compliance?" | Needs sufficient usage data to train context; post-500 projects analyzed |

---

## 5. Pricing Model

### Philosophy
Land transactionally (low friction, immediate value). Expand to platform subscription (portfolio volume + retention hooks). Create upgrade lever when portfolio grows.

### Tiers

| Tier | Price | Includes | Target Buyer |
|------|-------|----------|-------------|
| **Analyze** (transactional) | $750/project | One-time credit analysis + report; no ongoing monitoring | First-time buyer; project-by-project developer |
| **Developer** (annual) | $18,000/yr | Up to 10 active projects; all P0+P1 features; IRA alert service | SMB developer (1–10 active projects) |
| **Portfolio** (annual) | $42,000/yr | Up to 40 active projects; multi-project dashboard; investor portal (P2-1 early access); API access | Mid-size developer / IPP (10–40 projects) |
| **Enterprise** (annual) | Custom ($60k–$150k/yr) | Unlimited projects; dedicated CSM; custom reporting; SSO; audit support | Large IPPs, tax equity investors, law firms |

### Revenue Model Assumptions (Year 1 Targets)
- Target: 30 Analyze customers → convert 40% to Developer = 12 platform subs
- 12 Developer × $18k = $216k ARR
- 5 Portfolio × $42k = $210k ARR
- 2 Enterprise × $80k = $160k ARR
- **Year 1 ARR Target: $586k** (conservative; assumes 6-month sales cycle for Enterprise)

---

## 6. User Journey & Key Workflows

### Primary Workflow: New Project Onboarding → Credit Report

```
1. PROJECT SETUP (5 min)
   Developer enters: project name, address, technology type, 
   capacity (MW), COD target, financing structure
   → System auto-identifies applicable bonus credit categories
   → Generates compliance checklist with deadlines

2. PREVAILING WAGE SETUP (30 min, one-time)
   Upload initial contract for construction trades
   Enter county/MSA for each work location
   System pulls current Davis-Bacon wage determinations from DOL API
   → Generates pay rate floor alerts per trade classification

3. DOMESTIC CONTENT INPUT (2 hrs, ongoing)
   Enter equipment list: inverters, racking, modules, cables
   Tag each by manufacturer + country of origin
   System calculates running BABA % vs. required threshold
   → Flags borderline components; suggests substitution scenarios

4. BONUS CREDIT VALIDATION (automated)
   Energy community: auto-geocoded from IRS shapefile
   Low-income: pull application status from DOE portal
   FEOC: component manufacturer cross-checked against Treasury list
   → Real-time eligibility dashboard

5. REPORT GENERATION (10 min)
   Select report type: IRS Form 3800 package / Investor DD package / Internal summary
   System assembles documentation from all inputs
   PDF export with audit trail timestamps
   → Share link or download

6. ONGOING MONITORING
   Weekly payroll upload (or API pull, P1)
   IRA rule change alerts pushed to developer
   → Re-run compliance check when rules update
```

### Secondary Workflow: Tax Equity Investor Due Diligence

```
1. Developer shares project room link (P2-1 Investor Portal)
2. Investor reviews: credit eligibility summary, prevailing wage records, 
   BABA calculation, FEOC attestations
3. Investor marks items as "Verified" or requests documentation
4. System generates sign-off log with timestamps
→ Replaces 40+ email threads and 2–6 week DD cycles
```

---

## 7. Competitive Differentiation: Why We Win

| Dimension | Enverus / Enterprise ($100k+) | Consultants ($300/hr) | CreditStack |
|-----------|------------------------------|----------------------|-------------|
| **Price** | $100k+/yr | $20–80k/project | $750–$42k |
| **Self-serve** | No; requires implementation | No; requires engagement | Yes; onboard in <1 day |
| **IRA-specific focus** | Broad energy analytics | Generic tax advisory | Purpose-built for IRA stacking |
| **Speed to first report** | 3–6 month implementation | 4–8 weeks | Same day |
| **Ongoing rule updates** | Manual; consultant re-engagement | Billable hourly | Included in subscription |
| **Audit trail** | Limited | PDF binder, manual | Automated, timestamped, investor-ready |

**Three reasons we win:**
1. **Affordability unlocks a market.** 5,000+ SMB developers have no option today. We're not taking share from Enverus — we're creating a new segment.
2. **Speed is money.** Tax equity deals have hard close dates. A same-day credit analysis vs. a 6-week consulting engagement directly impacts deal velocity and financing cost.
3. **Regulatory volatility is our moat.** Every time IRA rules change (and they will), customers who manage this in Excel restart from scratch. CreditStack absorbs that complexity and updates automatically.

---

## 8. Success Metrics

### North Star Metric
**Projects analyzed per month** — captures both new customer acquisition and existing customer usage. A developer who brings new projects to the platform is retained, expanding, and getting value.

**Current baseline:** 0 (pre-launch)
**Target (Month 6):** 50 projects/month
**Target (Month 12):** 200 projects/month

### Supporting Metrics

| Metric | Baseline | 60-Day Target | 90-Day Target |
|--------|---------|--------------|--------------|
| MRR | $0 | $15k | $45k |
| Analyze → Developer conversion | — | 35% | 40% |
| Time to first report (new customer) | — | <4 hrs | <2 hrs |
| Report accepted by tax equity investor without revision | — | ≥80% | ≥90% |
| Monthly active projects per Developer customer | — | ≥4 | ≥6 |
| Net Revenue Retention (NRR) | — | — | ≥110% |
| Customer-reported credit value unlocked | — | $5M+ | $20M+ |

### Launch Success Gate
By 90 days post-GA:
- [ ] 10+ paying customers
- [ ] At least 3 projects where CreditStack-generated report was accepted by a tax equity investor
- [ ] 0 P0 bugs in production
- [ ] NPS ≥ 40 from active users

---

## 9. Key Risks & Mitigations

| Risk | Likelihood | Impact | Mitigation |
|------|------------|--------|-----------|
| IRA policy rollback (OBBBA rewriting provisions) | High | High | Build rule engine as configurable logic, not hardcoded; position as "navigate whatever rules are current" |
| Enterprise competition moves downstream | Medium | High | Speed to market; developer community trust; data moat from early customer outcomes |
| Tax equity investors don't trust automated reports | Medium | High | Partner with 2–3 established law firms as validation co-brands; run closed beta with investor design partners |
| DOL/IRS API availability for wage data | Low | Medium | Cache wage determination data locally; manual upload fallback |
| Sales cycle longer than projected | Medium | Medium | Transactional Analyze tier creates fast first revenue; low-friction land |

---

## 10. What We Are Not Building (v1)

| Out of Scope | Reason | Revisit Condition |
|-------------|--------|-----------------|
| Interconnection queue intelligence | Different buyer workflow; dilutes MVP focus | Q3 2026 if IRA product hits $500k ARR |
| BESS dispatch optimization | High technical complexity; different ICP | Year 2 if market signal warrants |
| EU CSRD / Scope 3 reporting | Different regulatory regime; US-first thesis | International expansion trigger |
| Carbon credit issuance/trading | Adjacent but unrelated workflow; regulatory complexity | Post-Series A |
| Permitting workflow automation | Different buyer (BD team vs. finance team) | Roadmap exploration Q4 2026 |
| Native mobile app | Core user is desktop-based (finance/compliance role) | Only if mobile usage data warrants |

---

## 11. Next Steps

| Action | Owner | Deadline | Notes |
|--------|-------|----------|-------|
| Recruit 5 developer design partners for closed beta | PM | May 2, 2026 | Target SEIA member directory + LinkedIn |
| DOL Davis-Bacon API access request | Engineering | Apr 25, 2026 | Government portal; may take 2–3 weeks |
| IRS energy community shapefile integration spike | Engineering | Apr 30, 2026 | Public data; validate accuracy vs. IRS tool |
| Design kickoff: project setup + credit analyzer flow | Design | May 5, 2026 | Use problem brief above; no solution handed to design |
| Tax equity investor partner outreach (3 targets) | PM | May 9, 2026 | Needed to validate report format before dev |
| Legal review: IRS Form 3800 output representation | Legal/Counsel | May 16, 2026 | Ensure we don't inadvertently constitute tax advice |

---

*CreditStack. Every IRA bonus credit. Fully documented. Zero surprises at audit.*
