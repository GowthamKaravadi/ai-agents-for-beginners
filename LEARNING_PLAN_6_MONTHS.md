# 6-Month AI Agents Learning Journey (Python-First)

> **Job Posting Reference**: This plan was created in the context of an AI Agents engineering role  
> (LinkedIn job posting `4409175383`).  
> LinkedIn pages are often gated and inaccessible in automation environments.  
> **See [Appendix A](#appendix-a--job-description-paste-template) to paste the full JD text and generate a  
> personalized skills → modules → projects mapping.**

---

## Table of Contents

1. [Assumptions](#1-assumptions)
2. [Is 6 Months Enough?](#2-is-6-months-enough)
3. [Course Map (Lessons in This Repo)](#3-course-map-lessons-in-this-repo)
4. [Week-by-Week Curriculum (24 Weeks)](#4-week-by-week-curriculum-24-weeks)
   - [Month 1 — Python & Engineering Foundations](#month-1-weeks-14--python--engineering-foundations)
   - [Month 2 — Backend APIs & Data Layer](#month-2-weeks-58--backend-apis--data-layer)
   - [Month 3 — LLM Fundamentals, Prompt Engineering & Evaluation](#month-3-weeks-912--llm-fundamentals-prompt-engineering--evaluation)
   - [Month 4 — Agent Architecture, RAG & Tooling](#month-4-weeks-1316--agent-architecture-rag--tooling)
   - [Month 5 — Production Readiness & Deployment](#month-5-weeks-1720--production-readiness--deployment)
   - [Month 6 — Capstone Projects & Interview Prep](#month-6-weeks-2124--capstone-projects--interview-prep)
5. [Milestones & Measurable Outputs](#5-milestones--measurable-outputs)
6. [Capstone Project Options](#6-capstone-project-options)
7. [Portfolio Readiness Checklist](#7-portfolio-readiness-checklist)
8. [Appendix A — Job Description Paste Template](#appendix-a--job-description-paste-template)
9. [Appendix B — Skills → Modules → Projects Mapping Table (Generic)](#appendix-b--skills--modules--projects-mapping-table-generic)

---

## 1. Assumptions

### Starting Profile (Adjust as Needed)

| Dimension | Beginner | Intermediate | Advanced |
|-----------|----------|--------------|----------|
| **Python** | Knows syntax; can write scripts | OOP, typing, exceptions, iterators | Package authoring, async, C-extensions |
| **Git / GitHub** | Knows `add`/`commit`/`push` | Branching, PRs, rebasing | CI/CD authoring, release management |
| **LLMs / AI** | Has used ChatGPT | Understands tokens, context windows | Has fine-tuned or deployed an LLM |
| **Cloud** | None | Has deployed a web app | Has designed multi-region cloud systems |

> **This plan targets the Beginner → Intermediate transition**, the most common profile for people starting their AI Agents career journey.  
> If you are already at Intermediate on all dimensions, compress Months 1–2 into 3–4 weeks and spend the saved time on advanced topics (multi-agent system design, MLOps, security).

### Weekly Time Commitment

| Tier | Hours / Week | Pace |
|------|-------------|------|
| 🟢 **Comfortable** | 6 hrs/week | 36 hrs/month; plan may stretch to 8–9 months |
| 🟡 **Recommended** | 10 hrs/week | 40 hrs/month; plan fits in 6 months |
| 🔴 **Accelerated** | 15 hrs/week | 60 hrs/month; could finish in 4–5 months |

> All time estimates in this document assume **10 hrs/week (Recommended tier)**.  
> At 6 hrs/week, multiply every week-count by ≈ 1.5 × to find your adjusted timeline.

---

## 2. Is 6 Months Enough?

### Short Answer

| Role Level | 6 Months Enough? | Condition |
|------------|-----------------|-----------|
| **Junior / Entry AI Engineer** | ✅ Yes | 10–15 hrs/week + 2 solid projects |
| **Mid-Level AI / ML Engineer** | ⚠️ Borderline | Requires prior software engineering experience; strong capstone projects are mandatory |
| **Senior AI / ML Engineer** | ❌ Unlikely | Typically requires 9–12 months minimum, plus prior production engineering experience |

### Detailed Reasoning

**Why 6 months CAN be enough (Junior/Mid):**
- Modern AI agent frameworks (Microsoft Agent Framework, LangChain, AutoGen) abstract away the most complex infrastructure.
- The concepts in this repository (Lessons 01–15) cover the full lifecycle — from agent fundamentals to production deployment.
- Hiring bar for junior AI roles in 2025–2026 emphasises **working projects + engineering habits** over deep academic knowledge.
- The [AI Agents for Beginners](https://github.com/microsoft/ai-agents-for-beginners) course is structured so that a motivated learner can complete all 15 lessons in ~8–10 weeks of focused study, leaving the remaining time for building and polishing projects.

**Why 6 months may NOT be enough (Senior):**
- Senior roles typically expect **production incidents handled**, **architecture owned end-to-end**, and **team mentorship**.
- Deep knowledge of distributed systems, model evaluation at scale, and MLOps pipelines takes accumulated project experience — not just study.
- If the JD asks for "5+ years" or "staff engineer" equivalents, plan for 9–12 months and prioritise building production-level, deployable projects.

**Weekly hours breakdown to reach job-ready in 6 months:**

```
Month 1 (Weeks 1–4):   Python + tooling foundations      ≈ 40 hrs
Month 2 (Weeks 5–8):   Backend APIs + data layer         ≈ 40 hrs
Month 3 (Weeks 9–12):  LLM + prompt eng + eval           ≈ 40 hrs
Month 4 (Weeks 13–16): Agent architecture + RAG + tools  ≈ 40 hrs
Month 5 (Weeks 17–20): Production + deployment           ≈ 40 hrs
Month 6 (Weeks 21–24): Capstone projects + interview     ≈ 40 hrs
                                                 Total: ~240 hrs
```

At **10 hrs/week × 24 weeks = 240 hrs** — this is realistic and achievable.

---

## 3. Course Map (Lessons in This Repo)

Use this as a quick reference throughout the plan. Each lesson folder contains a `README.md` and Jupyter notebooks under `code_samples/`.

| Lesson | Topic | Month to Study |
|--------|-------|----------------|
| [00 — Course Setup](./00-course-setup/README.md) | Environment setup, Azure credentials | Month 1 |
| [01 — Intro to AI Agents](./01-intro-to-ai-agents/README.md) | Agent types, components, when to use agents | Month 3 |
| [02 — Agentic Frameworks](./02-explore-agentic-frameworks/README.md) | MAF, AutoGen, LangChain, Semantic Kernel | Month 3 |
| [03 — Agentic Design Principles](./03-agentic-design-patterns/README.md) | UX dimensions: Space, Time, Core | Month 4 |
| [04 — Tool Use Pattern](./04-tool-use/README.md) | Function calling, schema definition, execution loop | Month 4 |
| [05 — Agentic RAG](./05-agentic-rag/README.md) | Iterative retrieval, self-correction, multi-source | Month 4 |
| [06 — Trustworthy AI Agents](./06-building-trustworthy-agents/README.md) | Safety, responsible AI, prompt injection | Month 4 |
| [07 — Planning Design](./07-planning-design/README.md) | Task decomposition, iterative re-planning | Month 4 |
| [08 — Multi-Agent Systems](./08-multi-agent/README.md) | Coordination patterns, handoff, group chat | Month 5 |
| [09 — Metacognition](./09-metacognition/README.md) | Self-reflection, Reflexion, self-critique | Month 5 |
| [10 — Agents in Production](./10-ai-agents-production/README.md) | Observability, evaluation, cost management | Month 5 |
| [11 — Agentic Protocols](./11-agentic-protocols/README.md) | MCP, A2A, NLWeb — standardised communication | Month 5 |
| [12 — Context Engineering](./12-context-engineering/README.md) | Prompt engineering, context window management | Month 3 |
| [13 — Agent Memory](./13-agent-memory/README.md) | Short-term, long-term, episodic, semantic memory | Month 4 |
| [14 — Microsoft Agent Framework](./14-microsoft-agent-framework/README.md) | MAF deep-dive: middleware, workflows, observability | Month 4 |
| [15 — Browser Use Agents](./15-browser-use/README.md) | Autonomous web browsing and interaction | Month 6 |

---

## 4. Week-by-Week Curriculum (24 Weeks)

---

### Month 1 (Weeks 1–4) — Python & Engineering Foundations

**Goal**: Build a clean, professional Python development environment and habits.  
**Why first**: Every AI agent is code first. Bad engineering habits (no tests, no types, no CI) will cost you in every subsequent month.

---

#### Week 1 — Python Deep Dive

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | OOP: classes, inheritance, `__dunder__` methods, `dataclasses` | 2 hr |
| 3 | Type hints, `mypy`, annotating functions and data structures | 1.5 hr |
| 4 | Exception hierarchy: custom exceptions, `try/except/finally`, `contextlib` | 1 hr |
| 5–6 | Iterators, generators (`yield`), `itertools`, `functools` | 2 hr |
| 7 | Review: build a small typed CLI utility (e.g., a file organiser) | 1.5 hr |

**Resources:**
- [Python Docs — Classes](https://docs.python.org/3/tutorial/classes.html)
- [Real Python — Type Checking](https://realpython.com/python-type-checking/)
- [Fluent Python (book)](https://www.oreilly.com/library/view/fluent-python-2nd/9781492056348/) — Chapters 1–4

---

#### Week 2 — Testing & Code Quality

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | `pytest`: fixtures, parametrise, `tmp_path`, `monkeypatch` | 2 hr |
| 3 | Mocking: `unittest.mock`, `pytest-mock`, when to mock LLM calls | 1.5 hr |
| 4 | Coverage: `pytest-cov`, reading reports, avoiding coverage-gaming | 1 hr |
| 5 | `ruff` (linting + formatting), `pre-commit` hooks, `.editorconfig` | 1 hr |
| 6–7 | Refactor Week 1 utility: add tests, types, linting, CI via GitHub Actions | 2 hr |

**Deliverable**: A GitHub repository with a tested, typed Python package passing CI.

---

#### Week 3 — Python Packaging & Async

| Day | Activity | Time |
|-----|----------|------|
| 1 | `pyproject.toml`, `setuptools` / `hatch`, packaging best practices | 1.5 hr |
| 2–3 | `async`/`await` fundamentals: event loop, `asyncio.gather`, `asyncio.Queue` | 2 hr |
| 4 | `httpx` async HTTP client, connection pooling, retries | 1 hr |
| 5–6 | `pydantic` v2: models, validators, serialisation, settings management | 2 hr |
| 7 | Build an async data-fetching CLI tool with typed Pydantic models | 1.5 hr |

---

#### Week 4 — Git Workflows & Environment Setup

| Day | Activity | Time |
|-----|----------|------|
| 1 | Git branching strategies: `main`/`dev`/feature branches, PRs, code review | 1.5 hr |
| 2 | GitHub Actions basics: YAML syntax, jobs, steps, environment variables | 1.5 hr |
| 3 | Environment management: `python-dotenv`, secrets management, `.env.example` | 1 hr |
| 4 | Docker basics: `Dockerfile`, `docker-compose`, `.dockerignore` | 1.5 hr |
| 5 | [Lesson 00](./00-course-setup/README.md): Complete course environment setup (Azure, Python venv) | 1 hr |
| 6–7 | Polish Month 1 project; write a short `ARCHITECTURE.md` explaining it | 1.5 hr |

**Month 1 Deliverable**: A clean Python package on GitHub with tests, type hints, linting, CI/CD, and Docker support.

---

### Month 2 (Weeks 5–8) — Backend APIs & Data Layer

**Goal**: Build a production-quality REST API service — the backbone of any AI agent product.  
**Why now**: Before adding LLMs, learn how to build and test robust services. Agents are products; products need APIs, databases, and auth.

---

#### Week 5 — FastAPI Fundamentals

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | FastAPI basics: routes, request/response models (Pydantic), status codes | 2 hr |
| 3 | Dependency injection, middleware, CORS, error handlers | 1.5 hr |
| 4 | Authentication: API keys, JWT basics (no deep security yet) | 1.5 hr |
| 5–6 | Background tasks, `asyncio` in FastAPI, `lifespan` events | 2 hr |
| 7 | Build: "Task Runner API" — submit tasks, get status, retrieve results | 1 hr |

---

#### Week 6 — Databases & ORM

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | PostgreSQL basics: tables, indexes, JOINs, transactions | 2 hr |
| 3–4 | SQLAlchemy 2.x: async sessions, ORM models, Alembic migrations | 2 hr |
| 5 | Redis basics: key-value store, caching patterns, TTL | 1.5 hr |
| 6–7 | Add persistence to Task Runner API: store tasks + results in Postgres | 2 hr |

---

#### Week 7 — API Robustness & Testing

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | Integration testing with `httpx.AsyncClient` and `pytest-asyncio` | 2 hr |
| 3 | Retry patterns: `tenacity`, exponential backoff, circuit breakers | 1.5 hr |
| 4 | Structured logging: `structlog` or `loguru`, JSON logs, correlation IDs | 1.5 hr |
| 5–6 | OpenAPI docs, versioning (`/v1/`, `/v2/`), pagination patterns | 2 hr |
| 7 | Rate limiting, request validation, basic input sanitisation | 1 hr |

---

#### Week 8 — API Deployment & Docker

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | Multi-stage Docker build for FastAPI + Postgres (docker-compose) | 2 hr |
| 3 | GitHub Actions: build image, run tests, push to GHCR | 1.5 hr |
| 4 | Health checks, readiness probes, graceful shutdown | 1 hr |
| 5–7 | Complete "Agent Service API" — CRUD for agents, run history, status | 3 hr |

**Month 2 Deliverable**: A deployed (Docker + GH Actions) "Agent Service API" with Postgres, auth, retries, structured logging, and 80%+ test coverage.

---

### Month 3 (Weeks 9–12) — LLM Fundamentals, Prompt Engineering & Evaluation

**Goal**: Understand LLMs deeply enough to use them reliably; build evaluation infrastructure from day one.  
**Why now**: Agents are LLM-powered. This month turns you from "API caller" to "LLM engineer".

---

#### Week 9 — LLM APIs & Concepts

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | [Lesson 01](./01-intro-to-ai-agents/README.md): AI Agent fundamentals; agent types, components | 2 hr |
| 3 | LLM API concepts: tokens, context windows, temperature, top-p, stop sequences | 1.5 hr |
| 4 | OpenAI / Azure OpenAI SDK: completions, streaming, retry handling | 1.5 hr |
| 5 | Rate limits, cost estimation, model selection (GPT-4o vs GPT-4o-mini) | 1 hr |
| 6–7 | [Lesson 02](./02-explore-agentic-frameworks/README.md): Agentic frameworks overview (MAF, LangChain, AutoGen, Semantic Kernel) | 2 hr |

---

#### Week 10 — Prompt Engineering

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | Prompt patterns: zero-shot, few-shot, chain-of-thought, tree-of-thought | 2 hr |
| 3 | [Lesson 12](./12-context-engineering/README.md): Context engineering and context window management | 1.5 hr |
| 4 | JSON output mode, function calling basics, structured outputs | 1.5 hr |
| 5 | System prompt design: persona, constraints, output format, guardrails | 1.5 hr |
| 6–7 | Build: "Prompt Library" — a reusable set of tested prompt templates for your projects | 1.5 hr |

---

#### Week 11 — Evaluation Framework

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | Why evals matter: regression, golden test sets, LLM-as-judge concept | 2 hr |
| 3–4 | Build a golden test harness: YAML test cases → run prompt → compare output | 2 hr |
| 5 | Metrics: exact match, semantic similarity (`sentence-transformers`), BLEU/ROUGE basics | 1.5 hr |
| 6–7 | [Lesson 10](./10-ai-agents-production/README.md) (preview): offline evaluation section; RAGAS for RAG evaluation | 2 hr |

---

#### Week 12 — LLM Integration Project

| Day | Activity | Time |
|-----|----------|------|
| 1–3 | Add LLM capability to your Agent Service API: chat endpoint with system prompt | 3 hr |
| 4–5 | Add streaming response support | 2 hr |
| 6–7 | Run eval harness against your API; fix regressions; document eval results in README | 2 hr |

**Month 3 Deliverable**: An LLM-powered chat API with a working evaluation harness and documented prompt library.

---

### Month 4 (Weeks 13–16) — Agent Architecture, RAG & Tooling

**Goal**: Build full AI agents using the patterns and tools in this repository.  
**Why now**: You have all the prerequisites — Python, APIs, LLMs, evals. Now combine them.

---

#### Week 13 — Agent Design Patterns (Core)

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | [Lesson 03](./03-agentic-design-patterns/README.md): Agentic design principles (Space, Time, Core) | 2 hr |
| 3–4 | [Lesson 04](./04-tool-use/README.md): Tool Use pattern — function schemas, execution loop, `@tool` decorator | 2 hr |
| 5 | [Lesson 07](./07-planning-design/README.md): Planning Design — task decomposition, re-planning | 1.5 hr |
| 6–7 | Build: agent with 3+ tools (calculator, web search, file reader); test each tool path | 2 hr |

---

#### Week 14 — RAG (Retrieval-Augmented Generation)

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | [Lesson 05](./05-agentic-rag/README.md): Agentic RAG — iterative retrieval, self-correction, multi-source | 2 hr |
| 3 | Vector embeddings: `sentence-transformers`, embedding dimensions, cosine similarity | 1.5 hr |
| 4 | Chunking strategies: fixed-size, sentence, semantic; overlap trade-offs | 1.5 hr |
| 5 | Azure AI Search or FAISS local: indexing, querying, re-ranking | 1.5 hr |
| 6–7 | Build: RAG pipeline over a small document set (e.g., this repo's READMEs) | 2 hr |

---

#### Week 15 — Agent Memory, Safety & Advanced Patterns

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | [Lesson 13](./13-agent-memory/README.md): Memory architectures (short-term, long-term, episodic, semantic) | 2 hr |
| 3 | [Lesson 06](./06-building-trustworthy-agents/README.md): Trustworthy AI — safety, PII, prompt injection defence | 1.5 hr |
| 4 | [Lesson 09](./09-metacognition/README.md): Metacognition — Reflexion, self-critique loops | 1.5 hr |
| 5–6 | [Lesson 14](./14-microsoft-agent-framework/README.md): Microsoft Agent Framework deep-dive | 2 hr |
| 7 | Add memory and safety guardrails to your tool-using agent | 1 hr |

---

#### Week 16 — Agent Integration Project

| Day | Activity | Time |
|-----|----------|------|
| 1–4 | Build "Document Q&A Agent": ingests docs, RAG retrieval, answers with citations | 4 hr |
| 5 | Integrate your eval harness: golden Q&A pairs + automatic faithfulness check | 1.5 hr |
| 6–7 | Add structured logging (correlation IDs, tool call traces), write README with demo GIF | 2 hr |

**Month 4 Deliverable**: A working agent with tool use, RAG, memory, safety guardrails, evaluation, and structured logging.

---

### Month 5 (Weeks 17–20) — Production Readiness & Deployment

**Goal**: Make your agents production-grade: observable, secure, deployable, and scalable.  
**Why now**: Junior-to-mid promotion requires more than "it works locally".

---

#### Week 17 — Observability & Monitoring

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | [Lesson 10](./10-ai-agents-production/README.md): Agents in Production — traces, spans, metrics, cost tracking | 2 hr |
| 3 | OpenTelemetry: instrumentation SDK, trace exporters, Jaeger/Zipkin local setup | 1.5 hr |
| 4 | Langfuse (or Azure AI Foundry tracing): LLM-specific observability | 1.5 hr |
| 5–6 | Add OpenTelemetry traces to your agent service (tool call spans, LLM call spans) | 2 hr |
| 7 | Alerting patterns: latency SLOs, error rate thresholds, cost budgets | 1 hr |

---

#### Week 18 — Multi-Agent Systems

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | [Lesson 08](./08-multi-agent/README.md): Multi-Agent patterns — group chat, hand-off, collaborative filtering | 2 hr |
| 3 | [Lesson 11](./11-agentic-protocols/README.md): Agentic protocols — MCP, A2A, NLWeb | 1.5 hr |
| 4–5 | Design and implement a 2-agent system (e.g., Planner + Executor) | 2 hr |
| 6–7 | Add visibility: log each inter-agent message, trace full multi-agent conversation | 2 hr |

---

#### Week 19 — Security, Cost & Reliability

| Day | Activity | Time |
|-----|----------|------|
| 1 | Input validation and sanitisation for agent inputs | 1 hr |
| 2 | Prompt injection defence: jailbreak detection, system prompt hardening | 1.5 hr |
| 3 | Cost control: model routing (expensive → cheap model), caching (Redis + semantic cache) | 1.5 hr |
| 4 | Concurrency: `asyncio` task management, queue-based agent execution (Redis/Celery) | 1.5 hr |
| 5–7 | Reliability: retries, timeouts, circuit breakers for LLM API calls | 2.5 hr |

---

#### Week 20 — CI/CD & Cloud Deployment

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | GitHub Actions: build → test → build Docker → push to registry → deploy | 2 hr |
| 3 | Secrets management: GitHub Secrets, Azure Key Vault basics | 1 hr |
| 4–5 | Deploy to Azure Container Apps (or App Service): environment variables, scaling | 2 hr |
| 6–7 | End-to-end production checklist: health check, logs in Azure Monitor, cost dashboard | 2 hr |

**Month 5 Deliverable**: Your Document Q&A Agent deployed to the cloud with OpenTelemetry traces, CI/CD pipeline, cost monitoring, and a live demo URL.

---

### Month 6 (Weeks 21–24) — Capstone Projects & Interview Prep

**Goal**: Build 1–2 polished, JD-aligned capstone projects and prepare intensively for interviews.

---

#### Week 21 — Capstone Design & Setup

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | Review your target JD (see Appendix A) and choose 1–2 capstone projects from Section 6 | 2 hr |
| 3 | Design architecture: draw system diagram, define APIs, choose tech stack | 2 hr |
| 4 | Set up repository, CI, Docker, `README.md` skeleton, and project board | 1.5 hr |
| 5–7 | Sprint 1: core agent loop + primary tool integration | 2.5 hr |

---

#### Week 22 — Capstone Build Sprint

| Day | Activity | Time |
|-----|----------|------|
| 1–4 | Sprint 2: RAG pipeline, memory, safety guardrails, eval harness | 5 hr |
| 5–7 | Sprint 3: observability, CI/CD, deployment, cost tracking | 3 hr |

---

#### Week 23 — Capstone Polish & System Design Prep

| Day | Activity | Time |
|-----|----------|------|
| 1–2 | Write comprehensive README: problem statement, architecture diagram, demo GIF, eval results | 2 hr |
| 3 | Record a 3-minute Loom walkthrough of your capstone | 1 hr |
| 4–5 | System design study: agent workflows, latency/cost trade-offs, data flow diagrams | 2 hr |
| 6–7 | Study [STUDY_GUIDE.md](./STUDY_GUIDE.md): Tier 1 lessons (RAG, production, multi-agent, tool use) | 2 hr |

---

#### Week 24 — Interview Prep Sprint

| Day | Activity | Time |
|-----|----------|------|
| 1 | Python coding: async, generators, dataclasses, typing — LeetCode Medium × 5 | 1.5 hr |
| 2 | LLM concepts: tokens, context, fine-tuning vs RAG, prompt patterns | 1.5 hr |
| 3 | Agent concepts: tool use, planning, memory, safety, multi-agent patterns | 1.5 hr |
| 4 | System design mock: "Design a customer support AI agent at scale" | 2 hr |
| 5 | Behavioural questions: STAR stories for each project you built | 1.5 hr |
| 6–7 | Mock interviews (Pramp, Interviewing.io, or with a peer) | 2 hr |

**Month 6 Deliverable**: 1–2 polished capstone projects on GitHub + portfolio README + interview preparation complete.

---

## 5. Milestones & Measurable Outputs

| Month | Milestone | Measurable Output |
|-------|-----------|------------------|
| 1 | Python & tooling foundation | GitHub repo: typed Python package, `pytest` tests ≥ 80% coverage, passing CI |
| 2 | Backend API service | FastAPI + Postgres service deployed via Docker + GitHub Actions; OpenAPI docs live |
| 3 | LLM integration + eval | Chat API endpoint + golden test harness with ≥ 10 test cases passing |
| 4 | Working AI agent | Agent with tool use, RAG, memory, safety; eval harness passing; demo GIF in README |
| 5 | Production-ready deployment | Live demo URL; OpenTelemetry traces visible in dashboard; CI/CD green |
| 6 | Portfolio + interview ready | 2 capstone projects, updated GitHub profile, 3 mock interviews completed |

---

## 6. Capstone Project Options

Choose projects that match your target JD. Each option is mapped to the most common AI agent job requirements.

---

### Option A — Document Intelligence Agent (Recommended for RAG / NLP Roles)

**What it does**: Ingests a document corpus (PDFs, Markdown, HTML), builds a searchable vector index, and answers user questions with cited sources. Optionally generates executive summaries.

**JD skills covered**: RAG, embeddings, vector search, LLM API integration, evaluation, observability.

**Tech stack**: Python, FastAPI, Azure AI Search (or FAISS), Azure OpenAI / OpenAI, Pydantic, PostgreSQL, Docker.

**Evaluation**: Automated faithfulness score (RAGAS), citation accuracy, latency percentiles.

**Repo structure**:
```
doc-agent/
├── src/
│   ├── ingestion/      # chunking, embedding, indexing
│   ├── retrieval/      # query, re-rank, top-k
│   ├── generation/     # prompt assembly, LLM call, citation
│   └── api/            # FastAPI endpoints
├── evals/              # golden Q&A pairs + eval runner
├── tests/
├── Dockerfile
└── README.md           # includes architecture diagram + demo
```

---

### Option B — Workflow Automation Agent (Recommended for Agentic / Multi-Step Roles)

**What it does**: Accepts a high-level goal ("research competitors and draft a report"), decomposes it into steps using a planning agent, executes each step (web search, summarisation, writing), and produces an auditable run log.

**JD skills covered**: Agent planning, tool use, multi-step reasoning, multi-agent orchestration, observability, safety.

**Tech stack**: Python, Microsoft Agent Framework (MAF), Azure AI Foundry, OpenTelemetry, Redis.

**Evaluation**: Plan quality (are steps sensible?), tool call success rate, end-to-end completion rate, cost per run.

**Repo structure**:
```
workflow-agent/
├── src/
│   ├── planner/        # goal decomposition → step list
│   ├── executor/       # tool dispatch, retry, result capture
│   ├── tools/          # web_search, summarise, write_file
│   └── observer/       # OpenTelemetry spans, run log storage
├── evals/
├── tests/
├── Dockerfile
└── README.md
```

---

### Option C — Customer Support Agent (Recommended for Product / SaaS Roles)

**What it does**: Handles customer queries using a RAG knowledge base (help docs, FAQs), escalates to human when confidence is low, tracks all conversations, and provides an admin dashboard with quality metrics.

**JD skills covered**: RAG, safety, escalation logic, conversation memory, eval metrics, production observability, admin tooling.

**Tech stack**: Python, FastAPI, PostgreSQL, Azure OpenAI, Azure AI Search, Langfuse (observability), Streamlit (admin UI).

**Evaluation**: Resolution rate, hallucination rate (LLM-as-judge), escalation accuracy, CSAT proxy (thumbs up/down).

---

### Option D — Code Review Agent (Recommended for Developer Tooling Roles)

**What it does**: Takes a GitHub PR diff, analyses the changes with an LLM, identifies bugs/style issues/security concerns, and posts structured review comments. Optionally runs in a GitHub Action.

**JD skills covered**: Tool use (GitHub API), LLM reasoning, structured output, CI/CD integration, security awareness.

**Tech stack**: Python, GitHub API (`PyGithub`), Azure OpenAI / OpenAI, Pydantic, GitHub Actions.

**Evaluation**: Precision/recall against a labelled set of intentional bugs; false positive rate.

---

## 7. Portfolio Readiness Checklist

Use this checklist before applying for roles. Each item should be true for every project in your portfolio.

### Code Quality
- [ ] Project has a `README.md` with: purpose, architecture diagram, setup instructions, demo
- [ ] Code uses Python type hints throughout (`mypy` passes with minimal errors)
- [ ] Tests exist with ≥ 70% line coverage (`pytest-cov`)
- [ ] Linting passes (`ruff check .`)
- [ ] No secrets committed (`.env` is in `.gitignore`; `.env.example` exists)
- [ ] Dependencies pinned in `requirements.txt` or `pyproject.toml`

### AI / Agent Quality
- [ ] At least one agent uses tools (function calling / `@tool` decorator)
- [ ] At least one project uses RAG (embeddings + retrieval + generation)
- [ ] Evaluation harness exists (golden test cases + automated scoring)
- [ ] Prompt templates are version-controlled and documented
- [ ] Safety guardrails are implemented (input validation, output checking)

### Production Quality
- [ ] Application runs in Docker (`docker build` + `docker run` work with no manual steps)
- [ ] CI/CD pipeline passes (GitHub Actions: lint → test → build → deploy)
- [ ] Observability is wired (structured logs with correlation IDs; ideally OpenTelemetry traces)
- [ ] Health check endpoint exists (`/health` or `/ping`)
- [ ] Cost estimation documented (estimated $ per 1000 requests)

### Portfolio Presentation
- [ ] GitHub profile `README.md` lists your top 2–3 projects with one-line descriptions
- [ ] Each project has a demo (GIF, video, or live URL)
- [ ] At least one project has an "Evaluation Results" section with numbers
- [ ] Architecture diagram exists (can be a simple ASCII diagram or Mermaid chart)
- [ ] You can explain every line of code in your projects in an interview

### Interview Readiness
- [ ] Can define and contrast: RAG vs fine-tuning, single-agent vs multi-agent, MCP vs REST
- [ ] Can walk through a tool use flow end-to-end (schema → LLM → execution → result)
- [ ] Can design a multi-agent customer support system from scratch (system design question)
- [ ] Can explain how you would evaluate an LLM agent in production
- [ ] Can describe one failure you hit in a project and how you fixed it (STAR format)
- [ ] Have completed ≥ 3 mock interviews (coding + system design + behavioural)

---

## Appendix A — Job Description Paste Template

> **Instructions**: LinkedIn job pages are often gated and inaccessible in automation environments.  
> To get a personalized plan tailored to your specific JD, paste the job description text below  
> and use the mapping table in [Appendix B](#appendix-b--skills--modules--projects-mapping-table-generic) to map each required skill to the relevant  
> lesson(s) and project(s) in this plan.

---

### How to Paste Your JD

1. Open the LinkedIn job posting (or any other job board).
2. Copy the full text of the **Responsibilities** and **Requirements / Qualifications** sections.
3. Paste it in the section below, replacing the placeholder text.
4. Work through Appendix B to identify which weeks in this plan to prioritise.

---

```
=== JOB DESCRIPTION (PASTE HERE) ===

Job Title: 
Company:
Location:
Posted:

--- ABOUT THE ROLE / WHAT YOU'LL DO ---
[Paste responsibilities here]

--- REQUIREMENTS / QUALIFICATIONS ---
[Paste requirements here]

--- NICE TO HAVE ---
[Paste nice-to-have skills here]

=== END OF JOB DESCRIPTION ===
```

---

### Quick JD Analysis Questions

After pasting the JD, answer these questions to prioritise your study plan:

| Question | Your Answer | Impact on Plan |
|----------|-------------|----------------|
| Is this Junior, Mid, or Senior level? | | Junior/Mid → 6 months likely enough; Senior → plan 9–12 months |
| Does it require production ML/LLM experience? | Yes / No | Yes → prioritise Month 5; compress Month 1–2 if you have prior backend experience |
| Does it mention RAG, vector search, or embeddings? | Yes / No | Yes → Week 14 (RAG) is mandatory; add Option A capstone |
| Does it mention multi-agent or agent orchestration? | Yes / No | Yes → Week 18 (multi-agent) is mandatory; add Option B capstone |
| Does it require cloud deployment (Azure, AWS, GCP)? | Yes / No | Yes → Month 5 (production) must include cloud deployment |
| Does it mention observability, monitoring, or MLOps? | Yes / No | Yes → Week 17 (observability) is mandatory; demonstrate OpenTelemetry in portfolio |
| Does it require specific frameworks (LangChain, AutoGen, etc.)? | | Add 1 week to learn that specific framework; map to Lesson 02 (Agentic Frameworks) |
| What is the required years of experience? | | <3 yrs → junior target; 3–6 yrs → mid target; 6+ yrs → senior target |

---

## Appendix B — Skills → Modules → Projects Mapping Table (Generic)

This table maps the most common AI agent job requirements to the lessons in this repository and the capstone projects in Section 6. Use it alongside your pasted JD to prioritise your study weeks.

| JD Skill / Requirement | Lesson(s) | Plan Weeks | Capstone Project |
|------------------------|-----------|------------|-----------------|
| **Python (intermediate+)** | Lesson 00 setup; Python best practices | Weeks 1–4 (Month 1) | All capstones |
| **LLM API integration** (OpenAI, Azure OpenAI) | Lesson 01, 02 | Weeks 9–10 (Month 3) | All capstones |
| **Prompt engineering** | Lesson 12 (Context Engineering) | Week 10 (Month 3) | All capstones |
| **Function calling / Tool use** | Lesson 04 | Week 13 (Month 4) | B (Workflow Agent), D (Code Review Agent) |
| **RAG / vector search / embeddings** | Lesson 05 | Week 14 (Month 4) | A (Document Agent), C (Support Agent) |
| **Agent memory** | Lesson 13 | Week 15 (Month 4) | C (Support Agent) |
| **Multi-agent orchestration** | Lesson 08 | Week 18 (Month 5) | B (Workflow Agent) |
| **Agent planning** | Lesson 07 | Week 13 (Month 4) | B (Workflow Agent) |
| **Responsible AI / safety / guardrails** | Lesson 06 | Week 15 (Month 4) | All capstones |
| **Agentic protocols (MCP, A2A)** | Lesson 11 | Week 18 (Month 5) | B (Workflow Agent) |
| **Evaluation / testing LLM systems** | Lesson 10 (production evals) | Weeks 11–12 (Month 3) + Week 16 | All capstones |
| **Observability (OpenTelemetry, traces)** | Lesson 10 | Week 17 (Month 5) | All capstones |
| **Production deployment (Docker, CI/CD)** | Lesson 00 + production section | Weeks 8, 20 | All capstones |
| **Cloud platforms (Azure AI Foundry)** | Lesson 00, 10, 14 | Weeks 4, 17–20 | All capstones |
| **REST API development** | FastAPI (not a lesson — external) | Weeks 5–8 (Month 2) | All capstones |
| **FastAPI / async Python** | External; supports all lessons | Weeks 5–8 (Month 2) | All capstones |
| **Testing (pytest, mocking)** | External; supports all lessons | Weeks 2, 7 | All capstones |
| **PostgreSQL / databases** | External; supports all lessons | Weeks 6–7 | All capstones |
| **Redis / caching** | External; supports all lessons | Weeks 6, 19 | B, C capstones |
| **Git / GitHub Actions / CI** | External; supports all lessons | Weeks 2, 4, 8, 20 | All capstones |
| **Docker / containerisation** | External; supports all lessons | Weeks 4, 8, 20 | All capstones |
| **Security (prompt injection, input validation)** | Lesson 06 | Weeks 15, 19 | All capstones |
| **Cost management for LLM workloads** | Lesson 10 | Weeks 17, 19 | All capstones |
| **Microsoft Agent Framework (MAF)** | Lesson 14 | Week 15 (Month 4) | B (Workflow Agent) |
| **LangChain / AutoGen / Semantic Kernel** | Lesson 02 | Week 9 (Month 3) | Any capstone |
| **Browser automation agents** | Lesson 15 | Week 21+ (Month 6 capstone) | Optional capstone |
| **System design for AI systems** | Lessons 08, 10 + STUDY_GUIDE.md | Week 23 (Month 6) | All capstones |
| **Machine learning fundamentals** | External (Lesson 01 covers agent theory) | Month 3 supplemental | N/A (theory) |

---

### How to Use This Table

1. Paste your JD into [Appendix A](#appendix-a--job-description-paste-template).
2. For each required skill in the JD, find the matching row in the table above.
3. Mark the corresponding **Plan Weeks** as **high priority** in your study schedule.
4. Choose the **Capstone Project** whose coverage most closely matches the mandatory skills.
5. If a skill appears in both "Requirements" and "Nice to Have", treat it as a bonus and study it in Month 6 if time allows.

---

*Last updated: 2026-05 | Repository: [microsoft/ai-agents-for-beginners](https://github.com/microsoft/ai-agents-for-beginners)*
