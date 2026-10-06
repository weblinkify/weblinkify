# Daniyal Tariq

### AI-Native Full-Stack Engineer · AI Systems · Cloud · Automation

I build **production-oriented AI and full-stack systems** that connect intelligent software with real-world applications.

My work spans **AI engineering, modern web development, Python APIs, agentic systems, cloud infrastructure, and developer automation** — from designing LLM-powered workflows to building the APIs, interfaces, data pipelines, containers, CI/CD, and cloud infrastructure that make them usable in production.

I care about systems that are:

**Typed · Modular · Testable · Observable · Secure · Deployable · Built to Evolve**

---

## What I Build

### 🤖 AI-Native Applications

I build applications where AI is part of the system architecture rather than simply a chatbot feature.

* LLM-powered applications
* Agentic AI workflows
* RAG pipelines
* Structured LLM outputs
* Tool calling
* MCP integrations
* Prompt orchestration
* AI evaluation
* Human-in-the-loop workflows
* AI safety and validation

### ⚡ Full-Stack Systems

I work across the application stack, connecting modern interfaces with reliable backend services.

* React
* Next.js
* TypeScript
* Python
* FastAPI
* GraphQL
* REST APIs
* PostgreSQL
* Redis
* Pydantic
* Async Python

### ☁️ Cloud & Platform Engineering

I design applications with deployment and operations in mind from the beginning.

* Microsoft Azure
* Azure OpenAI
* Azure AI Search
* Container Apps / AKS
* Docker
* Azure Container Registry
* Azure Key Vault
* Infrastructure as Code
* GitHub Actions
* CI/CD

### 🔧 Engineering Automation

I automate the repetitive parts of software delivery.

```text
Code
 ↓
Lint
 ↓
Type Check
 ↓
Test
 ↓
Security Scan
 ↓
Build
 ↓
Containerize
 ↓
Deploy
 ↓
Monitor
```

---

# Featured Work

## 🛰️ Telco AI Operations Assistant

### Enterprise Agentic AI Platform for Telecommunications

A production-oriented enterprise AI platform demonstrating how **Generative AI, Agentic AI, RAG, MCP, and cloud infrastructure** can work together in a telecommunications environment.

The system is designed around multiple specialised AI agents capable of investigating customers, incidents, network events, enterprise documentation, and controlled operational actions.

### Architecture

```text
                         ┌─────────────────┐
                         │   Enterprise UI │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │    FastAPI      │
                         └────────┬────────┘
                                  │
                                  ▼
                         ┌─────────────────┐
                         │ Supervisor Agent│
                         └────────┬────────┘
                                  │
              ┌───────────────────┼───────────────────┐
              ▼                   ▼                   ▼
       Knowledge Agent     Customer Agent      Incident Agent
              │                   │                   │
              ▼                   └─────────┬─────────┘
             RAG                            │
              │                             ▼
              ▼                         MCP Server
       Azure AI Search                     │
              │               ┌─────────────┼─────────────┐
              ▼               ▼             ▼             ▼
        Azure OpenAI     Customer      Incident      Network
                         Systems       Systems       Systems
```

### Engineering Focus

* **LangGraph** multi-agent orchestration
* **Model Context Protocol (MCP)**
* Retrieval-Augmented Generation
* Azure OpenAI
* Structured tool calling
* Human approval workflows
* RBAC and authorization
* Prompt injection protection
* Audit logging
* AI evaluation
* OpenTelemetry
* Docker
* GitHub Actions
* Azure deployment architecture

### Example Workflow

```text
User
 ↓
Supervisor
 ↓
Customer Agent
 ↓
MCP
 ↓
Enterprise Services
 ↓
Knowledge / RAG
 ↓
LLM
 ↓
Validated Response
```

For sensitive actions:

```text
AI Recommendation
       ↓
Validation
       ↓
Authorization
       ↓
Human Approval
       ↓
Enterprise Action
       ↓
Audit Trail
```

The goal is not simply to build an AI chatbot.

The goal is to demonstrate how an AI engineer can **design, secure, evaluate, deploy, and operate an enterprise AI system.**

---

## ⚡ Nexora AI

### AI-Native Full-Stack Application Platform

A production-oriented full-stack AI platform combining modern web development, Python services, LLM integrations, containers, automation, and cloud infrastructure.

**Stack**

```text
Next.js
React
TypeScript
     │
     ▼
GraphQL / REST
     │
     ▼
FastAPI
     │
     ▼
AI Services
     │
     ▼
LLM Provider
     │
     ▼
Azure
```

### Engineering Focus

* Modern TypeScript frontend architecture
* FastAPI backend services
* GraphQL / REST APIs
* LLM integrations
* Structured validation
* Async APIs
* Dockerized services
* CI/CD automation
* Cloud deployment
* Production-oriented architecture

🔗 **[Live Demo](https://nexora-ai-native.netlify.app/)**
🔗 **[Repository](https://github.com/weblinkify/ai-fullstack-platform)**

---

# 🌍 FieldIQ

### Connected Environmental Monitoring Platform

FieldIQ explores the intersection of **software, IoT, cloud data, and AI**.

The platform is designed around:

```text
Sensors
   ↓
Device
   ↓
Connectivity
   ↓
API
   ↓
Database
   ↓
Dashboard
   ↓
Analytics
   ↓
AI Insights
```

The current MVP uses simulated sensor data while establishing the foundation for future hardware integration.

### Current Direction

* Next.js
* React
* TypeScript
* Tailwind CSS
* Monitoring dashboards
* Simulated sensor data
* Sites and devices
* Alerts
* Data visualization

### Future Architecture

```text
Environmental Sensors
        ↓
      ESP32
        ↓
 Wi-Fi / Cellular
        ↓
    FieldIQ API
        ↓
   Data Platform
        ↓
   PostgreSQL
        ↓
 Monitoring Platform
        ↓
 Analytics + AI
```

The longer-term goal is to explore how **physical-world data can become actionable intelligence through software and AI.**

🔗 **[Live Demo](https://field-iq-theta.vercel.app/)**

---

# My Engineering Approach

## AI Is a System, Not a Feature

I don't treat an LLM as an isolated API call.

A reliable AI application needs:

```text
Model
 +
Context
 +
Tools
 +
Validation
 +
Security
 +
Evaluation
 +
Observability
 +
Human Oversight
```

The model is only one component of the system.

---

## Types Are Contracts

I prefer explicit interfaces and validation boundaries.

```text
User Input
   ↓
Schema Validation
   ↓
Business Logic
   ↓
Tool / Service
   ↓
Validated Output
   ↓
Application
```

Typed systems make applications easier to understand, test, refactor, and operate.

---

## Agents Need Boundaries

AI agents should not have unrestricted access to application infrastructure.

Instead:

```text
Agent
  ↓
Tool
  ↓
Authorization
  ↓
Enterprise Service
```

This creates clear boundaries between **AI reasoning and system execution**.

---

## Retrieved Data Is Untrusted

RAG systems must distinguish between:

```text
System Instructions
        ≠
Retrieved Content
```

Documents can contain incorrect, malicious, or instruction-like content.

AI systems therefore need explicit controls around:

* Prompt boundaries
* Tool permissions
* Output validation
* Context handling
* Prompt injection
* Source attribution

---

## Production Thinking Starts Early

I think about more than whether an application works locally.

Important questions include:

* What happens when the model fails?
* What happens when a tool times out?
* Can the request be retried safely?
* How is the action authorized?
* How is the result audited?
* How much does the request cost?
* Can we observe the workflow?
* Can the system scale?
* Can another engineer understand the architecture?

---

# Technical Stack

### Languages

`TypeScript` · `Python` · `SQL`

### Frontend

`React` · `Next.js` · `HTML` · `CSS` · `Tailwind CSS`

### Backend

`FastAPI` · `GraphQL` · `REST` · `Pydantic` · `SQLAlchemy` · `AsyncIO`

### AI Engineering

`Azure OpenAI` · `LangGraph` · `LangChain` · `MCP` · `RAG` · `Embeddings` · `Vector Search` · `Tool Calling` · `Structured Outputs`

### Data

`PostgreSQL` · `Redis` · `pgvector` · `Azure AI Search`

### Cloud

`Microsoft Azure` · `Azure Container Apps` · `AKS` · `Azure Container Registry` · `Azure Key Vault`

### DevOps

`Docker` · `Docker Compose` · `GitHub Actions` · `CI/CD` · `Terraform` · `Bicep`

### Observability

`OpenTelemetry` · `Azure Monitor` · `Application Insights`

### Quality

`Pytest` · `Ruff` · `Mypy` · `TypeScript` · `Integration Testing` · `AI Evaluation`

---

# System Design

I enjoy working at the intersection of application engineering and AI infrastructure.

A typical system I design looks like:

```text
                    ┌──────────────┐
                    │   Frontend   │
                    │ Next.js/React│
                    └──────┬───────┘
                           │
                           ▼
                    ┌──────────────┐
                    │ API Gateway  │
                    │ REST/GraphQL │
                    └──────┬───────┘
                           │
                           ▼
                 ┌────────────────────┐
                 │ Application Layer  │
                 └─────────┬──────────┘
                           │
              ┌────────────┼────────────┐
              ▼            ▼            ▼
           Agents         RAG         Tools
              │            │            │
              └────────────┼────────────┘
                           ▼
                     LLM Provider
                           │
                           ▼
                  Validation / Policy
                           │
                           ▼
                 Enterprise Services
                           │
                           ▼
                 Database / Cache / APIs
```

Around the system:

```text
Security
Observability
Testing
Evaluation
CI/CD
Infrastructure
```

---

# Currently Exploring

I'm currently focused on:

* 🤖 Agentic AI architecture
* 🧠 LLM-powered developer tools
* 🔎 Production RAG systems
* 🔌 Model Context Protocol
* 🕸️ Multi-agent workflows
* ⚡ TypeScript + Python full-stack systems
* ☁️ Azure AI infrastructure
* 🐳 Containerized applications
* 🔄 CI/CD automation
* 📊 AI evaluation and observability
* 🔐 Secure AI application design
* 🌐 AI + IoT systems

---

# What I Want to Build

I'm particularly interested in systems where **AI interacts with real software, data, and infrastructure**.

```text
AI
 +
Software
 +
Data
 +
Cloud
 +
Automation
 =
Intelligent Systems
```

The interesting engineering problems are not only about making models generate better answers.

They're about making AI systems:

**Reliable. Secure. Observable. Testable. Cost-aware. Governable. Useful.**

---

# GitHub

I use GitHub as my engineering workspace for:

* Building
* Experimenting
* Testing
* Documenting
* Automating
* Deploying
* Learning
* Iterating

### `@weblinkify`

Building at the intersection of:

**AI × Full Stack × Cloud × Automation**

---

## Let's Build

I'm interested in collaborating on **AI-native products, developer tools, intelligent automation, enterprise AI systems, and cloud-native applications.**

If you're building something where **AI needs to work like software — not just look like a demo — I'd love to explore it.**

📫 **[LinkedIn](https://www.linkedin.com/in/daniyaltariq09/)**
💻 **[GitHub](https://github.com/weblinkify)**
