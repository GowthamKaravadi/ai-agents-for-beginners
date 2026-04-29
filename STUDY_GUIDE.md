# AI Agents for Beginners — Study Guide, Course Summary & AI/ML Interview Prep

This guide serves two purposes:
1. **Course Summary**: A quick-reference overview of every lesson in the "AI Agents for Beginners" course.
2. **AI/ML Interview Prep**: A prioritized, tier-based study plan tailored to Senior AI/ML Engineer interview preparation, mapped directly to real-world job requirements.

---

## Part A — Repository Analysis for Interview Preparation

### A.1 Public Repositories Under `GowthamKaravadi`

| # | Repository | Branch | Purpose | Main Technologies | AI/ML Areas | Production Readiness |
|---|-----------|--------|---------|-------------------|-------------|----------------------|
| 1 | **ai-agents-for-beginners** | `main` | Structured 16-lesson course teaching how to build production-grade AI agents end-to-end | Python 3.12, Jupyter Notebooks, Azure AI Foundry, Microsoft Agent Framework (MAF), MCP, A2A | GenAI, Agents, RAG, Multi-Agent Systems, MLOps/Observability, Agentic Protocols | CI/CD via GitHub Actions; `.devcontainer` for Codespaces; structured `requirements.txt`; lesson code samples runnable in Azure environments |

> **Note**: The account may contain additional private or forked repositories. The list above reflects confirmed public repositories accessible via the `main` branch as of the time this guide was generated.

---

### A.2 Deep-Dive: `ai-agents-for-beginners`

**Purpose**: A Microsoft-curated, open-source educational course covering the full lifecycle of AI agent development — from fundamentals through multi-agent orchestration, RAG, safety, and production deployment.

**Main Technologies**:
- Language: Python 3.12+
- Notebooks: Jupyter (`.ipynb`)
- Cloud: Azure AI Foundry / Azure OpenAI
- Frameworks: Microsoft Agent Framework (MAF), Azure AI Agent Service V2
- Protocols: Model Context Protocol (MCP), Agent-to-Agent (A2A), NLWeb
- Libraries: `agent-framework`, `a2a-sdk`, `azure-ai-projects`, `azure-identity`, `azure-search-documents`, `openai`, `mcp[cli]`

**AI/ML Areas Covered**:

| Area | Lessons |
|------|---------|
| GenAI / LLM Fundamentals | 01, 02, 03 |
| Agentic Design Patterns | 03, 04, 07, 08, 09 |
| RAG (Retrieval-Augmented Generation) | 05 |
| Trustworthy / Responsible AI | 06 |
| Multi-Agent Systems | 08 |
| Metacognition & Self-Correction | 09 |
| MLOps / Observability / Production | 10 |
| Agentic Protocols (MCP, A2A, NLWeb) | 11 |
| Context Engineering | 12 |
| Agent Memory | 13 |
| Framework Deep-Dive (MAF) | 14 |
| Browser Automation Agents | 15 |

**Evidence of Production Readiness**:
- GitHub Actions CI/CD pipeline (`.github/workflows/`)
- `.devcontainer` for reproducible dev environments
- Structured Python `requirements.txt` with pinned dependencies
- Observability instrumentation via OpenTelemetry in code samples
- Security coverage: prompt injection, PII handling, content safety (Lesson 06, 10)
- Evaluation frameworks: offline/online eval, RAGAS, LLM-as-judge (Lesson 10)

---

## Part B — Prioritized Study Plan (Tier 1 / 2 / 3)

> **Mapping to Job Requirements**: The tiers below are ordered by observed frequency and weight in Senior AI/ML Engineer job postings and interview reports as seen on LinkedIn, Naukri, and equivalent platforms in 2025–2026. This is based on observed trends rather than exhaustive data and may vary by company.

### 🔴 Tier 1 — Must-Study (Maximum ROI per Hour)

These lessons directly map to the **most common Senior AI/ML interview topics**: GenAI architecture, RAG, production deployment, system design, and agent orchestration.

| Priority | Lesson | Interview Topic Mapped | Time Estimate |
|----------|--------|------------------------|---------------|
| **1** | **Lesson 01** — Intro to AI Agents | GenAI fundamentals, agent types, use cases | 1–2 hr |
| **2** | **Lesson 05** — Agentic RAG | RAG architecture, iterative retrieval, self-correction, NL2SQL | 2–3 hr |
| **3** | **Lesson 10** — AI Agents in Production | MLOps, observability (traces/spans), evaluation (offline/online), cost management | 2–3 hr |
| **4** | **Lesson 08** — Multi-Agent Systems | System design, agent coordination, fault tolerance, scalability | 2 hr |
| **5** | **Lesson 04** — Tool Use Design Pattern | Function calling, schema design, LLM↔tool integration | 1–2 hr |
| **6** | **Lesson 11** — Agentic Protocols (MCP, A2A, NLWeb) | Standardized agent communication, interoperability, enterprise integration | 1–2 hr |

**Why Tier 1?**
- RAG is one of the most asked-about GenAI topics in 2025-2026 interviews.
- Production observability and MLOps are baseline expectations for Senior roles.
- Multi-agent system design mirrors real-world distributed AI systems.
- Tool use / function calling is tested in nearly every LLM/agent coding interview.
- MCP and A2A are emerging enterprise standards interviewers probe for awareness of.

---

### 🟡 Tier 2 — Important (Depth After Tier 1)

These lessons deepen your understanding of agent design and safety — both common in behavioral and system design rounds.

| Priority | Lesson | Interview Topic Mapped | Time Estimate |
|----------|--------|------------------------|---------------|
| **7** | **Lesson 02** — Agentic Frameworks | Framework comparison (AutoGen, LangChain, Semantic Kernel, MAF), design trade-offs | 2 hr |
| **8** | **Lesson 07** — Planning Design | Task decomposition, iterative re-planning, agentic workflows | 1–2 hr |
| **9** | **Lesson 06** — Trustworthy AI Agents | Responsible AI, safety guardrails, PII, prompt injection, bias | 1–2 hr |
| **10** | **Lesson 14** — Microsoft Agent Framework | Middleware, workflows, checkpointing, orchestration patterns | 2 hr |
| **11** | **Lesson 09** — Metacognition | Self-reflection, self-correction, reflexion patterns | 1 hr |
| **12** | **Lesson 13** — Agent Memory | Memory architectures (short-term, long-term, episodic, semantic) | 1 hr |

**Why Tier 2?**
- Framework comparison is a standard "why did you choose X over Y?" question.
- Planning and metacognition tie to reasoning ability questions ("How would you handle a failing LLM chain?").
- Trustworthy AI is mandatory at FAANG/enterprise companies (safety reviews, bias audits).
- Memory architecture connects to database and state management system design.

---

### 🟢 Tier 3 — Nice to Have (Skim for Breadth)

These lessons add breadth and handle niche interview questions or specialization areas.

| Priority | Lesson | Interview Topic Mapped | Time Estimate |
|----------|--------|------------------------|---------------|
| **13** | **Lesson 03** — Agentic Design Principles | UX principles for agents, human-in-the-loop design | 0.5–1 hr |
| **14** | **Lesson 12** — Context Engineering | Prompt engineering at scale, context window management | 1 hr |
| **15** | **Lesson 15** — Browser Use Agents | Web automation, emerging agent capabilities | 0.5 hr |
| **16** | **Lesson 00** — Course Setup | Environment setup; only needed for hands-on coding | 0.5 hr |

---

## Part C — Quick-Start Reading Plans for Tier 1 Lessons

### 📖 Lesson 01 — Introduction to AI Agents
**Folder**: `01-intro-to-ai-agents/`

**Files to Read First**:
1. `README.md` — Full lesson (10 min read)
2. `code_samples/01-python-agent-framework.ipynb` — Run the code and trace the agent loop

**Interview Concepts Checklist**:
- [ ] Define an AI Agent and distinguish it from a standard LLM chatbot
- [ ] Name and explain all 5+ agent types (Reflex, Model-Based, Goal-Based, Utility-Based, Learning, Hierarchical, Multi-Agent)
- [ ] Describe the 3 core agent components: Environment, Sensors, Actuators
- [ ] Explain when to use agents vs. simple LLM calls (open-ended, multi-step, improvement over time)
- [ ] Compare agentic vs. non-agentic workflows with a real-world example

---

### 📖 Lesson 05 — Agentic RAG
**Folder**: `05-agentic-rag/`

**Files to Read First**:
1. `README.md` — Full lesson; focus on "Agentic RAG Core Loop" section
2. `code_samples/05-python-agent-framework.ipynb` — Trace the iterative retrieval loop

**Interview Concepts Checklist**:
- [ ] Explain the difference between traditional RAG and Agentic RAG
- [ ] Describe the iterative "maker-checker" loop and why it improves accuracy
- [ ] Explain how the agent owns its reasoning process (vs. scripted retrieval chains)
- [ ] Walk through the tool integration architecture (vector search → SQL → custom API)
- [ ] Describe self-correction mechanisms (re-querying, fallback to human oversight)
- [ ] Explain governance, explainability, and bias control in Agentic RAG
- [ ] Discuss when Agentic RAG is NOT the right choice (latency, cost, simple queries)
- [ ] Name at least 3 tools used: Azure AI Search, Azure SQL, Bing Web Grounding

---

### 📖 Lesson 10 — AI Agents in Production
**Folder**: `10-ai-agents-production/`

**Files to Read First**:
1. `README.md` — Full lesson; focus on metrics, evaluation, and cost sections
2. `code_samples/10-expense_claim-demo.ipynb` — Live example with traces and evaluation

**Interview Concepts Checklist**:
- [ ] Explain what "observability" means for AI agents (traces vs. spans)
- [ ] Name 5+ key production metrics: latency, cost, error rate, accuracy, user feedback
- [ ] Explain the difference between offline evaluation (test datasets) and online evaluation (live monitoring)
- [ ] Describe the offline→deploy→monitor→improve feedback loop
- [ ] Explain how to reduce LLM agent costs: smaller models, router models, caching
- [ ] Describe OpenTelemetry instrumentation for agents
- [ ] Explain how to handle common production issues: infinite loops, poor tool calls, multi-agent inconsistency
- [ ] Name observability tools: Langfuse, Azure AI Foundry, RAGAS, LLM Guard

---

### 📖 Lesson 08 — Multi-Agent Systems
**Folder**: `08-multi-agent/`

**Files to Read First**:
1. `README.md` — Full lesson; focus on design patterns and building blocks
2. `solution/solution.md` — Study the solution to the customer support design exercise

**Interview Concepts Checklist**:
- [ ] Describe 3 scenarios where multi-agent is better than single-agent
- [ ] Explain the advantages: specialization, scalability, fault tolerance
- [ ] Name and describe the 5 multi-agent building blocks: communication, coordination, architecture, visibility, patterns
- [ ] Describe 3 multi-agent patterns: group chat, hand-off, collaborative filtering
- [ ] Design a multi-agent system for a given domain (e.g., e-commerce refund, travel booking)
- [ ] Explain centralized vs. decentralized agent architectures
- [ ] Describe how to implement visibility/logging in multi-agent systems

---

### 📖 Lesson 04 — Tool Use Design Pattern
**Folder**: `04-tool-use/`

**Files to Read First**:
1. `README.md` — Full lesson; focus on function calling code examples
2. `code_samples/04-python-agent-framework.ipynb` — Implement and run the tool use pattern

**Interview Concepts Checklist**:
- [ ] Explain the Tool Use design pattern and its 6 building blocks (function schemas, execution logic, message handling, tool integration, error handling, state management)
- [ ] Write a function schema (JSON) for a custom tool
- [ ] Describe the full function calling flow: schema → LLM selects tool → execute → return result → LLM final response
- [ ] Use the `@tool` decorator in Microsoft Agent Framework
- [ ] Explain security considerations for tool use (SQL injection, read-only permissions, sandboxing)
- [ ] Compare MAF tool use vs. raw OpenAI function calling

---

### 📖 Lesson 11 — Agentic Protocols
**Folder**: `11-agentic-protocols/`

**Files to Read First**:
1. `README.md` — Full lesson; covers MCP, A2A, and NLWeb

**Interview Concepts Checklist**:
- [ ] Explain what MCP (Model Context Protocol) is and its 3 core primitives: Tools, Resources, Prompts
- [ ] Describe MCP's client-server architecture (Hosts, Clients, Servers)
- [ ] Compare MCP to traditional APIs (dynamic discovery vs. static integration)
- [ ] Explain A2A (Agent-to-Agent) protocol: Agent Cards, Agent Executor, Artifact, Event Queue
- [ ] Walk through A2A communication flow for a multi-vendor agent scenario
- [ ] Explain how NLWeb enables natural language interaction with websites via MCP
- [ ] Describe the security benefits of standardized protocols (built-in auth, interoperability)

---

## Part D — Cross-Cutting Interview Concepts

### D.1 System Design Patterns Summary

| Pattern | Lesson | One-Line Description |
|---------|--------|----------------------|
| Tool Use | 04 | LLM selects and calls external functions via schemas |
| Planning | 07 | Agent decomposes goals into subtask sequences |
| Agentic RAG | 05 | Iterative LLM↔retrieval loop with self-correction |
| Multi-Agent | 08 | Multiple specialized agents coordinate to solve complex tasks |
| Metacognition | 09 | Agent reflects on its own reasoning and adapts |
| ReAct | 02, 09 | Reasoning + Acting in an interleaved loop |
| Reflexion | 09 | Verbal reinforcement learning through self-feedback |

### D.2 Technology Stack to Know

| Technology | Why Interviewers Ask | Where to Study |
|-----------|---------------------|----------------|
| Azure AI Foundry | Microsoft cloud platform for production agents | Lessons 01, 10, 14 |
| Microsoft Agent Framework (MAF) | End-to-end Python agent SDK | Lessons 02, 04, 14 |
| Azure AI Search | Vector search for RAG | Lesson 05 |
| OpenTelemetry | Observability standard for LLM apps | Lesson 10, 14 |
| MCP (Model Context Protocol) | Emerging standard for LLM↔tool integration | Lesson 11 |
| A2A Protocol | Multi-agent communication standard | Lesson 11 |
| RAGAS | RAG evaluation framework | Lesson 10 |
| LangChain / AutoGen / Semantic Kernel | Competing frameworks (comparison questions) | Lesson 02 |

### D.3 Common Interview Questions → Where to Find Answers

| Interview Question | Best Lesson to Study |
|-------------------|----------------------|
| "Explain RAG. What are its limitations?" | Lesson 05 |
| "How do you evaluate an LLM application in production?" | Lesson 10 |
| "Design a multi-agent customer support system" | Lesson 08 |
| "What is function calling and how does it work?" | Lesson 04 |
| "How do you handle agent failures in production?" | Lessons 10, 08 |
| "What is the difference between RAG and fine-tuning?" | Lesson 05, 02 |
| "What frameworks have you used for building agents?" | Lesson 02, 14 |
| "How do you ensure AI agent safety and trustworthiness?" | Lesson 06 |
| "Explain MCP and why it matters" | Lesson 11 |
| "How would you reduce inference cost for an agent in production?" | Lesson 10 |
| "What is chain-of-thought prompting? How does it relate to agents?" | Lessons 07, 09 |
| "Walk me through your approach to prompt engineering" | Lesson 12 |

---

## Part E — Course Summary (All Lessons At a Glance)

| Lesson | Title | Key Takeaway |
|--------|-------|-------------|
| 00 | Course Setup | Environment, Azure setup, dependencies |
| 01 | Intro to AI Agents | Agent types, components, when to use agents |
| 02 | Agentic Frameworks | MAF, AutoGen, LangChain, Semantic Kernel comparison |
| 03 | Agentic Design Principles | Human-centric UX: Space/Time/Core dimensions |
| 04 | Tool Use Pattern | Function calling, schema definition, execution loop |
| 05 | Agentic RAG | Iterative retrieval, self-correction, multi-source grounding |
| 06 | Trustworthy AI Agents | Safety, responsible AI, prompt injection defense |
| 07 | Planning Design | Task decomposition, re-planning, goal-based agents |
| 08 | Multi-Agent Systems | Coordination patterns, handoff, group chat, filtering |
| 09 | Metacognition | Self-reflection, Reflexion, self-critique loops |
| 10 | Agents in Production | Observability, evaluation (offline/online), cost management |
| 11 | Agentic Protocols | MCP, A2A, NLWeb — standardized agent communication |
| 12 | Context Engineering | Prompt engineering, context window management |
| 13 | Agent Memory | Short-term, long-term, episodic, semantic memory types |
| 14 | Microsoft Agent Framework | MAF deep-dive: middleware, workflows, observability, memory |
| 15 | Browser Use Agents | Autonomous web browsing and interaction |

---

## Part F — Original Course Design Pattern Reference

### F.1 What are AI Agents?
AI Agents are systems that extend the capabilities of Large Language Models (LLMs) by giving them access to **tools**, **knowledge**, and **memory**. Unlike a standard LLM chatbot that only generates text based on training data, an AI Agent can:
- **Perceive** its environment (via sensors or inputs).
- **Reason** about how to solve a problem.
- **Act** to change the environment (via actuators or tool execution).

**Key Components of an Agent:**
- **Environment**: The space where the agent operates (e.g., a booking system).
- **Sensors**: Mechanisms to gather information (e.g., reading an API).
- **Actuators**: Mechanisms to perform actions (e.g., sending an email).
- **Brain (LLM)**: The reasoning engine that plans and decides which actions to take.

### F.2 Agentic Frameworks

The course uses **Microsoft Agent Framework (MAF)** with **Azure AI Foundry Agent Service V2** for building agents:

| Component | Focus | Best For |
|-----------|-------|----------|
| **Microsoft Agent Framework** | Unified Python/C# SDK for agents, tools, and workflows | Building agents with tools, multi-agent workflows, and production patterns. |
| **Azure AI Foundry Agent Service** | Managed cloud runtime | Secure, scalable deployment with built-in state management, observability, and trust. |

### F.3 Agentic Design Patterns

Design patterns help structure how agents operate to solve problems reliably.

#### **Tool Use Pattern** (Lesson 4)
This pattern enables agents to interact with the outside world.
- **Concept**: The agent is provided with a "schema" (a list of available functions and their parameters). The LLM decides *which* tool to call and with *what* arguments based on the user's request.
- **Flow**: User Request → LLM → **Tool Selection** → **Tool Execution** → LLM (with tool output) → Final Response.
- **Use Cases**: Retrieving real-time data (weather, stock prices), performing calculations, executing code.

#### **Planning Pattern** (Lesson 7)
This pattern enables agents to solve complex, multi-step tasks.
- **Concept**: The agent breaks down a high-level goal into a sequence of smaller subtasks.
- **Approaches**:
  - **Task Decomposition**: Splitting "Plan a trip" into "Book flight", "Book hotel", "Rent car".
  - **Iterative Planning**: Re-evaluating the plan based on the output of previous steps (e.g., if the flight is full, choose a different date).
- **Implementation**: Often involves a "Planner" agent that generates a structured plan (e.g., JSON) which is then executed by other agents.

### F.4 Design Principles

When designing agents, consider three dimensions:
- **Space**: Agents should connect people and knowledge, be accessible but unobtrusive.
- **Time**: Agents should learn from the *Past*, provide relevant nudges in the *Now*, and adapt for the *Future*.
- **Core**: Embrace uncertainty but establish trust through transparency and user control.

---

## Part G — How to Triage & Prioritize Unknown GitHub Repositories for AI/ML Interview Prep

When you have a list of GitHub repositories (your own or others') and don't yet know their contents, use the following fast-triage methodology — the same approach a senior engineer applies when onboarding to an unfamiliar codebase.

---

### G.1 The Five-Step Triage Process

#### Step 1 — Enumerate Repos and Capture Quick Metadata

Before opening a single file, collect surface-level signals for every repository:

| Signal | What to Note |
|--------|-------------|
| **Primary language(s)** | Python-heavy repos signal ML/data work; Go/Rust may indicate infra |
| **Last commit date** | Actively maintained vs. abandoned project |
| **Stars / forks** | Popularity proxy; high stars = proven utility |
| **Topics / tags** | Explicit labels like `machine-learning`, `llm`, `mlops`, `rag` |
| **Description / title** | One-line self-description is often the fastest signal |
| **Number of open issues / PRs** | High activity = production-grade or actively developed |

**Goal**: After Step 1 you should be able to mark each repo as "probably ML/AI", "probably infra/DevOps", or "unclear — needs inspection".

---

#### Step 2 — Inspect Key Entry-Point Files (≤ 5 min per repo)

For every repo that passed the Step 1 filter, read these files **in order**:

1. **`README.md`** — Goal, architecture, setup instructions, results/benchmarks. This single file answers ~70 % of classification questions.
2. **Dependency files** — `requirements.txt`, `pyproject.toml`, `environment.yml`, `Pipfile`, or `package.json`. The library list reveals the ML stack instantly:
   - `torch`, `tensorflow`, `jax` → deep learning
   - `transformers`, `langchain`, `openai`, `semantic-kernel`, `autogen` → LLM/agent work
   - `scikit-learn`, `xgboost`, `lightgbm` → classical ML
   - `mlflow`, `prefect`, `airflow`, `kubeflow` → MLOps / pipelines
   - `fastapi`, `flask`, `uvicorn` → model serving / APIs
3. **Notebooks (`*.ipynb`)** — Scan cell titles. Look for the sequence: EDA → model training → evaluation → deployment.
4. **Entry-point scripts** — `main.py`, `train.py`, `inference.py`, `app.py`, `api.py`, `serve.py`
5. **Infrastructure files** — `Dockerfile`, `docker-compose.yml`, `.github/workflows/*.yml`, `Makefile`
6. **Config files** — `configs/`, `*.yaml`, `hydra` configs (training hyperparameters, pipeline definitions)

**Goal**: After Step 2 you can fill in the table below for each repo.

---

#### Step 3 — Classify Each Repo into ML Interview Buckets

| Bucket | Signals to Look For | Interview Relevance |
|--------|-------------------|---------------------|
| **ML Fundamentals** | `scikit-learn`, classical algorithms, cross-validation, feature engineering | Algorithm theory, bias/variance trade-offs |
| **Deep Learning** | PyTorch/TensorFlow training loops, custom model architectures, backpropagation demos | DL architecture questions, optimization |
| **NLP / LLMs** | `transformers`, fine-tuning, tokenization, RLHF, prompt engineering, RAG | Most-asked topic in 2025–2026 interviews |
| **GenAI / Agents** | `langchain`, `autogen`, `semantic-kernel`, `agent-framework`, MCP, A2A, tool use | Rapidly growing interview category |
| **MLOps / Production** | `mlflow`, `docker`, CI/CD, model monitoring, drift detection, A/B testing | Senior-level baseline requirement |
| **Data Engineering** | `spark`, `dbt`, `airflow`, `kafka`, feature stores, ETL pipelines | Data infrastructure / pipeline design rounds |
| **Demos / POCs** | Single notebook, no tests, no CI, README is a README template | Low priority; skim only |

---

#### Step 4 — Prioritize Using Learning-ROI Tiers

Once each repo is classified, assign a tier:

| Tier | Criteria | Action |
|------|----------|--------|
| 🔴 **Tier 1** | End-to-end pipeline **+** production signals (API, Docker, tests, CI/CD, observability, evaluation) covering NLP/LLM/GenAI or MLOps | Study in depth — read all code, run notebooks, review PRs and issues |
| 🟡 **Tier 2** | Strong modeling or agents, but not fully productionized (e.g., good training code but no serving layer) | Study core concepts; skip boilerplate setup |
| 🟢 **Tier 3** | Demos, tutorials, small POCs, or utility scripts | Skim README and one representative notebook |

**Ordering rule within each tier**: prioritize repos that cover topics you've seen most frequently in recent job postings (RAG, agents, MLOps, system design) before those covering niche or foundational topics you already know well.

---

#### Step 5 — Build a Per-Repo "What to Read First" Plan

For each Tier 1 repo, create a short reading plan:

```
Repo: <repo-name>
Tier: 1
Bucket(s): NLP/LLMs, MLOps
Time estimate: 2–3 hr

Files to read first:
  1. README.md               — understand goal and architecture
  2. requirements.txt        — confirm tech stack
  3. notebooks/01_eda.ipynb  — understand data and problem framing
  4. src/train.py            — trace the training loop
  5. src/serve.py / api.py   — understand how the model is served
  6. .github/workflows/      — review CI/CD pipeline
  7. tests/                  — understand quality standards

Interview concepts to extract:
  - [ ] What ML problem is being solved?
  - [ ] What model/architecture is used and why?
  - [ ] How is the model evaluated (metrics, test set, production)?
  - [ ] How is the model deployed and monitored?
  - [ ] What were the key engineering trade-offs?
```

---

### G.2 Fallback: When Full Content Access Is Not Possible

If you cannot read the files inside a repo (private repos, API rate limits, no clone access), use the following metadata-only strategy:

| Metadata Source | What to Extract | How to Use It |
|----------------|----------------|---------------|
| **Repo description** | Domain, goal, tech stack keywords | First filter for ML relevance |
| **Topics / tags** | Explicit labels (`rag`, `llm`, `pytorch`, `mlops`) | Map directly to interview buckets in G.1 |
| **Primary language stat** | Python ≥ 80 % → strong ML signal | Deprioritize non-Python-primary repos unless infra-focused |
| **Commit activity graph** | Consistent commits over 6–12 months → production use | High-activity repos more likely to have production patterns |
| **Open issues / PRs** | Bug reports, feature requests, discussions | Signals real usage; issues about "model accuracy" or "latency" = production concerns |
| **Releases / tags** | Versioned releases (`v1.0`, `v2.3`) → mature, documented codebase | Prioritize versioned repos over `main`-only |
| **Fork count** | High forks → reference/template repo used by others | Good sign of educational or reusable value |
| **README preview** (first 1000 chars) | Even a partial README reveals the repo's purpose | Look for ML framework names, dataset names, task descriptions |

**Metadata-only prioritization checklist:**

```
For each repo (metadata only):
  [ ] Language is Python (or Python + infrastructure language)?
  [ ] Has topics/tags matching: ml, ai, llm, nlp, rag, agents, mlops, deep-learning?
  [ ] Description or name mentions a recognizable ML task or framework?
  [ ] Active commits in the last 6 months?
  [ ] Has open issues or PRs (signals active real-world use)?
  [ ] Has versioned releases?

Score: count of Yes answers
  5–6 Yes → Tier 1 candidate (request access or ask owner for key files)
  3–4 Yes → Tier 2 candidate (skim when accessible)
  0–2 Yes → Tier 3 or skip
```

---

### G.3 Fast Triage Cheat Sheet

```
REPO TRIAGE LOOP (per repo, ~5 min):
─────────────────────────────────────────────────────────────
1. METADATA:  language, topics, stars, last commit, description
              → mark as ML/non-ML/unclear

2. README:    goal? stack? results? architecture diagram?
              → confirm ML bucket(s)

3. DEPS:      requirements.txt / pyproject.toml
              → confirm framework (PyTorch, HF, LangChain, MLflow…)

4. NOTEBOOKS: *.ipynb titles → EDA? training? evaluation? demo?
              → identify depth of ML coverage

5. INFRA:     Dockerfile? CI? tests? monitoring?
              → assign production-readiness score

ASSIGN TIER:
  Tier 1 → end-to-end + production signals + LLM/RAG/MLOps
  Tier 2 → strong modeling, partial production
  Tier 3 → demo / tutorial / PoC

FALLBACK (no content access):
  Use metadata checklist from G.2 → score 5-6 = Tier 1 candidate
─────────────────────────────────────────────────────────────
```

---

### G.4 Applying This Process to `GowthamKaravadi` Repositories

The same triage loop was applied to the public repositories under `GowthamKaravadi`. Results are captured in **Part A** of this guide. The `ai-agents-for-beginners` repo scored **Tier 1** on all criteria:

- ✅ Python 3.12, Jupyter notebooks, Azure AI Foundry, MAF (ML-relevant stack)
- ✅ Topics: `ai-agents`, `llm`, `rag`, `multi-agent`, `mlops` (explicit ML tags)
- ✅ Active commits, open issues, versioned course structure (production signals)
- ✅ CI/CD via GitHub Actions, `.devcontainer`, structured `requirements.txt`
- ✅ End-to-end coverage: from fundamentals (Lesson 01) through production deployment (Lesson 10)

To apply the triage process to additional repositories as they become accessible, use the checklist in **G.2** and the reading plan template in **G.1 Step 5**.
