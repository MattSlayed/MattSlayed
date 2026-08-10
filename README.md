# Matthew Koeberg

**Solutions Engineer — AI Engineering & Technical Pre-Sales · Business Analyst · NOVATEK LLC · Johannesburg, South Africa**

I build the integration and run the client conversation. Most of my work sits at the seam where
language models meet institutions — industrial operations, contracts, quality management where the
interesting problem is rarely the model and almost always the plumbing, the process and the
accountability.

I write publicly about that seam, including a three-tier framework for making calibrated claims
about AI experience. Every claim made below points at a repository.

---

## Integration surface

The APIs and protocols I have actually shipped against, and what I did with each.

| Surface | What I built with it |
|---|---|
| **Anthropic Claude API** | Structured extraction against a defined schema; a ~10 KB extraction prompt written as a specification, not a chat prompt |
| **Anthropic Messages API** | Two-pass research agent with streaming responses, feeding a scoring model |
| **Model Context Protocol (MCP)** | A routing layer into Notion — database schemas, CRUD operations, bidirectional task relations |
| **Microsoft Graph API** | Multi-channel mail and document ingestion into a VPS-hosted FastAPI service |
| **Google Cloud Vision API** | Automated defect detection with confidence scoring, inside a human-gated workflow |
| **FastAPI · NestJS · Prisma · Supabase** | The service and persistence layers underneath the above |

Completed Anthropic's *Introduction to Model Context Protocol* (certificate ID `4id3xgeksg6b`). Four authored Claude Code skills ship inside
[d2a-intelligence-web](https://github.com/MattSlayed/d2a-intelligence-web).

---

## Systems built with the Claude API as a core component

Four, one of them running in client operations. Status stated plainly.

### [D2A Target Account Intelligence](https://github.com/MattSlayed/d2a-intelligence-web) — NOVATEK Agentic OS
[Live](https://d2a-intelligence-web.vercel.app) · Next.js · Anthropic Messages API

A demonstration Agentic Operating System. Profiles enterprise accounts, detects buying triggers,
routes to the right executive, and scores pursuit priority using the ABCD method — grounded in
live web research through a **two-pass research agent** with streaming responses.

Ships four authored Claude Code skills (`run-d2a-sweep`, `deploy-to-vercel`, `add-d2a-agent`,
`update-aos-docs`) and an enterprise PRD of 71 requirements with a traceability matrix.

### [Contract Management Platform](https://github.com/MattSlayed/Contracts-Management)
[Live](https://contracts-management-nu.vercel.app) · NestJS · Next.js · Prisma · TypeScript

AI-assisted contract lifecycle management for NEC3/NEC4 engineering contracts. The Claude API
extracts key terms, parties, dates, values and obligations; identifies risk; compares clauses; and
generates executive summaries. Obligation tracking and deadline management on top.

### [Workshop Intelligence System](https://github.com/MattSlayed/WIS)
Next.js · Supabase · Drizzle · Claude 3.5 Sonnet · Google Cloud Vision

An 11-step gated service workflow for **BRIMIS Engineering**, an industrial maintenance contractor
servicing valves and pumps across seven-plus Eskom power stations. Claude converts technician notes
into technical reports; Google Cloud Vision performs defect detection with confidence scoring.

The design point is the gates, not the AI. Step 6 locks repair until the client approves the PO.
Three hard human sign-off points sit between the model and anything that leaves the workshop —
because a defect marked closed while still open does not stay on the page. It travels.

*Deployment is currently offline pending a redeploy.*

### Central Intelligence System — client operations, private
Claude API · MCP · Notion · Python · FastAPI

Turns 50–100 unstructured operational emails a week into schema-validated priorities, action items
and per-station intelligence, via a ~10 KB structured-extraction prompt. An MCP routing layer into
Notion is in build-out. **Running.** Repository private — client operational data.

---

## Business analysis, in code and in documents

### [Fleet Management System](https://github.com/MattSlayed/my-projectFleet-management-app)
[Live](https://my-project-fleet-management-app.vercel.app) · Next.js · Prisma · NextAuth
Requirements elicited from stakeholder interviews, specified, then built: vehicle tracking, driver
assignment, maintenance scheduling, trip reporting with cost and utilisation tracking.

### [BRIMIS Incident Management System](https://github.com/MattSlayed/BRIMIS-Engineering)
Excel · VBA · Python
P1–P4 priority matrix with SLA tracking and visual compliance indicators. VBA forms designed for
artisans on the floor, not analysts at a desk. Dashboard with KPI metrics, category breakdowns and
resolution trends.

### [Market Basket Analysis](https://github.com/MattSlayed/MarketBasketAnalysis)
Python · Pandas · MLxtend · Jupyter
Apriori association rule mining over a simulated 10,000-order retail dataset, identifying
cross-selling opportunities. Delivered with a process model and a business requirements document.

### [Order Fulfilment Performance Analysis](https://github.com/MattSlayed/Order-Fulfillment-Analysis)
Python · Pandas · Jupyter
Fulfilment cycle-time analysis identifying bottlenecks, with on-time-delivery and order-accuracy
KPI tracking and recommendations.

---

## Web

**[NOVATEK website](https://github.com/MattSlayed/novatek-website)** · [live](https://novatek-website.vercel.app) — Vite, React, TypeScript, Tailwind, Framer Motion
**[nexora-solar](https://github.com/MattSlayed/nexora-solar)** · [live](https://nexora-solar-eight.vercel.app) — TypeScript, Vite, with a chatbot module
**[Financial analytics dashboard](https://github.com/MattSlayed/novatek-financial-dashboardv2)** — React, Chart.js; KPI tracking and budget variance analysis
**[koeberg-portfolio](https://github.com/MattSlayed/koeberg-portfolio)** — WordPress BA portfolio, custom SCSS theme, Docker, Vite

---

## What I have not done

The three-tier framework is only worth anything if it cuts both ways, so:

- **No machine-learning models.** I have not trained, tuned or deployed one. Apriori association
  rule mining is data mining, not supervised learning, and I will not stretch it.
- **No NLP pipelines.** The systems above call an API. I have not implemented tokenisation, entity
  extraction or sentiment analysis myself.
- **No predictive analytics or forecasting.** The dashboards report what happened.
- **No RAG, vector databases or embeddings.**
- **No MLOps.** No model monitoring, no A/B testing, no ML pipeline management.

If a role needs those, I am not yet your candidate. If a role needs someone who can sit with
operations people, work out what the system actually has to do, and then build it — that I can
evidence.

---

## Skills

**AI & integration** — Claude API · Anthropic Messages API · Model Context Protocol (MCP) ·
Microsoft Graph API · Google Cloud Vision API · REST API integration · prompt engineering ·
context engineering · agentic workflow design · Claude Code skills authoring · process automation

**Build** — TypeScript · Next.js · React · NestJS · FastAPI · Prisma · Supabase · Tailwind ·
Docker · Python · VBA

**Client-facing delivery** — technical discovery · requirements elicitation and specification ·
proof-of-concept design and build · stakeholder management to executive level · demo and training
delivery · process modelling · risk and gap analysis · BABOK v3

**Data & BI** — Power BI · star-schema modelling · DAX · Power Query M · Python ETL · SQL/SQLite ·
dashboard design

**Standards & methods** — ISO 9001:2015 · NEC3/NEC4 · McKinsey 7S · Scrum

---

## Writing

- **The Honest AI Resume** — a three-tier framework for claiming AI experience, applied to myself first
- **Workshop Intelligence** — a gated, 11-step AI workflow for high-stakes reporting
- **Building a Central Intelligence System with the Claude API and MCP**
- **The Data-Foundation Myth** — why most enterprise AI stalls before it starts

---

## Certifications

Introduction to Model Context Protocol · AI Fluency: Framework & Foundations — **Anthropic**
Agent Skills with Anthropic — **DeepLearning.AI** · AI Agent Security — **Proofpoint**
Databricks Fundamentals Accreditation — **Databricks** · AWS Educate: Cloud 101, Storage, Compute
Career Essentials in Generative AI — **Microsoft & LinkedIn** · Ethics in the Age of Generative AI
Wits Crucible venture programme — **University of the Witwatersrand**

**BBA**, NQF 7 — STADIO Higher Education

---

## What I'm looking for

**Solutions engineering, technical pre-sales, or integration work at an API-first product company.**
The part of the job I want is the part where someone brings a messy environment and a deadline, and
the work is to find out what they actually need, build a proof of concept that proves it, and get
them to a working go-live. I have been doing that as a consultant, one client at a time. I would
rather do it for a product, where the second client gets the benefit of the first.

Remote. Based in South Africa on SAST (UTC+2) — native EMEA overlap, and I work 15:00–21:00 SAST
when US Eastern cover is needed.

---

## Contact

**Email** matthew@novatekllc.co.za · **LinkedIn** [matthew-koeberg-a76760296](https://linkedin.com/in/matthew-koeberg-a76760296)
