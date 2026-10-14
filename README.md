<div align="center">

# Hi, I'm Daniyal Tariq 👋

### Full-Stack & AI Engineer: I build production-ready web apps, APIs and AI systems

**TypeScript · Angular · React · Next.js · Python · FastAPI · Java · Spring Boot · PostgreSQL · Docker · Azure**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/daniyaltariq09/)
[![Live demo](https://img.shields.io/badge/Featured-RiskPilot%20(live)-22c55e)](https://riskpilot-field-iq1.vercel.app)
[![Portfolio](https://img.shields.io/badge/Live%20demos-9%20projects-6366f1)](#-featured-work)

</div>

---

I turn product ideas into **working software you can click, test and deploy**: dashboards, SaaS platforms, map/data applications, mobile apps and AI features (LLMs, RAG, agents) built into real products.

Every project I deliver comes with **clean typed code, automated tests, CI/CD, Docker and clear documentation**, so your team can run it, change it and trust it after hand-over.

## 💼 How I can help you

| Service | What you get |
| --- | --- |
| 🧩 **Full-stack web apps & SaaS** | Admin dashboards, booking, invoicing, inventory and subscription platforms. Angular, React or Next.js front ends with REST/GraphQL APIs |
| 🗺️ **Maps & data visualisation** | Interactive maps with thousands of points (Mapbox / MapLibre, PostGIS), filters, area selection, live stats and CSV export |
| 🤖 **AI features & automation** | LLM integrations, RAG over your documents, AI agents with tool calling, document extraction with human review |
| ⚙️ **APIs & backends** | FastAPI, Spring Boot or Node: PostgreSQL, auth, validation, OpenAPI docs and integration tests |
| 🚀 **DevOps & deployment** | Docker, GitHub Actions CI/CD, Vercel, Netlify and Azure, with one-command local setup and preview deployments |
| 📱 **Mobile** | React Native (Expo) apps with streaming APIs and end-to-end tests |

---

## ⭐ Featured work

### 🛡️ RiskPilot: AI co-pilot for insurance underwriters *(newest)*

[![RiskPilot: submission workbench with AI risk assessment and cited evidence](https://raw.githubusercontent.com/weblinkify/riskpilot/main/docs/screenshot-submission.png)](https://riskpilot-field-iq1.vercel.app)

An underwriting workbench for commercial property insurance. RiskPilot triages broker submissions, scores each risk 0–100 with **explainable signals that cite the exact document and field they came from**, checks the carrier's appetite rules and suggests a next step (Quote, Refer, Request info, Decline). **The underwriter always makes the call:** overrides need a written reason, and every decision goes to an append-only audit log.

- **Frontend:** Angular 22 (standalone components, signals), Apollo GraphQL with generated types, dashboard KPIs and charts
- **Backend:** Java 21 + Spring Boot 3, GraphQL + REST/OpenAPI, PostgreSQL + Flyway, pluggable AI provider (deterministic mock or Claude LLM with grounding guards)
- **Mock mode:** the real GraphQL schema runs in the browser, so the demo needs **zero setup**. A golden-file test proves the Java and TypeScript scorers match on all 40 submissions
- **Quality:** unit, Testcontainers integration and Playwright end-to-end tests, Docker Compose, GitHub Actions CI

**[▶ Live demo](https://riskpilot-field-iq1.vercel.app)** · **[Code](https://github.com/weblinkify/riskpilot)**

---

### 🗺️ FieldIQ Map: 4,000 IoT sensors on an interactive map

[![FieldIQ Map: bounding-box selection with live area statistics](https://raw.githubusercontent.com/weblinkify/field-iq-map/main/docs/screenshots/bbox-selection.png)](https://fieldiq-web-rosy.vercel.app/map)

An environmental monitoring platform: **4,000 sensors across Finland** on a fast WebGL map with clusters, hover tooltips, sensor details with 24 h charts, **draw-a-box area statistics**, filters, a PM2.5 heatmap and CSV export. Every view is shareable by URL.

- **Frontend:** Angular 22 (signals, strict TypeScript), Tailwind, MapLibre / Mapbox GL behind one engine interface, Apollo GraphQL with generated types
- **Backend:** Java 21 + Spring Boot (REST + GraphQL), PostgreSQL + PostGIS spatial queries, Flyway, real-time reading simulator
- **Mock API:** the same contract in Node/TypeScript, so the demo runs with **zero setup**. Contract tests prove mock and real backends match
- **Quality:** 200+ automated tests: unit, integration (Testcontainers) and Playwright end-to-end in both modes, ~96% backend coverage, Docker Compose, GitHub Actions

**[▶ Live demo](https://fieldiq-web-rosy.vercel.app/map)** · **[Area stats demo](https://fieldiq-web-rosy.vercel.app/map?bbox=24.7,60.12,25.2,60.33)** · **[Code](https://github.com/weblinkify/field-iq-map)**

---

### 🧾 InvoiceLens: AI invoice extraction with a human in the loop

<img src="https://raw.githubusercontent.com/weblinkify/Invoice-lens/HEAD/docs/screenshots/demo.gif" alt="InvoiceLens: loading an invoice, fixing a low-confidence field and approving it" width="720" />

Upload PDFs or scans, and the AI extracts vendor, dates, VAT IDs, IBANs, line items and totals. You **only review the low-confidence fields**, then export or push clean data to your ERP via signed webhooks.
Python · FastAPI · React · LLM extraction · ~97% / 96% test coverage · runs fully without API keys (mock LLM) · **[Code](https://github.com/weblinkify/Invoice-lens)**

---

### 🛰️ Telco AI Operations Assistant: enterprise agentic AI

A multi-agent assistant for telecom operations. A supervisor agent routes work to knowledge, customer and incident agents, which use **RAG** over company documentation and **MCP** tools to reach enterprise systems. Sensitive actions need human approval and are fully audit-logged.
Python · FastAPI · LangGraph · MCP · Azure OpenAI · Azure AI Search · RBAC · OpenTelemetry · Docker · **[Code](https://github.com/weblinkify/llm-agent-platform)**

---

### ⚡ More projects

| Project | What it is | Stack | Links |
| --- | --- | --- | --- |
| **Nexora AI** | AI-native full-stack platform | Next.js · TypeScript · GraphQL/REST · FastAPI · LLM services | [Live](https://nexora-ai-native.netlify.app/) · [Code](https://github.com/weblinkify/ai-fullstack-platform) |
| **Pocket Chat** | ChatGPT-style iOS app with token-by-token streaming | React Native (Expo) · FastAPI · SSE · E2E iOS tests | [Code](https://github.com/weblinkify/pocket-chat) |
| **BookFlow AI** | Appointment booking SaaS for service businesses, with an AI assistant | React · TypeScript · Tailwind | [Live](https://bookflowui.netlify.app/) · [Code](https://github.com/weblinkify/bookflow) |
| **InvoiceFlow** | Invoicing & billing SaaS for freelancers and agencies | React · TypeScript · Tailwind | [Live](https://invoiceflowui.netlify.app/) · [Code](https://github.com/weblinkify/invoice-flow) |
| **InventoryFlow** | Inventory & stock management SaaS | React · TypeScript · Tailwind | [Live](https://inventoryflowui.netlify.app/) · [Code](https://github.com/weblinkify/inventory-flow) |
| **ProjectFlow** | Kanban project management SaaS | React · TypeScript · Tailwind | [Live](https://projectflowui.netlify.app/) · [Code](https://github.com/weblinkify/project-management-flow) |
| **SaaS Subscription** | Plans, billing and settings dashboard | React · TypeScript · Tailwind | [Live](https://saasflowui.netlify.app/) · [Code](https://github.com/weblinkify/SaaS-subscription-flow) |
| **FieldIQ (v1)** | IoT monitoring dashboard MVP | Next.js · React · TypeScript | [Live](https://field-iq-theta.vercel.app/) · [Code](https://github.com/weblinkify/fieldIQ) |
| **From Click to Code** | A real todo app with a built-in 23-lesson course on how the web works | JavaScript · Node · CI | [Code](https://github.com/weblinkify/from-click-to-code) |

---

## 🤝 How I work with clients

1. **Understand:** a short call to pin down the goal, users and must-haves.
2. **Plan:** a written scope with milestones, so you know what you get and when.
3. **Build in milestones:** working demos you can click at every step, not just at the end.
4. **Quality built in:** typed code, automated tests and CI on every change.
5. **Deploy:** live on Vercel, Netlify, Azure or your servers, with Docker for one-command setup.
6. **Hand-over:** a clear README, setup steps and walkthrough, so your team owns the code.

Clear, regular communication throughout. I'd rather show progress than promise it.

---

## 🛠️ Tech stack

**Frontend**
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?logo=typescript&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?logo=angular&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB)
![Next.js](https://img.shields.io/badge/Next.js-000000?logo=nextdotjs&logoColor=white)
![React Native](https://img.shields.io/badge/React%20Native-20232A?logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-06B6D4?logo=tailwindcss&logoColor=white)
![MapLibre](https://img.shields.io/badge/MapLibre%20%2F%20Mapbox-396CB2?logo=maplibre&logoColor=white)

**Backend & APIs**
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?logo=fastapi&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring%20Boot-6DB33F?logo=springboot&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?logo=nodedotjs&logoColor=white)
![GraphQL](https://img.shields.io/badge/GraphQL-E10098?logo=graphql&logoColor=white)
![REST](https://img.shields.io/badge/REST%20%2F%20OpenAPI-6BA539?logo=openapiinitiative&logoColor=white)

**Data**
![PostgreSQL](https://img.shields.io/badge/PostgreSQL%20%2B%20PostGIS-4169E1?logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?logo=redis&logoColor=white)
![pgvector](https://img.shields.io/badge/pgvector-336791?logo=postgresql&logoColor=white)

**AI**
![OpenAI](https://img.shields.io/badge/Azure%20OpenAI-0078D4?logo=openai&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?logo=langchain&logoColor=white)
![RAG](https://img.shields.io/badge/RAG%20%C2%B7%20Agents%20%C2%B7%20MCP-8B5CF6)

**DevOps & Cloud**
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?logo=githubactions&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?logo=microsoftazure&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?logo=vercel&logoColor=white)
![Netlify](https://img.shields.io/badge/Netlify-00C7B7?logo=netlify&logoColor=white)

**Testing**
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?logo=playwright&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?logo=vitest&logoColor=white)
![Pytest](https://img.shields.io/badge/Pytest-0A9EDC?logo=pytest&logoColor=white)
![JUnit](https://img.shields.io/badge/JUnit%205%20%2B%20Testcontainers-25A162?logo=junit5&logoColor=white)

---

## 🧭 What you can expect from my code

- **Runs on day one:** `docker compose up` or one `make` command, with no secrets needed for a demo.
- **Tested:** unit, integration and end-to-end tests that run in CI on every push.
- **Typed & documented:** strict TypeScript, typed Python, generated API types, and READMEs with screenshots.
- **Secure by default:** environment-based configuration, input validation, least-privilege containers.
- **Built to change:** small modules and clear contracts, so new features don't break old ones.

---

<div align="center">

### 📬 Let's build something

Have a product idea, an MVP to ship, or an existing app that needs features, AI or a clean-up?
**Message me on Upwork or [LinkedIn](https://www.linkedin.com/in/daniyaltariq09/)**. Happy to start with a short call.

</div>
