<div align="center">

# Hi, I'm Daniyal Tariq 👋

### Senior AI-Native Full-Stack Engineer · 🎓 Google Cloud Certified Professional Cloud Developer · AI agents, RAG & LLM apps · Python · TypeScript

7+ years building production web apps, APIs and AI systems

**LLMs · AI agents · RAG · MCP · LangGraph · Evals · Python · FastAPI · TypeScript · React · Angular · Next.js · Google Cloud · Azure**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/daniyaltariq09/)
[![Google Cloud Certified](https://img.shields.io/badge/Google%20Cloud%20Certified-Professional%20Cloud%20Developer-4285F4?logo=googlecloud&logoColor=white)](https://www.linkedin.com/in/daniyaltariq09/details/certifications/)
[![Live demo](https://img.shields.io/badge/Featured-Telco%20AI%20Ops%20(live)-8B5CF6)](https://telco-ai-ops.vercel.app)
[![Live demo](https://img.shields.io/badge/AI%20co--pilot-RiskPilot%20(live)-22c55e)](https://riskpilot-field-iq1.vercel.app)
[![Portfolio](https://img.shields.io/badge/AI%20projects-6%20built-6366f1)](#-featured-ai-work)

</div>

---

I build **AI systems that do real work inside real products**: multi-agent assistants that use your tools, RAG that answers from your documents **with citations**, AI co-pilots that explain their reasoning, and document extraction that only asks a human about the fields it is unsure of.

Demos are easy. Production AI is not. So every AI system I ship comes with **evals that run in CI, human approval for risky actions, guardrails against prompt injection, audit logs and a mock LLM mode**, so you can measure it, trust it and run it without API keys. Underneath sits a full-stack foundation of typed code, tests, Docker and CI/CD.

## 🤖 How I can help you

| Service | What you get |
| --- | --- |
| 🧠 **AI agents & tool calling** | Multi-agent workflows (LangGraph) that call your systems through **MCP** tools or APIs, with human-in-the-loop approval, RBAC per tool and full audit logs |
| 📚 **RAG over your documents** | Hybrid search (BM25 + pgvector / Azure AI Search), answers grounded in your docs with citations, PII masking before the LLM |
| 🧾 **Document AI & extraction** | Invoices, forms and submissions turned into structured data with confidence scores, review of only the uncertain fields, and export to your ERP |
| ✨ **AI features in your product** | Chat, streaming replies, AI assistants and co-pilots added to existing web or mobile apps, with a pluggable provider (Anthropic Claude, OpenAI, Azure OpenAI) |
| 📏 **Evals, safety & governance** | Golden eval suites (routing, retrieval, faithfulness, tool use, injection attacks) gated in CI, grounding guards, prompt-injection defences, AI risk registers and policies |
| 🧩 **Full-stack & cloud foundation** | FastAPI, Spring Boot or Node backends; React, Angular or Next.js front ends; PostgreSQL, Docker, GitHub Actions, Azure, Vercel; React Native mobile |

---

## 🛡️ How I build AI you can trust

- **Grounded, not guessed:** answers and scores cite the exact document and field they came from.
- **Humans make the call:** the AI proposes; risky actions run only after an authorised person approves, enforced in code (not in a prompt).
- **Measured on every change:** golden eval sets run in CI and block regressions, just like unit tests.
- **Secure by design:** prompt-injection quarantine, PII masking, least-privilege tools, rate limits and append-only audit logs.
- **Runs without API keys:** a deterministic mock LLM keeps demos, tests and CI free, fast and reproducible.
- **No vendor lock-in:** switching between Claude, OpenAI and Azure OpenAI is a one-line config change.

---

## ⭐ Featured AI work

### 🛰️ Telco AI Operations Assistant: enterprise multi-agent AI *(agentic AI)*

<a href="https://telco-ai-ops.vercel.app"><img src="https://raw.githubusercontent.com/weblinkify/llm-agent-platform/HEAD/docs/media/demo.gif" alt="Telco AI Ops: the AI proposes an incident, the graph pauses, an admin approves, then the MCP tools execute" width="720" /></a>

A multi-agent assistant for telecom support and NOC teams. A **LangGraph supervisor** routes work to knowledge, customer, incident and action agents. They answer from runbooks and SLAs with citations (**hybrid RAG**: BM25 + pgvector) and reach enterprise systems through **12 MCP tools**. The AI can *propose* creating incidents or paging teams, but **writes run only after a different authorised human approves**.

- **Agents:** LangGraph supervisor + 4 specialist agents, `interrupt()` / resume for human approval, streaming replies over SSE
- **Safety:** JWT + 4 RBAC roles enforced per MCP tool, prompt-injection quarantine (tested with a poisoned document), PII masking before the LLM, output guard, full audit log
- **Evals:** 48-case golden suite gated in CI: 100% routing, 95.8% retrieval recall@4, 100% tool-call correctness, 100% injection block rate
- **Ops:** FastAPI, Next.js console, Postgres, OpenTelemetry traces, Docker + Terraform for Azure Container Apps; Azure OpenAI, OpenAI or Anthropic

**[▶ Live demo](https://telco-ai-ops.vercel.app)** (mock mode, no sign-up) · **[Code](https://github.com/weblinkify/llm-agent-platform)**

---

### 🛡️ RiskPilot: AI co-pilot for insurance underwriters *(explainable AI)*

[![RiskPilot: submission workbench with AI risk assessment and cited evidence](https://raw.githubusercontent.com/weblinkify/riskpilot/main/docs/screenshot-submission.png)](https://riskpilot-field-iq1.vercel.app)

An underwriting workbench for commercial property insurance. RiskPilot triages broker submissions, scores each risk 0–100 with **explainable signals that cite the exact document and field they came from**, checks the carrier's appetite rules and suggests a next step (Quote, Refer, Request info, Decline). **The underwriter always makes the call:** overrides need a written reason, and every decision goes to an append-only audit log.

- **AI:** pluggable provider (deterministic mock or **Claude** with grounding guards), cited evidence for every signal
- **Frontend:** Angular 22 (standalone components, signals), Apollo GraphQL with generated types, dashboard KPIs and charts
- **Backend:** Java 21 + Spring Boot 3, GraphQL + REST/OpenAPI, PostgreSQL + Flyway
- **Quality:** a golden-file test proves the Java and TypeScript scorers match on all 40 submissions; unit, Testcontainers and Playwright tests in CI

**[▶ Live demo](https://riskpilot-field-iq1.vercel.app)** · **[Code](https://github.com/weblinkify/riskpilot)**

---

### 🧾 InvoiceLens: AI invoice extraction with a human in the loop *(document AI)*

<img src="https://raw.githubusercontent.com/weblinkify/Invoice-lens/HEAD/docs/screenshots/demo.gif" alt="InvoiceLens: loading an invoice, fixing a low-confidence field and approving it" width="720" />

Upload PDFs or scans, and the AI extracts vendor, dates, VAT IDs, IBANs, line items and totals with a **confidence score per field**. You **only review the low-confidence fields**, then export or push clean data to your ERP via signed webhooks.

Python · FastAPI · React · LLM extraction · ~97% / 96% test coverage · runs fully without API keys (mock LLM) · **[Code](https://github.com/weblinkify/Invoice-lens)**

---

### 🏥 CareSlot: healthcare booking built by a governed AI coding agent *(AI-assisted engineering)*

<a href="https://careslot-demo.vercel.app"><img src="https://raw.githubusercontent.com/weblinkify/care-slot/main/docs/images/demo.gif" alt="CareSlot: a patient booking an appointment" width="720" /></a>

GDPR-grade appointment booking where the organisation can prove **who accessed which patient's data, when and why**. Built with an **AI coding agent under a written AI development policy and AI risk register**, held to the same CI gates as human code: mypy strict, module boundaries, 117 backend tests, contract tests, Playwright + axe WCAG 2.2 AA, SBOM and Trivy scans.

React + TypeScript · Python + FastAPI · PostgreSQL 16 · AES-256-GCM envelope encryption · hash-chained audit log · **[▶ Live demo](https://careslot-demo.vercel.app)** · **[Code](https://github.com/weblinkify/care-slot)**

---

### ⚡ More AI projects

| Project | What it is | Stack | Links |
| --- | --- | --- | --- |
| **Nexora AI** | AI-native full-stack platform: ask questions, get LLM answers through a typed API | Next.js · TypeScript · GraphQL/REST · FastAPI · LLM services | [Live](https://nexora-ai-native.netlify.app/) · [Code](https://github.com/weblinkify/ai-fullstack-platform) |
| **Pocket Chat** | ChatGPT-style iOS app with token-by-token streaming and a mock LLM for key-free CI | React Native (Expo) · FastAPI · SSE · E2E iOS tests | [Code](https://github.com/weblinkify/pocket-chat) |
| **BookFlow AI** | Appointment booking SaaS for service businesses, with an AI assistant | React · TypeScript · Tailwind | [Live](https://bookflowui.netlify.app/) · [Code](https://github.com/weblinkify/bookflow) |

### 🧩 Full-stack foundations

The products my AI features plug into:

| Project | What it is | Stack | Links |
| --- | --- | --- | --- |
| **FieldIQ Map** | 4,000 IoT sensors on a WebGL map with area statistics, heatmap and CSV export | Angular 22 · MapLibre · Spring Boot · PostGIS · GraphQL | [Live](https://fieldiq-web-rosy.vercel.app/map) · [Code](https://github.com/weblinkify/field-iq-map) |
| **InvoiceFlow** | Invoicing & billing SaaS for freelancers and agencies | React · TypeScript · Tailwind | [Live](https://invoiceflowui.netlify.app/) · [Code](https://github.com/weblinkify/invoice-flow) |
| **InventoryFlow** | Inventory & stock management SaaS | React · TypeScript · Tailwind | [Live](https://inventoryflowui.netlify.app/) · [Code](https://github.com/weblinkify/inventory-flow) |
| **ProjectFlow** | Kanban project management SaaS | React · TypeScript · Tailwind | [Live](https://projectflowui.netlify.app/) · [Code](https://github.com/weblinkify/project-management-flow) |
| **SaaS Subscription** | Plans, billing and settings dashboard | React · TypeScript · Tailwind | [Live](https://saasflowui.netlify.app/) · [Code](https://github.com/weblinkify/SaaS-subscription-flow) |
| **FieldIQ (v1)** | IoT monitoring dashboard MVP | Next.js · React · TypeScript | [Live](https://field-iq-theta.vercel.app/) · [Code](https://github.com/weblinkify/fieldIQ) |
| **From Click to Code** | A real todo app with a built-in 23-lesson course on how the web works | JavaScript · Node · CI | [Code](https://github.com/weblinkify/from-click-to-code) |

---

## 🤝 How I deliver an AI project

1. **Understand:** a short call to pin down the task the AI should do, who uses it and what "good" looks like.
2. **Define success first:** a small golden set of real examples, so quality is measured, not guessed.
3. **Prototype fast:** a clickable demo on your data, with a mock LLM so it runs anywhere.
4. **Harden:** guardrails, human approval for risky actions, RBAC, audit logs and evals in CI.
5. **Deploy:** live on Google Cloud, Azure, Vercel or your servers, with Docker, tracing and cost-aware model choice.
6. **Hand-over:** a clear README, eval report, architecture notes and walkthrough, so your team owns it.

Clear, regular communication throughout. I'd rather show progress than promise it.

---

## 🛠️ Tech stack

**AI & LLMs**
![Anthropic Claude](https://img.shields.io/badge/Anthropic%20Claude-D97757?logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI%20%2F%20Azure%20OpenAI-0078D4?logo=openai&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?logo=langchain&logoColor=white)
![MCP](https://img.shields.io/badge/MCP-F97316)
![RAG](https://img.shields.io/badge/RAG%20%C2%B7%20Agents%20%C2%B7%20Tool%20calling-8B5CF6)
![pgvector](https://img.shields.io/badge/pgvector-336791?logo=postgresql&logoColor=white)
![Azure AI Search](https://img.shields.io/badge/Azure%20AI%20Search-0078D4?logo=microsoftazure&logoColor=white)
![Evals](https://img.shields.io/badge/Evals%20in%20CI-10B981)
![OpenTelemetry](https://img.shields.io/badge/OpenTelemetry-425CC7?logo=opentelemetry&logoColor=white)

**Backend & APIs**
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?logo=graphql&logoColor=white)
![REST](https://img.shields.io/badge/REST%20%2F%20OpenAPI-6BA539?logo=openapiinitiative&logoColor=white)

**Frontend & Mobile**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?logo=angular&logoColor=white)
![React Native](https://img.shields.io/badge/React%20Native-20232A?logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white)
![MapLibre](https://img.shields.io/badge/MapLibre%20%2F%20Mapbox-396CB2?logo=maplibre&logoColor=white)

**Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL%20%2B%20PostGIS-4169E1?logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white)

**DevOps & Cloud**
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Google Cloud](https://img.shields.io/badge/Google%20Cloud%20(certified)-4285F4?logo=googlecloud&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-844FBA?logo=terraform&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?logo=netlify&logoColor=white)

**Testing**
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?logo=vitest&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?logo=pytest&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit%205%20%2B%20Testcontainers-25A162?logo=junit5&logoColor=white)

---

## 🧭 What you can expect from my code

- **Runs on day one:** `docker compose up` or one `make` command, with a mock LLM so no secrets are needed for a demo.
- **AI quality you can see:** an eval suite and results report next to the unit, integration and end-to-end tests, all in CI.
- **Typed & documented:** strict TypeScript, typed Python, generated API types, architecture decisions and READMEs with screenshots.
- **Secure by default:** environment-based configuration, input validation, least-privilege tools and containers, no personal data in logs.
- **Built to change:** small modules, clear contracts and a swappable model provider, so new features (and new models) don't break old ones.

---

<div align="center">

### 📬 Let's build something intelligent

Want an AI agent, a RAG assistant over your documents, or AI features added to an existing product?
**Message me on Upwork or [LinkedIn](https://www.linkedin.com/in/daniyaltariq09/)**. Happy to start with a short call.

</div>
