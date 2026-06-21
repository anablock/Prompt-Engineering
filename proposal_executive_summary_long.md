# ANABLOCK DIGITAL SOLUTIONS
## Executive Summary — Annual Services Proposal
### Prepared for: Dr. My G. Tran, DDS
### Streamline Dental Solutions | The Forever Smile | Sterolux Sterilizers

**Prepared by:** Anablock (anablock.com)
**Date:** June 21, 2026
**Proposal Valid Through:** July 21, 2026
**Contract Term:** 12 Months (July 1, 2026 – June 30, 2027)

---

## WHO WE ARE

Anablock is Dr. Tran's embedded digital team. We are not a vendor — we are an extension of his organization. Since the early stages of Streamline Dental Solutions' growth, Anablock has designed, developed, and managed the digital infrastructure across all four of Dr. Tran's brands. We built the websites, manage the code, run the campaigns, and are now building the AI agents that will automate his operations.

We operate on one principle: **Your Success is Our Success.**

---

## WHAT WE MANAGE TODAY

| Brand | Domain | What Anablock Manages |
|---|---|---|
| Streamline Dental Solutions | silverstatesmiles.com | Website, SEO, PPC, CRM, lead gen, email, content |
| The Forever Smile | aforeversmiles.com | Website, SEO, PPC, creative, video, email, e-commerce build |
| Sterolux Sterilizers | steroluxsterilizer.com | Website, SEO, e-commerce, PPC (pending FDA) |
| Sterolux Shop | shop.steroluxsterilizer.com | E-commerce platform, product management |

**GitHub Repositories Actively Managed:**
- `anablock/streamline-dental-main`
- `anablock/sterolux-ecommerce`
- `anablock/sterolux-studio`
- `anablock/forever-smile`

---

## WHAT THIS PROPOSAL COVERS

This Annual Services Agreement formalizes the full scope of Anablock's engagement across all brands for the 12-month period July 1, 2026 – June 30, 2027. It covers 13 service modules, two AI agent builds, a Salesforce data migration, a CareStack API integration, and a full e-commerce platform build for The Forever Smile.

---

## SERVICES AT A GLANCE

| Module | Service | Type |
|---|---|---|
| 1 | Website Management & Development + pSEO + AEO + SEO Metadata (all 4 sites) | Monthly |
| 2 | Email Marketing (all brands) | Monthly |
| 3 | Blog & Content Generation (all brands) | Monthly |
| 4 | E-Commerce Website Management (Sterolux + Forever Smile shop) | Monthly |
| 5 | AI Agent for Lead Generation (Streamline + Forever Smile) | Monthly |
| 6 | Video Editing (Forever Smile + Streamline) | Monthly |
| 7 | AI Payroll Agent — QuickBooks + ADP MCP Server | Monthly |
| 8 | AI Contract & Timesheet Agent — MCP Server (Basecamp + ADP + QuickBooks + DocuSign) | Monthly |
| 8B | Salesforce → Anablock CRM Patient Lead Migration | One-Time |
| 8C | Anablock CRM ↔ CareStack API Bidirectional Integration | Monthly |
| 9 | PPC Campaign Management — Google Ads + Meta Ads (per cost center) | Monthly |
| 10 | Anablock CRM — full platform access | Included |
| 11 | System Integration & Technical Operations | Monthly |
| 12 | A Forever Smile Monthly Creative Production (Meta, Google, AI search, e-commerce shop) | Monthly |
| 13 | Deliverables & Reporting (6 monthly reports) | Monthly |

---

## THE AI AGENT STACK

Two custom AI agents are being built and maintained as part of this engagement — both powered by Model Context Protocol (MCP) servers connecting to live APIs.

### AI Payroll Agent (Module 7)
Connects to **QuickBooks Online** and **ADP Workforce Now** via MCP. The agent answers payroll questions, reconciles expenses, flags variances, surfaces time clock corrections, and drafts vendor payment batches — all in plain language, accessible via web chat, Slack, or Google Chat. All write operations require human confirmation.

### AI Contract & Timesheet Agent (Module 8)
Connects to **Basecamp**, **ADP**, **QuickBooks**, **DocuSign/HelloSign**, and **Google Drive** via MCP. The agent manages the full vendor contract lifecycle (repository, expiration alerts, template generation, e-signature), automates timesheet exception reporting, routes approval workflows, and answers labor cost questions by location in real time. All write operations require human confirmation.

---

## SALESFORCE MIGRATION (Module 8B)

All patient lead data from Streamline Dental Solutions' Salesforce instance will be migrated to Anablock CRM in a structured 6-phase process:

| Phase | What Happens |
|---|---|
| 1. Discovery & Audit | Full Salesforce object inventory, field mapping, data quality assessment |
| 2. Extraction | Salesforce Bulk API 2.0 — SOQL queries, up to 15 GB CSV export, External ID mapping |
| 3. Transformation | Phone normalization, pipeline stage mapping, deduplication, HTML stripping, timestamp preservation |
| 4. Migration | Dependency-ordered load — contacts → leads → notes/activity → pipeline stages. 10% test run first. |
| 5. Validation | Record count comparison, 50-record spot audit, duplicate check, pipeline distribution report, sign-off |
| 6. Decommission Support | Salesforce set to read-only for 90-day archive, final migration report delivered |

**Objects migrated:** Leads, Contacts, Accounts, Opportunities, Activities/Tasks, Campaign Membership, all custom dental fields.

---

## CARESTACK INTEGRATION (Module 8C)

A bidirectional, real-time integration between Anablock CRM and CareStack (developer.carestack.com) using CareStack's REST API and webhooks.

**Anablock CRM becomes the single source of truth for patient leads and relationships. CareStack remains the system of record for clinical operations, scheduling, and billing.**

### CareStack → Anablock CRM (7 automated flows)

| CareStack Event | Anablock CRM Action |
|---|---|
| New patient created | Auto-create/update contact with demographics + insurance. Assign pipeline stage. |
| Appointment scheduled | Log note. Auto-advance LEAD/QUALIFIED_LEAD to NURTURING. |
| Appointment completed | Update last contacted date. Trigger post-visit follow-up sequence. |
| Appointment cancelled/no-show | Log event. Trigger re-engagement sequence after 48 hours. |
| Treatment plan created/updated | Log plan summary (type, estimated value, status) on contact. |
| Payment received | Update payment note. Trigger thank-you/review request sequence. |
| Patient communication sent | Log communication event on contact timeline. |

### Anablock CRM → CareStack (3 automated flows)

| Anablock CRM Event | CareStack Action |
|---|---|
| Lead advanced to CUSTOMER | Auto-create patient record in CareStack — no front desk re-entry required. |
| Contact info updated | Push update to CareStack patient record. |
| Communication opt-in/out changed | Sync patient communication preferences in CareStack. |

---

## THE FOREVER SMILE E-COMMERCE BUILD

Two stores built on the same headless Shopify + Next.js + Vercel architecture as the Sterolux Shop.

### Store 1 — B2C Patient Shop (aforeversmiles.com/shop)

Luxury patient-facing storefront for dental implant treatment packages, post-care products, oral health supplements, educational courses, and subscriptions. Includes CareCredit/Sunbit financing, Anablock CRM sync, and SEO-optimized product pages.

| Phase | Hours | Cost |
|---|---|---|
| Discovery & Architecture | 20 | $1,100 |
| UI/UX Design | 40 | $2,200 |
| Frontend Development | 80 | $4,400 |
| Shopify Backend | 30 | $1,650 |
| Integrations (CRM, booking, financing) | 25 | $1,375 |
| Content & SEO | 20 | $1,100 |
| QA, Testing & Launch | 15 | $825 |
| Training & Handoff | 10 | $550 |
| **TOTAL** | **240 hrs** | **$13,200** |

### Store 2 — B2B Practitioner Portal (partners.aforeversmiles.com)

Gated wholesale and licensing portal for licensed dental practitioners. Includes NPI verification, tiered pricing, DocuSign licensing agreements, co-branded marketing asset downloads, CE tracking, and Anablock CRM B2B pipeline integration.

| Phase | Hours | Cost |
|---|---|---|
| Discovery & B2B Architecture | 25 | $1,375 |
| UI/UX Design | 35 | $1,925 |
| Frontend Development | 70 | $3,850 |
| Shopify B2B Backend | 35 | $1,925 |
| Integrations (NPI, DocuSign, CRM, referral tracking) | 30 | $1,650 |
| Content & Catalog | 20 | $1,100 |
| QA, Testing & Launch | 15 | $825 |
| Training & Handoff | 10 | $550 |
| **TOTAL** | **240 hrs** | **$13,200** |

### E-Commerce Build Timeline

| Milestone | Target Date |
|---|---|
| Project kickoff & discovery | Week 1 — July 7, 2026 |
| Design approval | Week 3 — July 21, 2026 |
| B2C store development complete | Week 7 — August 18, 2026 |
| B2C store launch | Week 8 — August 25, 2026 |
| B2B portal development complete | Week 11 — September 15, 2026 |
| B2B portal launch | Week 12 — September 22, 2026 |

---

## COMPLETE COST BREAKDOWN

### Cost Center 1 — Streamline Dental Solutions

#### Monthly Flat Fee (All Services)

| What's Included | Monthly | Annual |
|---|---|---|
| Website management & dev across all 4 brands (Module 1) | | |
| pSEO + AEO + Traditional SEO across all 4 websites (Module 1) | | |
| Email marketing — all brands (Module 2) | | |
| Blog & content generation — all brands (Module 3) | | |
| E-commerce management — Sterolux + Forever Smile (Module 4) | | |
| AI lead generation agent — Streamline + Forever Smile (Module 5) | | |
| Video editing — Forever Smile + Streamline (Module 6) | | |
| AI Payroll Agent — QuickBooks + ADP MCP Server build + maintenance (Module 7) | | |
| AI Contract & Timesheet Agent — MCP Server build + maintenance (Module 8) | | |
| Salesforce → Anablock CRM migration (Module 8B) | | |
| CareStack API bidirectional integration build + maintenance (Module 8C) | | |
| System integrations & technical ops (Module 11) | | |
| Anablock CRM — full platform (Module 10) | | |
| A Forever Smile monthly creative production — Meta, Google, AI search, e-commerce (Module 12) | | |
| All custom dev & ad-hoc work — no per-asset billing, no overages | | |
| **MONTHLY FLAT FEE** | **$5,500** | **$66,000** |

#### PPC Campaign Management — Streamline Dental / Forever Smile

| Account | Platforms | Monthly | Annual |
|---|---|---|---|
| silverstatesmiles.com + aforeversmiles.com | Google Ads + Meta Ads | $2,500 | $30,000 |

> Ad spend paid directly by client to Google and Meta. Not included in management fee.

#### Streamline Dental Solutions Total

| | Monthly | Annual |
|---|---|---|
| All-Inclusive Flat Fee | $5,500 | $66,000 |
| PPC Management — Streamline / Forever Smile | $2,500 | $30,000 |
| Anablock CRM | Included | Included |
| **STREAMLINE DENTAL TOTAL** | **$8,000** | **$96,000** |

---

### Cost Center 2 — Sterolux Sterilizers *(Pending FDA Approval)*

| | Monthly | Annual |
|---|---|---|
| PPC Management — Sterolux (Google + Meta, B2B dental targeting) | $2,500 | $30,000 |
| All creative, dev & landing page work | Included | Included |
| **STEROLUX TOTAL** | **$2,500** | **$30,000** |

> Sterolux PPC activates upon FDA approval. Billed to Sterolux Sterilizers on a separate invoice.

---

### One-Time Projects

| Project | Fixed Fee |
|---|---|
| B2C Patient Shop — aforeversmiles.com/shop | $13,200 |
| B2B Practitioner Portal — partners.aforeversmiles.com | $13,200 |
| Bundle Discount (both stores together) | –$1,650 |
| **TOTAL E-COMMERCE BUILD** | **$24,750** |

#### E-Commerce Milestone Payment Schedule

| Milestone | Amount |
|---|---|
| Contract signing (deposit) | $8,250 (33%) |
| B2C store design approval | $4,125 (16.5%) |
| B2C store launch | $4,125 (16.5%) |
| B2B portal design approval | $4,125 (16.5%) |
| B2B portal launch (final) | $4,125 (16.5%) |
| **Total** | **$24,750** |

---

### Year 1 Total Investment Summary

| Scenario | Monthly | Year 1 Total |
|---|---|---|
| Streamline Dental (flat fee + PPC) | $8,000/mo | $96,000 |
| + Forever Smile E-Commerce Build (one-time) | — | $24,750 |
| **Streamline + E-Commerce (Year 1)** | | **$120,750** |
| + Sterolux PPC (if FDA approved mid-year, ~6 months) | $2,500/mo | ~$15,000 |
| **Full Portfolio — Year 1 (all accounts active)** | | **~$135,750** |

---

### Payment Options — Streamline Dental Solutions

| Option | Structure | Annual Total | Savings |
|---|---|---|---|
| **Option A — Monthly** | $8,000/month | $96,000 | — |
| **Option B — Quarterly** | $23,500/quarter (prepaid) | $94,000 | ~$2,000 (~2%) |
| **Option C — Annual Prepay** | $90,000/year (upfront) | $90,000 | ~$6,000 (~6%) |

---

## WHAT YOU GET FOR $8,000/MONTH

For $8,000/month — $5,500 flat fee + $2,500 PPC management — Streamline Dental Solutions receives:

**Digital Infrastructure**
- Full website management across 4 brand properties
- pSEO at scale — automated location × service pages, treatment × location pages, product × category pages
- AEO — content structured to be cited by ChatGPT, Perplexity, Google AI Overviews, and Bing Copilot
- Traditional SEO — schema markup, Core Web Vitals, sitemaps, canonicals, internal linking

**Marketing & Content**
- Monthly email campaigns across all brands
- SEO blog articles per brand
- Full video editing pipeline (Reels, TikTok, YouTube Shorts, long-form)
- Monthly creative production for The Forever Smile: 6–8 Meta ads, 4–6 Google Display sets, Google PMax refresh, 2–4 AI search ad sets, 1–2 landing pages, 10–15 ad copy variants

**AI Automation**
- AI Payroll Agent (QuickBooks + ADP MCP) — live payroll queries, variance alerts, payment scheduling
- AI Contract & Timesheet Agent (Basecamp + ADP + QuickBooks + DocuSign MCP) — contract lifecycle, timesheet exceptions, approval workflows
- AI Lead Generation Agent — chatbot/agent, CRM integration, Dentina/WhatConverts optimization
- CareStack ↔ Anablock CRM bidirectional integration — 7 inbound flows, 3 outbound flows, full pipeline automation

**Data & Operations**
- Salesforce → Anablock CRM full patient lead migration (6-phase, all objects)
- Anablock CRM — full platform, all dashboards, all integrations
- System integrations & technical ops across all platforms
- PPC campaign management — Google Ads + Meta Ads for Streamline Dental and The Forever Smile

**Reporting**
- 6 monthly reports: SEO/pSEO/AEO, PPC performance, creative production, e-commerce, CRM pipeline, operations
- Weekly sync with Otter.ai notes and action items
- All work tracked in Basecamp and GitHub

**No hourly tracking. No overages. No surprises.**

---

## NEXT STEPS

1. Review this proposal with your team
2. Confirm scope adjustments or additions
3. Select payment option (A, B, or C)
4. Sign the Service Agreement (to be sent separately)
5. Confirm contract start date — proposed: **July 1, 2026**

---

**Questions?**
Vuk Dukic | Anablock
vuk@anablock.com | anablock.com

---

*This proposal is confidential and prepared exclusively for Dr. My G. Tran, Streamline Dental Solutions, The Forever Smile, and Sterolux Sterilizers. All pricing is valid through July 21, 2026.*
