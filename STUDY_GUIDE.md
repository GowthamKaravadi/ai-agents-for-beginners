# AI Agents for Beginners — Study Guide, Course Summary & AI/ML Interview Prep

This guide serves two purposes:
1. **Course Summary**: A quick-reference overview of every lesson in the "AI Agents for Beginners" course.
2. **AI/ML Interview Prep**: A prioritized, tier-based study plan covering **all 18 public repositories** under `GowthamKaravadi`, tailored to Senior AI/ML Engineer interview preparation and mapped directly to real-world job requirements.

---

## Part A — Repository Analysis for Interview Preparation

### A.1 Public Repositories Under `GowthamKaravadi`

> **Scope**: All 18 confirmed public repositories (including forks) as of April 29, 2026. Private repositories, if any, are not included.

| # | Repository | Type | Purpose | Main Technologies | AI/ML Areas | Study Priority |
|---|-----------|------|---------|-------------------|-------------|---------------|
| 1 | **ai-agents-for-beginners** | Fork | Structured 16-lesson course: production-grade AI agents end-to-end | Python 3.12, Jupyter, Azure AI Foundry, MAF, MCP, A2A | GenAI, Agents, RAG, Multi-Agent, MLOps, Agentic Protocols | 🔴 Tier 1 |
| 2 | **Made-With-ML** | Fork | Learn to develop, deploy, and iterate on production-grade ML apps | Python, FastAPI, Docker, CI/CD, MLOps tooling | MLOps, Production ML, Model Serving, Data Engineering | 🔴 Tier 1 |
| 3 | **RAG_Techniques** | Fork | Advanced techniques for Retrieval-Augmented Generation systems | Python, Jupyter, vector DBs, LLMs | Advanced RAG, Hybrid Search, Query Transformation, Re-ranking | 🔴 Tier 1 |
| 4 | **Hands-On-Large-Language-Models** | Fork | Official code for O'Reilly "Hands-On Large Language Models" | Python, Jupyter, Transformers, OpenAI API | LLMs, Embeddings, Fine-tuning, Text Classification, Semantic Search | 🔴 Tier 1 |
| 5 | **Prompt-Engineering-Guide** | Fork | Comprehensive guides, papers, and notebooks on prompt engineering, RAG, and AI agents | Markdown, Python, Jupyter | Prompt Engineering, Context Engineering, RAG, AI Agents | 🔴 Tier 1 |
| 6 | **GenAI_Agents** | Fork | Tutorials and implementations for GenAI agent techniques (basic to advanced) | Python, Jupyter, LangChain, OpenAI | GenAI Agents, Tool Use, Memory, Multi-Agent Systems | 🟡 Tier 2 |
| 7 | **nn-zero-to-hero** | Fork | Neural Networks: Zero to Hero (Andrej Karpathy course) | Python, Jupyter, PyTorch | Neural Networks, Backprop, Transformers, Tokenization, GPT from scratch | 🟡 Tier 2 |
| 8 | **annotated_deep_learning_paper_implementations** | Fork | 60+ annotated DL paper implementations with side-by-side notes | Python, PyTorch, Jupyter | Transformers, GANs, RL (PPO, DQN), Optimizers (Adam), Capsule Nets | 🟡 Tier 2 |
| 9 | **mml-book.github.io** | Fork | Companion webpage and notebooks for "Mathematics for Machine Learning" | Python, Jupyter | Linear Algebra, Probability, Optimization, Regression — ML foundations | 🟡 Tier 2 |
| 10 | **awesome-nlp** | Fork | Curated NLP resource list (papers, tools, datasets, courses) | Markdown | NLP, Text Classification, NER, Translation, Transformers, LLMs | 🟡 Tier 2 |
| 11 | **ML-For-Beginners** | Fork | 12-week, 26-lesson classic ML curriculum with quizzes | Python, Jupyter, Scikit-learn | Classic ML, Regression, Classification, Clustering, NLP, Time Series | 🟢 Tier 3 |
| 12 | **100-Days-Of-ML-Code** | Fork | Structured 100-day ML coding curriculum | Python, Jupyter | ML algorithms, Data Preprocessing, Scikit-learn, Deep Learning intro | 🟢 Tier 3 |
| 13 | **Python** | Fork | Algorithms implemented in Python (The Algorithms project) | Python | Data Structures, Algorithms, Sorting, Graphs — coding interview prep | 🟢 Tier 3 |
| 14 | **awesome-datascience** | Fork | Curated Data Science resources (tools, books, papers, tutorials) | Markdown | Data Science, Statistics, EDA, Feature Engineering, Visualization | 🟢 Tier 3 |
| 15 | **everything-claude-code** | Fork | Agent harness performance optimization: skills, memory, and security for Claude Code and Codex | Markdown, Shell | Agentic tooling, Prompt engineering, Developer productivity with AI | 🟢 Tier 3 |
| 16 | **awesome-rl** | Fork | Curated Reinforcement Learning resources | Markdown | RL fundamentals, Model-Free RL, Policy Gradients, Deep RL | 🟢 Tier 3 |
| 17 | **all-rl-algorithms** | Fork | Implementations of all RL algorithms in a simple, readable style | Python | Q-Learning, SARSA, DQN, PPO, DDPG, A3C, SAC | 🟢 Tier 3 |
| 18 | **Snap-Tap-Input** | Fork | Python GUI software based on Razer's Snap-Tap keyboard feature | Python, Tkinter | _(Not AI/ML — skip for interview prep)_ | ⚪ Skip |

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

### A.3 Deep-Dive: Other Repositories

#### `Made-With-ML`
**What it covers**: End-to-end production ML — from design, data, modeling, and evaluation through deployment, CI/CD, testing, and monitoring. Structured as a comprehensive MLOps course with a real-world project.
**Key topics**: Labeling, preprocessing, feature engineering, model training, experiment tracking (MLflow), model packaging (Docker), REST API (FastAPI), CI/CD (GitHub Actions), monitoring and data drift.
**Interview value**: This is the most directly applicable repo for "how would you put a model in production?" and MLOps system design questions.

#### `RAG_Techniques`
**What it covers**: 20+ advanced RAG techniques implemented as Jupyter notebooks, each with explanations, diagrams, and code.
**Key techniques**: Simple RAG, Contextual Compression, Multi-Query Retrieval, RAG Fusion, Self-Querying, Hypothetical Document Embeddings (HyDE), Re-ranking, Adaptive RAG, CRAG (Corrective RAG), Self-RAG.
**Interview value**: Lets you go beyond "I know RAG" to "I know 10 different RAG variants and when to use each."

#### `Hands-On-Large-Language-Models`
**What it covers**: O'Reilly book companion code covering LLM fundamentals through applied fine-tuning and deployment.
**Key chapters**: Text embeddings, semantic search, text classification with LLMs, fine-tuning (LoRA, QLoRA), RAG applications, LLM evaluation, building LLM-powered apps.
**Interview value**: Provides concrete runnable examples for every major LLM topic; anchors theoretical knowledge to working code.

#### `Prompt-Engineering-Guide`
**What it covers**: Comprehensive, community-maintained guide covering all prompt engineering techniques, model-specific guides, and AI agent prompting patterns.
**Key topics**: Zero-shot, few-shot, chain-of-thought (CoT), self-consistency, ReAct, Tree of Thoughts, retrieval-augmented prompting, adversarial prompting, prompt security.
**Interview value**: Demonstrates you can engineer effective prompts under constraints — directly testable via live coding or take-home exercises.

#### `GenAI_Agents`
**What it covers**: Progressive tutorials for building GenAI agents — from simple single-function agents to complex multi-agent systems with memory and planning.
**Key modules**: Basic agent setup, tool integration, retrieval-augmented agents, multi-agent orchestration, memory-enabled agents, self-correcting agents.
**Interview value**: Bridges theory from `ai-agents-for-beginners` to independent implementation patterns outside Azure.

#### `nn-zero-to-hero`
**What it covers**: Andrej Karpathy's hands-on course building neural networks from scratch — from basic micrograd autograd engine to a GPT character-level language model.
**Key notebooks**: `micrograd` (autograd from scratch), `makemore` (bigram → MLP → RNN → Transformer), `nanoGPT` (GPT-2-scale training).
**Interview value**: Interviewers at top companies frequently ask about backpropagation, gradient flow, and attention mechanism internals — this repo builds that intuition.

#### `annotated_deep_learning_paper_implementations`
**What it covers**: 60+ deep learning paper re-implementations with line-by-line annotations, covering transformers, GANs, optimizers, and RL.
**Key implementations**: Original Transformer, ViT, GPT, Switch Transformer, DDPM (diffusion), StyleGAN2, Adam/AdaBelief/Sophia optimizers, PPO, DQN, capsule networks, knowledge distillation.
**Interview value**: Useful for demonstrating research-level comprehension and for answering questions about specific architectures or "can you explain how Adam works internally?"

#### `mml-book.github.io`
**What it covers**: Companion material for "Mathematics for Machine Learning" — covering the mathematical prerequisites for understanding modern ML.
**Key chapters**: Linear algebra (Ch. 2), analytic geometry (Ch. 3), matrix decompositions / SVD / PCA (Ch. 4), probability & distributions (Ch. 6), optimization (Ch. 7), regression (Ch. 9), dimensionality reduction (Ch. 10), density estimation (Ch. 11).
**Interview value**: Mathematical foundations are tested in senior ML interviews ("derive the closed-form solution for linear regression", "explain PCA geometrically", "what happens to gradient flow in deep networks").

#### `awesome-nlp`
**What it covers**: Community-curated reading list for NLP — covering research papers, libraries, tools, datasets, and tutorials across all NLP subfields.
**Key sections**: Language models, question answering, summarization, NER, machine translation, dialogue systems, evaluation, LLMs.
**Interview value**: Acts as a map for NLP breadth — useful for "what are you aware of in NLP?" questions and for identifying gaps before a focused interview.

#### `ML-For-Beginners`
**What it covers**: Microsoft's 12-week, 26-lesson classic ML course with Scikit-learn — regression, classification, clustering, NLP, time series, reinforcement learning basics.
**Interview value**: Good for ensuring fundamentals are solid (bias/variance, confusion matrix, cross-validation, feature scaling) before focusing on deep learning and GenAI.

#### `100-Days-Of-ML-Code`
**What it covers**: 100-day structured ML curriculum with roadmaps, visual infographics, and code for supervised/unsupervised/deep learning.
**Interview value**: Quick-reference infographics for algorithms (SVM, random forest, PCA, k-means) — useful for rapid review before coding rounds.

#### `Python` (The Algorithms)
**What it covers**: Clean Python implementations of standard computer science algorithms — sorting, searching, dynamic programming, graphs, trees, mathematical algorithms, machine learning basics.
**Interview value**: Direct prep for coding interview rounds (often LeetCode-style in Python) — use to refresh DSA before behavioral/technical screens.

#### `awesome-datascience`
**What it covers**: Curated resources for the full data science workflow — statistics, EDA, feature engineering, visualization, and ML pipelines.
**Interview value**: Breadth coverage for "data science" interview rounds common at companies that blend DS and ML engineering roles.

#### `everything-claude-code`
**What it covers**: Advanced agentic tooling harness covering skills, instincts, memory, security patterns, and research-first development for AI coding agents.
**Interview value**: Useful for demonstrating awareness of cutting-edge agentic tooling architecture and AI safety/security patterns in autonomous code agents.

#### `awesome-rl` and `all-rl-algorithms`
**What they cover**: Curated resources (`awesome-rl`) and clean Python implementations (`all-rl-algorithms`) for all major RL algorithms.
**Interview value**: Study only if RL is expected in the role (robotics, recommendation systems, game AI). For most Senior AI/ML/GenAI roles, RL is a lower priority.

---

> **Scope**: All 18 public repositories under `GowthamKaravadi` have been analyzed. `Snap-Tap-Input` is excluded as it is unrelated to AI/ML.
> **Mapping to Job Requirements**: Tiers are ordered by observed frequency and weight in Senior AI/ML Engineer job postings and interview reports (LinkedIn, Naukri, 2025–2026). This is based on observed trends rather than exhaustive data and may vary by company.

---

### 🔴 Tier 1 — Must-Study (Maximum ROI per Hour)

These repositories and lessons map directly to the **most common Senior AI/ML interview topics**: GenAI architecture, RAG, production deployment, system design, and agent orchestration.

#### Tier 1A — Repositories

| Priority | Repository | What to Study | Interview Topic Mapped | Est. Time |
|----------|-----------|---------------|------------------------|-----------|
| **1** | **ai-agents-for-beginners** | Lessons 01, 04, 05, 08, 10, 11 (see Tier 1B below and Part C for detailed reading plans) | GenAI fundamentals, RAG, tool use, multi-agent design, MLOps, protocols | 10–15 hr |
| **2** | **Made-With-ML** | `notebooks/` — production ML lifecycle; `README.md` for MLOps architecture | End-to-end ML deployment, CI/CD for ML, model serving, monitoring | 6–8 hr |
| **3** | **RAG_Techniques** | All notebooks; focus on hybrid search, re-ranking, query transformation, self-querying | Advanced RAG patterns, vector databases, chunking strategies, evaluation | 4–6 hr |
| **4** | **Hands-On-Large-Language-Models** | Ch. 2–5 (embeddings, text classification, semantic search), Ch. 9 (fine-tuning), Ch. 10–11 (LLM apps) | LLM fundamentals, embeddings, fine-tuning, LLM-powered applications | 6–8 hr |
| **5** | **Prompt-Engineering-Guide** | `guides/` — zero-shot, few-shot, CoT, ReAct, RAG; `notebooks/` | Prompt engineering techniques, context engineering, RAG design, agent prompting | 4–5 hr |

**Why Tier 1?**
- RAG is one of the most-asked GenAI topics in 2025–2026 interviews; `RAG_Techniques` gives hands-on depth.
- `Made-With-ML` is the gold standard for "how do you productionize an ML model?" questions.
- LLM fundamentals from `Hands-On-Large-Language-Models` underpin every GenAI question.
- Prompt engineering (`Prompt-Engineering-Guide`) is directly testable in take-home and live coding rounds.
- `ai-agents-for-beginners` uniquely covers agentic protocols (MCP, A2A) and production observability that are now expected at senior levels.

#### Tier 1B — Key Lessons Within `ai-agents-for-beginners`

| Priority | Lesson | Interview Topic Mapped | Time Estimate |
|----------|--------|------------------------|---------------|
| **1** | **Lesson 01** — Intro to AI Agents | GenAI fundamentals, agent types, use cases | 1–2 hr |
| **2** | **Lesson 05** — Agentic RAG | RAG architecture, iterative retrieval, self-correction, NL2SQL | 2–3 hr |
| **3** | **Lesson 10** — AI Agents in Production | MLOps, observability (traces/spans), evaluation (offline/online), cost management | 2–3 hr |
| **4** | **Lesson 08** — Multi-Agent Systems | System design, agent coordination, fault tolerance, scalability | 2 hr |
| **5** | **Lesson 04** — Tool Use Design Pattern | Function calling, schema design, LLM↔tool integration | 1–2 hr |
| **6** | **Lesson 11** — Agentic Protocols (MCP, A2A, NLWeb) | Standardized agent communication, interoperability, enterprise integration | 1–2 hr |

---

### 🟡 Tier 2 — Important (Depth After Tier 1)

These repositories and lessons deepen your understanding of neural network internals, NLP, DL paper implementations, and mathematical foundations — common in behavioral, design, and deep-dive technical rounds.

#### Tier 2A — Repositories

| Priority | Repository | What to Study | Interview Topic Mapped | Est. Time |
|----------|-----------|---------------|------------------------|-----------|
| **6** | **GenAI_Agents** | All tutorials in order (basic → advanced); focus on memory and multi-agent notebooks | GenAI agent patterns, tool integration, agent memory, multi-step reasoning | 4–5 hr |
| **7** | **nn-zero-to-hero** | All 6 Jupyter notebooks (micrograd → GPT); prioritize `makemore` and `nanoGPT` | Neural net internals, backprop, attention, tokenization, GPT architecture | 8–10 hr |
| **8** | **annotated_deep_learning_paper_implementations** | Transformers (original + ViT), optimizers (Adam), PPO, DQN | Research paper comprehension, transformer architecture deep-dive, RL | 5–8 hr |
| **9** | **mml-book.github.io** | Ch. 2 (linear algebra), Ch. 5 (optimization), Ch. 9–11 (regression, dimensionality reduction, density estimation) | ML mathematical foundations, PCA, optimization, probability | 5–7 hr |
| **10** | **awesome-nlp** | Curated reading: Transformers section, LLM section, named entity recognition, summarization | NLP taxonomy, state-of-the-art models, evaluation metrics | 2–3 hr (skim) |

#### Tier 2B — Key Lessons Within `ai-agents-for-beginners`

| Priority | Lesson | Interview Topic Mapped | Time Estimate |
|----------|--------|------------------------|---------------|
| **7** | **Lesson 02** — Agentic Frameworks | Framework comparison (AutoGen, LangChain, Semantic Kernel, MAF), design trade-offs | 2 hr |
| **8** | **Lesson 07** — Planning Design | Task decomposition, iterative re-planning, agentic workflows | 1–2 hr |
| **9** | **Lesson 06** — Trustworthy AI Agents | Responsible AI, safety guardrails, PII, prompt injection, bias | 1–2 hr |
| **10** | **Lesson 14** — Microsoft Agent Framework | Middleware, workflows, checkpointing, orchestration patterns | 2 hr |
| **11** | **Lesson 09** — Metacognition | Self-reflection, self-correction, reflexion patterns | 1 hr |
| **12** | **Lesson 13** — Agent Memory | Memory architectures (short-term, long-term, episodic, semantic) | 1 hr |

**Why Tier 2?**
- `nn-zero-to-hero` (Karpathy) is widely regarded as the best resource for understanding why LLMs work — a must for senior deep-dive questions.
- Annotated paper implementations provide evidence of research-level understanding.
- Math foundations (`mml-book`) underpin questions about optimization, regularization, and loss surface.
- Framework comparison is a standard "why did you choose X over Y?" question.
- Trustworthy AI is mandatory at FAANG/enterprise companies (safety reviews, bias audits).

---

### 🟢 Tier 3 — Nice to Have (Skim for Breadth)

These resources add breadth, fill in classic ML gaps, and handle niche or specialization questions.

#### Tier 3A — Repositories

| Priority | Repository | What to Study | Interview Topic Mapped | Est. Time |
|----------|-----------|---------------|------------------------|-----------|
| **11** | **ML-For-Beginners** | Weeks 4–8 (ML algorithms), Week 11 (NLP), Week 12 (time series) — skip weeks 1–3 if you know the basics | Classic ML: regression, classification, clustering, NLP, time series | 3–4 hr (skim) |
| **12** | **100-Days-Of-ML-Code** | Day 1–30: supervised learning infographics; Day 60–90: unsupervised and deep learning | ML fundamentals refresher, visual learning aids | 2–3 hr (skim) |
| **13** | **Python** | Searching, sorting, graph algorithms, dynamic programming sections | Coding interview preparation (data structures & algorithms in Python) | 2–3 hr |
| **14** | **awesome-datascience** | Curated reading list: statistics, feature engineering, visualization tools | Data science interview breadth, EDA techniques | 1–2 hr (skim) |
| **15** | **everything-claude-code** | `SKILLS.md`, `MEMORY.md`, `SECURITY.md` — agentic tool patterns and safety | Advanced agentic tooling, agent memory and security architecture | 1 hr |
| **16** | **awesome-rl** | RL fundamentals section, model-free RL, deep RL references | RL concepts if asked (less common for non-RL senior roles) | 1 hr (skim) |
| **17** | **all-rl-algorithms** | `dqn.py`, `ppo.py`, `ddpg.py` — read implementations for DQN and PPO | RL algorithm internals, if RL interview expected | 2–3 hr |

#### Tier 3B — Remaining Lessons Within `ai-agents-for-beginners`

| Priority | Lesson | Interview Topic Mapped | Time Estimate |
|----------|--------|------------------------|---------------|
| **13** | **Lesson 03** — Agentic Design Principles | UX principles for agents, human-in-the-loop design | 0.5–1 hr |
| **14** | **Lesson 12** — Context Engineering | Prompt engineering at scale, context window management | 1 hr |
| **15** | **Lesson 15** — Browser Use Agents | Web automation, emerging agent capabilities | 0.5 hr |
| **16** | **Lesson 00** — Course Setup | Environment setup; only needed for hands-on coding | 0.5 hr |

---

### ⏱ Total Time Estimates by Tier

| Tier | Scope | Estimated Time |
|------|-------|---------------|
| 🔴 Tier 1 (5 repos + 6 lessons) | `ai-agents-for-beginners` top lessons, `Made-With-ML`, `RAG_Techniques`, `Hands-On-LLMs`, `Prompt-Engineering-Guide` | **33–43 hr** |
| 🟡 Tier 2 (5 repos + 6 lessons) | `GenAI_Agents`, `nn-zero-to-hero`, annotated DL, `mml-book`, `awesome-nlp`, remaining top lessons | **26–35 hr** |
| 🟢 Tier 3 (7 repos + 4 lessons) | Classic ML, algorithms, data science, RL, remaining lessons | **12–18 hr** (skim) |
| **Total** | All 17 AI/ML repos | **~70–100 hr** |

> **Recommended 2-week sprint**: Do all of Tier 1 in week 1 (daily 4–6 hr), and the highest-priority Tier 2 items (nn-zero-to-hero + GenAI_Agents + key `ai-agents-for-beginners` lessons) in week 2.

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
