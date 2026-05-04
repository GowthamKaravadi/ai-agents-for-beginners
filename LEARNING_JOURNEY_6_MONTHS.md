# 6-Month Learning Journey — Wells Fargo Senior AI Engineer

> **Role**: Senior AI Engineer · Wells Fargo · Bengaluru, Karnataka, India  
> **Stack**: Python · FastAPI · Docker · GitHub Actions · Neo4j · Vector DBs · LLMs · RAG · MCP · Agents  
> **Repo used as study base**: [`microsoft/ai-agents-for-beginners`](https://github.com/microsoft/ai-agents-for-beginners)

---

## Table of Contents
1. [JD Requirements Breakdown](#1-jd-requirements-breakdown)
2. [Is 6 Months Enough?](#2-is-6-months-enough)
3. [Week-by-Week 24-Week Plan](#3-week-by-week-24-week-plan)
4. [Skills → JD Requirements Map](#4-skills--jd-requirements-map)
5. [Portfolio Projects](#5-portfolio-projects)
6. [Suggested Resources](#6-suggested-resources)
7. [Interview Preparation Checklist](#7-interview-preparation-checklist)

---

## 1. JD Requirements Breakdown

### Role: Senior AI Engineer — Wells Fargo (Bengaluru, India)

#### What You Will Do (Responsibilities)

| Domain | Key Responsibilities |
|--------|---------------------|
| **AI / LLM / Agent Dev** | Build & deploy LLM-powered apps (commercial + OSS models); design & implement RAG pipelines; create AI agents that reason over structured (graph) and unstructured data; define tool-use patterns (function calling, API tools, memory tools); apply strong prompt engineering for reliability, safety, performance |
| **Graph, Vector & NLP** | Design & manage knowledge graphs using **Neo4j**; model complex relationships & optimize **Cypher** queries; implement semantic search using **vector databases**; apply NLP concepts: embeddings, entity extraction, classification, summarization, similarity search |
| **MCP & AI Platform** | Set up & operate **Model Context Protocol (MCP)** servers; register datasets, APIs & tools for secure LLM access; enable scalable, observable, governed LLM interactions |
| **Python / APIs / Backend** | Build AI microservices using Python (**FastAPI / Flask**); integrate & consume internal/external APIs within AI workflows; develop pipelines for ingestion, embedding generation, indexing & retrieval |
| **Model Evaluation & Optimization** | Evaluate LLM & NLP models (qualitative + quantitative); measure & monitor performance (accuracy, latency, cost, hallucinations); continuously iterate on prompts, retrieval strategies & model configurations |

#### Required Qualifications
- **6+ years** of AI Engineering experience (or equivalent through training/education)

#### Desired Qualifications
- Strong Python; experience with Spark/Scala
- Deep Learning frameworks: PyTorch, TensorFlow (or equivalent)
- NLP concepts & modern language modeling
- Practical LLMs, prompt engineering, agent-based systems
- Hands-on **Neo4j** or other graph DBs
- **Vector databases** for similarity search and embeddings
- **MCP** server setup or LLM tool orchestration frameworks
- REST APIs, function calling, tool integrations
- Model evaluation & monitoring techniques
- Git and CI/CD pipelines

#### Nice-to-Have
- LangChain, LlamaIndex, Semantic Kernel
- Cloud: **Azure** preferred; AWS/GCP welcome
- **Docker** and Kubernetes
- Knowledge graphs, ontologies, semantic systems
- AI governance, security, responsible AI practices

#### Job Expectations
- Bachelor's/Master's in CS, Engineering, AI/ML or related
- Experience delivering enterprise-scale AI or data platforms

---

## 2. Is 6 Months Enough?

### Short Answer

| Weekly Hours | Verdict | Notes |
|---|---|---|
| **6 hrs/week** | ⚠️ Unlikely | You'll cover ~50% of skills; strong for junior roles, but gaps will show at senior-level interviews |
| **10 hrs/week** | ✅ Possible | You can cover all core skills and build 2 portfolio projects; expect interview-readiness for mid → senior transition |
| **15+ hrs/week** | ✅ Yes | Enough to deeply learn all skills, build polished projects with tests + CI, and practice mock interviews |

### Why the JD Is Challenging

The Wells Fargo role explicitly requires **6+ years of experience**. This means:
- They expect **depth in multiple areas simultaneously**: RAG, Neo4j, vector DBs, MCP, FastAPI, evals — not surface-level knowledge
- Enterprise-scale means they will probe system design (latency, fault tolerance, cost, governance)
- Responsible AI / governance awareness is a differentiator

### 6-Month Realistic Expectations

| Scenario | What 6 months gets you |
|---|---|
| Starting from Python intermediate, no AI | Ready for **mid-level** AI engineer roles; strong portfolio; may need 3–6 more months for senior |
| Starting from Python advanced + some ML | Ready for **senior-level** AI roles if you build & present solid projects; 6 months is sufficient |
| Starting from strong AI/backend background | Use 6 months to specialise: Neo4j, MCP, evals, RAG — directly targeting this JD |

> **Bottom line**: 6 months at **10–15 hrs/week** is sufficient to become a **competitive candidate** for this role, especially if you can demonstrate 2–3 well-documented projects covering the key JD areas.

---

## 3. Week-by-Week 24-Week Plan

### Overview

| Month | Focus | Outcome |
|---|---|---|
| 1 (Weeks 1–4) | Python + Backend + Tooling Foundation | Clean FastAPI microservice with tests, Docker, CI |
| 2 (Weeks 5–8) | LLM Fundamentals + Prompt Engineering | Prompt harness, eval pipeline, function calling |
| 3 (Weeks 9–12) | Agent Architecture + RAG | Agentic RAG service with tool use and vector DB |
| 4 (Weeks 13–16) | Graph Systems: Neo4j + Knowledge Graphs | Graph-powered agent with Cypher queries and embeddings |
| 5 (Weeks 17–20) | MCP + Platform Engineering + Production | MCP server, observability, Docker/CI/CD pipeline |
| 6 (Weeks 21–24) | Capstone Projects + Interview Prep | Polished portfolio + mock interview readiness |

---

### Month 1 — Python, Backend & Engineering Foundation (Weeks 1–4)

> **Goal**: Build the engineering discipline needed for a Senior role — clean code, tests, CI/CD, containerization.

#### Week 1 — Python Mastery & Code Quality
- **Learn**: Python typing, dataclasses, Pydantic v2, exceptions, generators, context managers
- **Learn**: Black, Ruff, pre-commit hooks, `.editorconfig`
- **Practice**: Refactor a messy Python script into a typed, tested module
- **Deliverable**: A typed Python utility library with full `pytest` coverage (≥90%)
- **Measurable**: `pytest --cov` shows ≥90%; `ruff` and `black` pass with 0 errors

#### Week 2 — FastAPI Microservice
- **Learn**: FastAPI routing, Pydantic request/response models, dependency injection, middleware
- **Learn**: Async/await in Python, `httpx` for async HTTP clients
- **Practice**: Build a "Task Runner" REST API — create tasks, poll status, fetch results
- **Repo lessons**: Study `11-agentic-protocols/` to understand microservice architecture for agents
- **Deliverable**: FastAPI service with `/tasks`, `/tasks/{id}`, `/health` endpoints
- **Measurable**: 100% of endpoints tested with `pytest` + `httpx`; OpenAPI docs auto-generated

#### Week 3 — Docker + PostgreSQL + GitHub Actions
- **Learn**: Dockerfile, multi-stage builds, `docker-compose` for local dev
- **Learn**: PostgreSQL basics, SQLAlchemy (async), Alembic migrations
- **Learn**: GitHub Actions — CI workflow: lint → test → build Docker image
- **Practice**: Add PostgreSQL persistence to your Week 2 FastAPI service
- **Deliverable**: Dockerized FastAPI + Postgres service; GitHub Actions CI runs on every PR
- **Measurable**: `docker-compose up` brings up all services; CI passes on push; DB migrations run cleanly

#### Week 4 — Testing Discipline & Code Review Habits
- **Learn**: `pytest` fixtures, mocking (`unittest.mock`, `respx`), parametrize
- **Learn**: Integration tests vs unit tests; test coverage strategies
- **Practice**: Add integration tests that test the full request-to-DB flow
- **Practice**: Write a PR, review your own diff, iterate
- **Deliverable**: ≥85% branch coverage; integration tests that spin up Docker services
- **Measurable**: `pytest -m integration` passes; `pytest --cov --cov-report=html` shows ≥85% branch coverage

---

### Month 2 — LLM Fundamentals + Prompt Engineering (Weeks 5–8)

> **Goal**: Understand how LLMs work, how to prompt them reliably, how to evaluate them quantitatively.

#### Week 5 — LLM APIs + Function Calling
- **Learn**: OpenAI / Azure OpenAI API; rate limits, retries, cost estimation
- **Learn**: Function calling / tool use (JSON schema → LLM → execute → return result)
- **Practice**: Build a "function calling playground" — register 5 custom tools, test LLM routing
- **Repo lessons**: `04-tool-use/` — complete all code samples in `04-python-agent-framework.ipynb`
- **Deliverable**: Python module with `@tool` decorated functions + test cases for each tool call
- **Measurable**: Each tool is invoked correctly by the LLM; schema validation passes; errors are handled gracefully

#### Week 6 — Prompt Engineering Patterns
- **Learn**: System prompts, chain-of-thought, few-shot examples, ReAct, JSON output guardrails
- **Learn**: Structured output with Pydantic + `response_format`
- **Practice**: Build a prompt template library with versioned prompts (store in files, not strings)
- **Practice**: Test prompts like code: assert on output structure, tone, required fields
- **Repo lessons**: `12-context-engineering/` — study context window management
- **Deliverable**: A prompt library with ≥10 versioned prompts; pytest suite asserting output structure
- **Measurable**: 0 hallucinated fields in structured output tests; prompts stored as YAML templates

#### Week 7 — LLM Evaluation Framework
- **Learn**: Offline evaluation (golden datasets, regression tests); online evaluation (sampling, dashboards)
- **Learn**: RAGAS metrics (faithfulness, answer relevancy, context precision/recall)
- **Learn**: LLM-as-judge pattern for qualitative evaluation
- **Practice**: Create a golden test set of 20 prompt→expected output pairs; run automated eval
- **Repo lessons**: `10-ai-agents-production/` — study the evaluation and observability sections
- **Deliverable**: Eval harness that runs nightly, produces a JSON report of pass/fail + RAGAS scores
- **Measurable**: Baseline eval scores recorded; regression detected if score drops >5%

#### Week 8 — Observability & Structured Logging
- **Learn**: OpenTelemetry Python SDK; traces, spans, metrics; structured JSON logging
- **Learn**: Langfuse or Azure AI Foundry traces for LLM observability
- **Practice**: Instrument your Week 5 function calling code with trace/span context
- **Deliverable**: Every LLM call produces a trace with: model, prompt tokens, completion tokens, latency, tool calls used
- **Measurable**: Langfuse dashboard (or equivalent) shows traces; alerts fire if p99 latency >5s

---

### Month 3 — Agent Architecture + RAG (Weeks 9–12)

> **Goal**: Build production-grade agentic RAG — the single most-tested skill in this JD.

#### Week 9 — Vector Databases + Embeddings
- **Learn**: Embedding models (OpenAI `text-embedding-3-small`, sentence-transformers)
- **Learn**: Vector databases: Chroma (local), pgvector (Postgres), or Azure AI Search
- **Learn**: Chunking strategies (sentence, paragraph, semantic); overlap; metadata filtering
- **Practice**: Ingest a set of 50+ documents; build a semantic search endpoint
- **Repo lessons**: `05-agentic-rag/` — study chunking and retrieval patterns
- **Deliverable**: FastAPI `/search` endpoint returning top-k results with similarity scores + source citations
- **Measurable**: Retrieval precision ≥0.80 on a 10-query golden set; p95 latency ≤500ms

#### Week 10 — Basic RAG Pipeline
- **Learn**: Classic RAG: retrieve → augment → generate; citation tracking; hallucination reduction
- **Learn**: Re-ranking (cross-encoder, MMR); hybrid search (BM25 + vector)
- **Practice**: Build a document Q&A service over your Week 9 vector store
- **Repo lessons**: `05-agentic-rag/code_samples/` — run the full notebook
- **Deliverable**: Q&A endpoint returning answer + ranked citations + confidence score
- **Measurable**: Faithfulness ≥0.85 on RAGAS eval; answers include source references

#### Week 11 — Agentic RAG (Iterative Retrieval)
- **Learn**: Agentic RAG loop: query → retrieve → evaluate → re-query if needed → synthesize
- **Learn**: Self-correction patterns; sub-query decomposition; iterative refinement
- **Practice**: Extend Week 10 pipeline to retry retrieval when confidence is low
- **Repo lessons**: `09-metacognition/` — study self-correction and reflexion patterns
- **Deliverable**: Agent that performs up to 3 retrieval iterations; logs reasoning at each step
- **Measurable**: Answer quality improves by ≥10% vs baseline single-retrieval on hard queries

#### Week 12 — Multi-Source RAG + NLP Preprocessing
- **Learn**: NLP concepts: entity extraction (spaCy / Azure Text Analytics), classification, summarization
- **Learn**: Ingesting from multiple sources: PDFs, web pages, databases; pipeline orchestration
- **Practice**: Add entity extraction step to enrich chunk metadata before indexing
- **Repo lessons**: `08-multi-agent/` — study coordination patterns for multi-source retrieval
- **Deliverable**: Ingestion pipeline supporting 3+ source types; entity-enriched chunks in vector store
- **Measurable**: Entity extraction runs for all chunks; filtered searches by entity return correct results

---

### Month 4 — Graph Systems: Neo4j + Knowledge Graphs (Weeks 13–16)

> **Goal**: Master the Neo4j + Cypher skills that are explicitly called out in this JD and rare in the market.

#### Week 13 — Neo4j Fundamentals + Cypher
- **Learn**: Neo4j data model (nodes, relationships, properties); Cypher query language
- **Learn**: `MATCH`, `CREATE`, `MERGE`, `WHERE`, `WITH`, `RETURN`; path queries; aggregation
- **Practice**: Install Neo4j Desktop (or AuraDB free); model a small knowledge graph (e.g., a company's product catalog with entities and relationships)
- **Resources**: [Neo4j Fundamentals](https://graphacademy.neo4j.com/courses/neo4j-fundamentals/), [Cypher Basics](https://graphacademy.neo4j.com/courses/cypher-fundamentals/)
- **Deliverable**: Knowledge graph with ≥5 node types, ≥8 relationship types, ≥200 nodes; 10 Cypher queries documented
- **Measurable**: All queries run in <100ms on local dataset; complex path queries return correct results

#### Week 14 — Graph-Enhanced RAG
- **Learn**: Combining vector search + graph traversal for richer context (GraphRAG)
- **Learn**: Entity linking (map extracted entities to graph nodes); relationship-aware retrieval
- **Practice**: Build a "Graph + Vector" retrieval pipeline: extract entities from query → traverse graph → fetch relevant chunks → generate answer
- **Repo lessons**: `05-agentic-rag/` — adapt the retrieval pattern to include graph context
- **Deliverable**: Hybrid retrieval endpoint that fetches both semantic chunks and graph-context paths
- **Measurable**: Answers to relationship-heavy questions improve vs pure vector RAG (≥15% quality gain on test set)

#### Week 15 — Knowledge Graph Construction Pipeline
- **Learn**: Automated KG construction: NER → entity resolution → relation extraction → graph population
- **Learn**: Ontology design; schema-free vs schema-based graphs
- **Practice**: Build a pipeline that reads documents, extracts entities + relationships, and populates Neo4j automatically
- **Deliverable**: Automated KG construction pipeline; Python script with `neo4j` driver; Cypher-based validation queries
- **Measurable**: Processing 100 documents produces a connected graph; precision of extracted relations ≥0.75

#### Week 16 — Graph Performance + Cypher Optimization
- **Learn**: Neo4j indexes, constraints, execution plans (`EXPLAIN`, `PROFILE`)
- **Learn**: Graph algorithms: shortest path, community detection, centrality (via GDS library)
- **Practice**: Optimize your Week 13–15 queries; add indexes on frequently queried properties
- **Deliverable**: Index-optimized Cypher queries; query latency reduced by ≥50% after optimization
- **Measurable**: `PROFILE` shows index usage; p95 query latency ≤50ms on dataset of 10K nodes

---

### Month 5 — MCP + Platform Engineering + Production (Weeks 17–20)

> **Goal**: Build and deploy a production-grade AI platform with MCP, observability, and CI/CD.

#### Week 17 — Model Context Protocol (MCP)
- **Learn**: MCP architecture: Hosts, Clients, Servers; core primitives: Tools, Resources, Prompts
- **Learn**: Building an MCP server in Python (`mcp[cli]` SDK); registering tools and resources
- **Practice**: Build an MCP server that exposes: (1) vector search tool, (2) Neo4j query tool, (3) document retrieval resource
- **Repo lessons**: `11-agentic-protocols/` — complete MCP section; study how the course registers tools
- **Deliverable**: Running MCP server with ≥3 tools; tested with `mcp` CLI inspector
- **Measurable**: Tools discovered and called correctly via MCP protocol; input/output schemas validated

#### Week 18 — Secure LLM Access + Tool Orchestration
- **Learn**: Secret management (env vars, Azure Key Vault); API key rotation; input validation against prompt injection
- **Learn**: Tool orchestration patterns: sequential, parallel, conditional tool chains
- **Practice**: Wrap your MCP tools with auth middleware; add rate limiting; add input sanitization
- **Repo lessons**: `06-building-trustworthy-agents/` — study safety and governance patterns
- **Deliverable**: MCP server with auth token validation; rate limiting (100 req/min); prompt injection guard
- **Measurable**: Unauthorized requests return 401; injected prompts are rejected; rate limit triggers correctly

#### Week 19 — Production Deployment: Docker + GitHub Actions
- **Learn**: Multi-stage Dockerfiles for Python services; health checks; graceful shutdown
- **Learn**: GitHub Actions: matrix builds, Docker image push to GHCR/ACR, deployment workflows
- **Learn**: Environment promotion: dev → staging → prod; feature flags basics
- **Practice**: Deploy your RAG + MCP service stack with `docker-compose`; add a full CI/CD pipeline
- **Deliverable**: `docker-compose.yml` for local; GitHub Actions workflow: test → build → push → deploy
- **Measurable**: Full CI runs in <10 min; Docker image size <500MB; health check passes after deploy

#### Week 20 — Observability + Model Monitoring Dashboard
- **Learn**: Production metrics: p50/p95/p99 latency, error rate, token cost/request, hallucination rate
- **Learn**: Alerting: Prometheus + Grafana (or Azure Monitor); log aggregation (Azure Log Analytics)
- **Practice**: Add metrics instrumentation to all LLM calls; build a simple Grafana dashboard (or equivalent)
- **Repo lessons**: `10-ai-agents-production/` — study the full production observability section
- **Deliverable**: Dashboard with: request rate, latency histogram, cost/day, error rate, eval score trend
- **Measurable**: Dashboard updates in real time; alert fires if error rate >1% over 5 min

---

### Month 6 — Capstone Projects + Interview Preparation (Weeks 21–24)

> **Goal**: Produce polished portfolio projects that directly map to the JD; prepare for technical interviews.

#### Week 21 — Capstone Project 1: Agentic RAG Microservice (finalize)
- Polish [Project 1](#project-1-enterprise-knowledge-agent-rag--graph) (see §5 below)
- Add architecture diagram (Mermaid or draw.io) to README
- Record a 3-minute demo video; add screenshots of Grafana dashboard
- Write a blog-style `ARCHITECTURE.md` explaining design decisions

#### Week 22 — Capstone Project 2: Graph-Enhanced Knowledge Agent (finalize)
- Polish [Project 2](#project-2-graph-enhanced-qa-agent-neo4j--mcp) (see §5 below)
- Document Neo4j schema, example Cypher queries, and KG construction pipeline
- Add eval results table (RAGAS scores before/after graph enrichment)

#### Week 23 — System Design Practice
- **Practice**: Design a "Financial Document Analysis Platform" (fits Wells Fargo context)
  - Components: ingestion pipeline, vector store, knowledge graph, RAG agent, evaluation, monitoring
  - Draw data flow diagram; identify failure points; discuss latency/cost/accuracy trade-offs
- **Practice**: 3 mock system design sessions (use excalidraw.com for whiteboarding)
- **Practice**: Explain your portfolio projects out loud, timing yourself (2 min overview + 5 min deep dive)

#### Week 24 — Interview Prep Sprint + Final Polish
- Run all interview checklists in §7
- Practice 10 LeetCode medium Python problems (focus on string/list/dict patterns)
- Review Wells Fargo-specific context: financial data regulations, responsible AI in banking
- Final GitHub portfolio review: clean READMEs, passing CI badges, demo links, architecture diagrams

---

## 4. Skills → JD Requirements Map

| JD Requirement | Month Covered | Week(s) | Deliverable |
|---|---|---|---|
| Build & deploy LLM-powered apps | M2 + M5 | 5, 19 | Function calling service + deployed Docker stack |
| RAG pipeline design | M3 | 9–11 | Agentic RAG microservice with evals |
| AI agents over structured + unstructured data | M3 + M4 | 11–14 | Graph + RAG agent with multi-source retrieval |
| Tool-use patterns (function calling, memory) | M2 + M5 | 5, 17 | `@tool` decorated functions + MCP server |
| Prompt engineering (reliability, safety) | M2 | 6, 8 | Versioned prompt library + guardrails |
| Neo4j + Cypher queries | M4 | 13, 16 | Knowledge graph with optimized Cypher |
| Vector databases (semantic search) | M3 | 9 | Vector DB with hybrid search + metadata filtering |
| NLP: embeddings, NER, classification | M3 | 12 | NER pipeline for chunk enrichment |
| MCP server setup | M5 | 17, 18 | Secure MCP server with 3+ tools |
| FastAPI / Flask microservices | M1 | 2, 3 | Typed FastAPI service with Docker |
| REST APIs, function calling | M1 + M2 | 2, 5 | FastAPI endpoints + OpenAI function calling |
| Model evaluation + monitoring | M2 + M5 | 7, 20 | RAGAS eval harness + Grafana dashboard |
| Git + CI/CD | M1 + M5 | 3, 19 | GitHub Actions CI/CD pipeline |
| Docker | M1 + M5 | 3, 19 | Multi-stage Dockerfile + docker-compose |
| Azure (preferred) | M5 | 18, 19 | Azure deployment (Key Vault, ACR, Monitor) |
| LangChain / LlamaIndex | M3 | 10, 11 | (Optional: use LlamaIndex for ingestion pipeline) |
| AI governance + responsible AI | M2 + M5 | 8, 18 | Prompt injection guards + rate limiting + audit logs |

---

## 5. Portfolio Projects

### Project 1: Enterprise Knowledge Agent (RAG + Graph)

> **JD Match**: RAG pipelines · Neo4j · Vector DBs · FastAPI · NLP · Evaluation · Observability

#### Overview
A production-grade knowledge retrieval system that combines vector search and a Neo4j knowledge graph to answer complex enterprise queries with source citations, confidence scores, and full observability.

#### Architecture
```
User Query
    │
    ▼
FastAPI Gateway (auth + rate limiting)
    │
    ├─► Entity Extractor (spaCy)
    │       │
    │       ▼
    │   Neo4j Graph (relationship context)
    │
    ├─► Vector Store (pgvector / Chroma)
    │       │
    │       ▼
    │   Semantic Chunks (with metadata)
    │
    ▼
LLM Synthesizer (GPT-4o / Azure OpenAI)
    │
    ├─► Answer + Citations + Confidence Score
    │
    └─► Observability (OpenTelemetry → Langfuse)
```

#### Milestones

| Milestone | Week | Acceptance Criteria |
|---|---|---|
| M1: Vector ingestion pipeline | 9 | Ingests 100+ docs; `pytest` passes for chunking, embedding, storage |
| M2: Semantic search API | 9 | `/search?q=...` returns top-5 results with scores ≤500ms p95 |
| M3: Basic RAG Q&A | 10 | `/ask` returns answer + citations; faithfulness ≥0.85 RAGAS |
| M4: Neo4j KG integration | 14 | Entity-linked graph; hybrid retrieval improves hard-question score ≥15% |
| M5: Agentic RAG loop | 11 | Agent retries retrieval up to 3× if confidence low; logged reasoning |
| M6: Evaluation harness | 7 | Nightly RAGAS eval CI step; PR fails if score drops >5% |
| M7: Production deployment | 19 | Docker + GitHub Actions CI; health check passes; OpenTelemetry traces |
| M8: Observability dashboard | 20 | Grafana/Azure Monitor: latency, cost, eval score, error rate |

#### Acceptance Criteria (Final)
- [ ] All endpoints have OpenAPI docs; no unhandled 500 errors in tests
- [ ] RAGAS faithfulness ≥ 0.85, answer relevancy ≥ 0.80 on 20-query golden set
- [ ] p95 end-to-end latency ≤ 3 seconds for typical queries
- [ ] Prompt injection attempts return safe error responses (tested with 5 adversarial inputs)
- [ ] GitHub Actions CI passes: lint + test + Docker build + eval
- [ ] README includes architecture diagram, setup instructions, and eval results table
- [ ] Code coverage ≥ 80%

#### Tech Stack
```
Python 3.12 · FastAPI · Pydantic v2 · SQLAlchemy (async)
pgvector / ChromaDB · Neo4j (Python driver)
OpenAI / Azure OpenAI · sentence-transformers · spaCy
RAGAS · OpenTelemetry · Langfuse
Docker · docker-compose · GitHub Actions
pytest · httpx · ruff · black
```

---

### Project 2: Graph-Enhanced QA Agent (Neo4j + MCP)

> **JD Match**: Neo4j · Cypher · MCP server · Tool orchestration · Agent reasoning · Responsible AI

#### Overview
An AI agent that reasons over a knowledge graph using natural language. Users ask questions in plain English; the agent generates and executes Cypher queries, retrieves graph context, and explains relationships. The agent is exposed via a Model Context Protocol (MCP) server, making it composable with other LLM tools.

#### Architecture
```
User (natural language question)
    │
    ▼
MCP Client (Claude Desktop / custom LLM host)
    │
    ▼
MCP Server (Python · mcp[cli])
    ├── Tool: graph_query(cypher) → Neo4j results
    ├── Tool: semantic_search(query) → vector chunks
    ├── Tool: summarize_path(node_a, node_b) → relationship explanation
    └── Resource: graph_schema → node types, relationship types
    │
    ▼
LLM (Azure OpenAI / GPT-4o)
    │
    ▼
Answer + Cypher query used + Graph path visualization (ASCII / JSON)
```

#### Milestones

| Milestone | Week | Acceptance Criteria |
|---|---|---|
| M1: Neo4j graph populated | 13 | ≥200 nodes, ≥8 rel types; 10 Cypher queries documented |
| M2: NL→Cypher translator | 14 | LLM generates valid Cypher for 90% of test questions |
| M3: MCP server running | 17 | MCP inspector shows 3+ tools with correct schemas |
| M4: Secure tool access | 18 | Auth token required; prompt injection test suite passes |
| M5: KG construction pipeline | 15 | Processes 50 docs → populates graph automatically |
| M6: Graph optimization | 16 | Indexes added; p95 query latency ≤50ms |
| M7: Deployed + documented | 19 | Docker image published to GHCR; README with example queries |

#### Acceptance Criteria (Final)
- [ ] MCP server passes schema validation for all tools
- [ ] NL→Cypher accuracy ≥ 85% on 20-question test set (human-judged)
- [ ] Cypher injection attacks rejected (tested with 5 adversarial inputs)
- [ ] Graph query p95 latency ≤ 100ms after index optimization
- [ ] CI pipeline runs: lint + unit tests + integration tests against Neo4j test container
- [ ] Automated KG construction pipeline: processes 50 docs without manual intervention
- [ ] README includes: schema diagram, example queries, MCP tool reference, setup instructions

#### Tech Stack
```
Python 3.12 · FastAPI · mcp[cli]
Neo4j 5.x · Python neo4j driver · GDS (Graph Data Science)
spaCy · OpenAI / Azure OpenAI
Docker (Neo4j container) · GitHub Actions
pytest · testcontainers-python · ruff · black
```

---

## 6. Suggested Resources

### Core Courses & Documentation

| Resource | Topic | Priority | Time |
|---|---|---|---|
| [ai-agents-for-beginners repo](https://github.com/microsoft/ai-agents-for-beginners) (this repo!) | Full agent curriculum | ⭐ Must | 40–60 hrs |
| [Neo4j Graph Academy — Neo4j Fundamentals](https://graphacademy.neo4j.com/courses/neo4j-fundamentals/) | Neo4j + Cypher | ⭐ Must | 4 hrs |
| [Neo4j Graph Academy — Cypher Fundamentals](https://graphacademy.neo4j.com/courses/cypher-fundamentals/) | Cypher queries | ⭐ Must | 4 hrs |
| [Neo4j Graph Academy — Using Neo4j with Python](https://graphacademy.neo4j.com/courses/app-python/) | Python + Neo4j | ⭐ Must | 6 hrs |
| [FastAPI Official Tutorial](https://fastapi.tiangolo.com/tutorial/) | FastAPI microservices | ⭐ Must | 6 hrs |
| [OpenAI Function Calling Docs](https://platform.openai.com/docs/guides/function-calling) | Tool use / function calling | ⭐ Must | 3 hrs |
| [RAGAS Documentation](https://docs.ragas.io/) | RAG evaluation | ⭐ Must | 3 hrs |
| [MCP Documentation](https://modelcontextprotocol.io/introduction) | Model Context Protocol | ⭐ Must | 4 hrs |
| [OpenTelemetry Python Docs](https://opentelemetry.io/docs/languages/python/) | Observability / tracing | High | 3 hrs |
| [Azure AI Foundry Documentation](https://learn.microsoft.com/azure/ai-foundry/) | Azure AI platform | High | 5 hrs |
| [LangChain + LlamaIndex Quickstart](https://docs.llamaindex.ai/) | Indexing + agent frameworks | Medium | 4 hrs |
| [Docker for Beginners (Play With Docker)](https://training.play-with-docker.com/) | Docker / containers | High | 5 hrs |
| [GitHub Actions — Getting Started](https://docs.github.com/en/actions/writing-workflows) | CI/CD | High | 3 hrs |
| [spaCy 101](https://spacy.io/usage/spacy-101) | NLP / NER | High | 3 hrs |
| [Prompt Engineering Guide](https://www.promptingguide.ai/) | Prompt patterns | ⭐ Must | 4 hrs |
| [Langfuse Documentation](https://langfuse.com/docs) | LLM observability | Medium | 2 hrs |

### Repo Lessons — Priority Order for This JD

| Priority | Lesson | JD Skills Covered |
|---|---|---|
| 1 | `04-tool-use/` | Function calling, tool use patterns |
| 2 | `05-agentic-rag/` | RAG pipeline, retrieval, embeddings |
| 3 | `10-ai-agents-production/` | Evaluation, observability, cost monitoring |
| 4 | `11-agentic-protocols/` | MCP server setup, tool orchestration |
| 5 | `08-multi-agent/` | Multi-agent coordination patterns |
| 6 | `06-building-trustworthy-agents/` | Safety, prompt injection, responsible AI |
| 7 | `12-context-engineering/` | Prompt engineering at scale |
| 8 | `09-metacognition/` | Self-correction, Reflexion pattern |
| 9 | `13-agent-memory/` | Memory architectures |
| 10 | `01-intro-to-ai-agents/` | Agent types, fundamentals |

### Practice Activities (Weekly)

| Activity | Frequency | Purpose |
|---|---|---|
| Run and modify repo notebooks | 3×/week | Hands-on with agent patterns |
| Write a Cypher query from scratch | Daily (Month 4) | Neo4j fluency |
| Write 1 new test | Daily | TDD habit for Senior roles |
| Read 1 LLM paper abstract | 2×/week | Awareness of recent advances |
| Contribute 1 PR to an OSS project | Monthly | Demonstrated collaboration |
| Record a 3-min walkthrough of your project | Weekly (Month 6) | Interview practice |
| Mock system design session | 2×/week (Month 6) | Interview readiness |

---

## 7. Interview Preparation Checklist

### Python & Backend

- [ ] Explain Python async/await; when to use it vs threads vs multiprocessing
- [ ] Write a FastAPI endpoint from scratch with Pydantic validation and error handling
- [ ] Explain dependency injection in FastAPI; write a `Depends()` example
- [ ] Describe SQLAlchemy async session management; explain N+1 query problem
- [ ] Explain Python `typing` module; write a fully typed function signature
- [ ] Write a `pytest` fixture with teardown for a database connection
- [ ] Explain what `__enter__` / `__exit__` do; write a context manager
- [ ] Describe how to structure a Python package (not just a script)

### LLMs & Prompt Engineering

- [ ] Explain the difference between `temperature`, `top_p`, and `max_tokens`
- [ ] Describe chain-of-thought prompting; when does it help?
- [ ] Explain JSON mode / structured output; how do you enforce output schema?
- [ ] What is a system prompt? How does it differ from a user prompt?
- [ ] Describe the ReAct pattern (Reason + Act); draw the loop diagram
- [ ] Explain prompt injection; describe 3 mitigation strategies
- [ ] How do you version prompts? How do you test them automatically?
- [ ] Explain the difference between fine-tuning and RAG; when to use each

### RAG & Vector Search

- [ ] Explain the classic RAG pipeline end-to-end (ingest → embed → store → retrieve → generate)
- [ ] What is chunking? Describe 3 chunking strategies and their trade-offs
- [ ] Explain hybrid search (BM25 + vector); when is it better than pure vector?
- [ ] What is re-ranking? Explain cross-encoder vs bi-encoder
- [ ] Describe RAGAS metrics: faithfulness, answer relevancy, context precision
- [ ] What is Agentic RAG? How does it differ from classic RAG?
- [ ] Explain how to reduce hallucinations in RAG
- [ ] Walk through an ingestion pipeline for 3 source types (PDF, web, database)

### Neo4j & Knowledge Graphs

- [ ] Explain the property graph model (nodes, relationships, properties, labels)
- [ ] Write a Cypher query to find all nodes related to a given node within 2 hops
- [ ] Explain the difference between `CREATE` and `MERGE` in Cypher
- [ ] Describe how you would design a knowledge graph for a financial domain
- [ ] Explain how to combine vector search with graph traversal (GraphRAG)
- [ ] What are Neo4j indexes? How do you check if a query uses them (`EXPLAIN`/`PROFILE`)?
- [ ] Describe 2 use cases where a graph DB outperforms a relational DB
- [ ] Explain entity resolution / disambiguation in KG construction

### MCP & Agent Architecture

- [ ] Explain MCP's 3 primitives: Tools, Resources, Prompts
- [ ] Describe the MCP client-server architecture; what is a "Host"?
- [ ] How do you register a new tool in an MCP server (Python SDK)?
- [ ] Explain tool orchestration patterns: sequential, parallel, conditional
- [ ] What is the agent loop? Draw: Observe → Think → Act → Observe
- [ ] Describe memory types in agents: short-term, long-term, episodic, semantic
- [ ] Explain how to prevent infinite loops in an agent
- [ ] Compare MCP to raw function calling; when would you use each?

### Model Evaluation & Monitoring

- [ ] What metrics do you track for an LLM in production? (latency, cost, accuracy, hallucinations)
- [ ] Explain offline vs online evaluation; describe the deploy → monitor → improve loop
- [ ] What is LLM-as-judge? What are its limitations?
- [ ] Describe how OpenTelemetry traces work for LLM applications
- [ ] How do you set up an alert for hallucination rate exceeding a threshold?
- [ ] Explain how to reduce LLM inference cost (smaller models, caching, router models)
- [ ] What is RAGAS? Name and explain 4 metrics
- [ ] How do you build a golden test set for prompt regression testing?

### System Design (Senior-Level)

- [ ] **Design a financial document analysis platform** (ingestion → KG → RAG → monitoring)
  - Must cover: multi-source ingestion, entity extraction, Neo4j population, vector search, LLM synthesis, evaluation CI, cost management, governance
- [ ] **Design a multi-tenant AI agent service** (isolation, rate limiting, cost attribution)
- [ ] **Explain your project's architecture** in 5 minutes (with whiteboard diagram)
- [ ] What are the latency bottlenecks in a RAG pipeline? How do you reduce p95 latency?
- [ ] How do you handle LLM API failures (retries, fallback models, circuit breakers)?
- [ ] Describe a blue/green or canary deployment for an LLM-powered service

### Responsible AI & Governance (Wells Fargo Context)

- [ ] What is responsible AI? Name 4 Microsoft responsible AI principles
- [ ] Describe prompt injection; give 3 real-world examples in a banking context
- [ ] How do you handle PII (Personally Identifiable Information) in LLM pipelines?
- [ ] Explain AI governance: audit logs, model cards, usage policies
- [ ] What is content filtering? How does Azure OpenAI's content safety work?
- [ ] Describe a bias audit for an NLP classifier in a financial context
- [ ] How do you document a model for compliance (model card)?
- [ ] What is the EU AI Act high-risk category, and why does banking AI fall there?

### Behavioral / Culture Fit

- [ ] Describe a time you improved a system's performance significantly — what did you measure and optimize?
- [ ] Describe a time a model failed in production — how did you detect it and respond?
- [ ] How do you stay current with the rapidly changing LLM/AI landscape?
- [ ] Describe a time you had to explain a complex AI system to a non-technical stakeholder
- [ ] How do you approach building AI systems that need to be auditable and compliant?

---

## Quick-Start Checklist (Week 1 Actions)

- [ ] Fork and clone this repo; set up Python 3.12 venv; install `requirements.txt`
- [ ] Run `01-intro-to-ai-agents/code_samples/01-python-agent-framework.ipynb` end-to-end
- [ ] Create a GitHub repo named `wells-fargo-ai-portfolio`; add MIT license, `.gitignore`, pre-commit config
- [ ] Sign up for: Neo4j AuraDB Free, Azure Free Trial (or use GitHub Models free tier)
- [ ] Create your first FastAPI "hello world" with a `/health` endpoint and a passing `pytest` test
- [ ] Bookmark all resources in §6
- [ ] Set a weekly calendar block for study hours (be honest about your availability)

---

*Generated based on the Wells Fargo Senior AI Engineer job description (LinkedIn, May 2026 posting) and the `microsoft/ai-agents-for-beginners` course repository. Plan assumes Python intermediate starting level at 10–15 hrs/week.*
