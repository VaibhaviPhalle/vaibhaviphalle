<h1 align="center">Hi, I'm Vaibhavi Phalle 👋</h1>
<h3 align="center"> Software Engineer · Distributed Systems · AI Infrastructure</h3>


Email: vphalle82@gmail.com &nbsp;|&nbsp;
LinkedIn: linkedin.com/in/vaibhaviphalle &nbsp;|&nbsp;
GitHub: github.com/vaibhaviphalle
</p>

---

<p align="left">
Software Engineer with 3+ years building distributed systems and high-throughput backend services at Bank of America, with strong fundamentals in OOP, data structures, distributed systems, and system design. I build end-to-end, from schema design to production monitoring, and have recently extended that rigor into AI infrastructure, shipping a retrieval-augmented generation system and a distributed rate limiter to production-grade quality.
</p>

---

### 🧭 Experience

**Independent Study & Project Development**, *Self-Directed, Backend & AI Infrastructure*
`Dec 2024 – Present`
- Relocated to the US in December 2024; used the work-authorization waiting period for structured upskilling and hands-on project development
- Completed 3 DataCamp courses and self-studied core LLM concepts: tokenization, embeddings, transformer architecture, and attention (Q/K/V), building a solid foundation in modern AI systems
- Applied that foundation to sharpen backend engineering skills and build production-style systems/projects end-to-end, from architecture through evaluation

**Bank of America**, *SDE I*
`Jul 2023 – Nov 2024`

My work at BofA moved through four connected layers of the same problem: get data flowing reliably, know when it breaks, control who can see it, and make the codebase easy for the next engineer to extend. Roughly in that order:

*Backend & APIs*
- Designed and built REST APIs in Python (FastAPI, SQLAlchemy) powering a real-time analytics dashboard consumed directly by business teams, the foundation the rest of this work sat on top of.

*Distributed Data & Orchestration*
- Designed DAG-based orchestration pipelines for distributed data workflows, improving fault tolerance and cutting manual operations by 30%.

*Observability & Reliability*
- Built centralized observability, distributed logging, and automated alerting for production systems, cutting incident-detection time by 40%, and owned on-call triage and incident response when things did break.

*Security & Access Control*
- Implemented authentication and authorization flows (OAuth2, Bearer Token, JWT) for internal services, drawing a clear line between "who someone is" and "what they're allowed to do."
- Extended that thinking into a full RBAC and ABAC access-control design for the trader-facing dashboard below, gating data visibility both by role (engineers vs. traders) and by team attribute (equity vs. other desks within Global Banking), across a tool used broadly across teams.

*Frontend*
- Built a trader-facing dashboard in ReactJS that replaced a firehose of roughly 1,000 emails per minute during peak windows with dedicated, filterable views, reading data directly from the database and rendering it across multiple visualization sub-panels.

*Engineering Quality & Ownership*
- Refactored core services into modular, well-tested OOP components, improving team engineering productivity by 25%.
- Took ownership of raising unit and integration test coverage across every production repository, moving it from roughly 70% to 90 to 95% and catching regressions before they reached deployment.

**Bank of America**, *Senior Tech Associate*
`Jul 2022 – Jul 2023`

The year before this was mostly foundation-laying: get comfortable with scale, get comfortable with infrastructure, and get into the room where architecture decisions get made.

- Designed and built a real-time transaction-processing service over a distributed key-value store, handling millions of daily transactions with low-latency ingestion. Architecturally comparable to a document or object store like MongoDB, implemented here on internal tooling.
- Led the migration to containerized Docker deployments on Kubernetes-adjacent CI/CD pipelines, strengthening release reliability.
- Used Redis for fast data access while writing scripts for report generation, cutting lookup time for frequently accessed data.

**LogisticsNow**, *Software Engineering Intern*
`Oct 2021 – May 2022`

Where it started: a freight-tracking startup, small team, everything built from scratch.

- Built Kafka producer-consumer pipelines for asynchronous event processing across the freight tracking platform.
- Built and managed the user database from scratch in MySQL, owning schema design and production data entry management.
- Developed a Selenium-based automated test suite that caught production-blocking bugs before release.

---

### 🚀 Featured Projects

**🔀 [Distributed Rate Limiter](https://github.com/VaibhaviPhalle/distributed_rate_limiter/blob/main/README.md)**

- A hybrid rate-limiting API gateway combining a global token bucket with per-tenant sliding-window counters, enforced atomically through Redis Lua scripts so correctness holds under concurrent load across gateway instances.
- Cheap-first evaluation order rejects infrastructure-threatening bursts before a tenant is ever charged quota, with independently configurable fail-open/fail-closed strategy per layer. Tenant policies live in Postgres with a 60-second in-memory cache so changes propagate without a restart.

📊 Load-tested with Locust: **1,438 requests, 0 failures, 18ms P99** latency added by the rate-limit check.

`Python` `FastAPI` `Redis (Lua)` `PostgreSQL` `Docker Compose` `Locust`

**📚 [RAG Docs Assistant](https://github.com/VaibhaviPhalle/DevDocs_Rag/blob/main/README.md)**

- A hybrid retrieval-augmented generation system answering questions over official FastAPI, Redis, and Kubernetes documentation, built with production-service rigor rather than as an LLM-wrapper demo.
- Combines dense vector search and BM25 keyword search via reciprocal rank fusion, followed by cross-encoder re-ranking, with a two-layer citation enforcement system (chunk-ID existence check plus a Ragas-scored faithfulness check) that regenerates or refuses rather than returning an unsupported claim.

📊 CI-gated evaluation pipeline runs a **100–200 question golden set** on every merge, blocking regressions like a broken unit test. Fully self-hosted, zero paid APIs.

`Python` `FastAPI` `Qdrant` `Ollama` `Ragas` `Docker Compose` `GitHub Actions`

---

### 🛠️ Skills

**Languages & Core Fundamentals**

<p align="left">
  <img src="https://img.shields.io/badge/Python-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/C++-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/SQL-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/JavaScript-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/ReactJS-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/FastAPI-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/SQLAlchemy-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/Pydantic-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/pandas-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/NumPy-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/OOP%20%26%20Design%20Patterns-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/Data%20Structures%20%26%20Algorithms-2C3E50?style=flat-square" />
  <img src="https://img.shields.io/badge/REST%20API%20Design-2C3E50?style=flat-square" />
</p>

**AI / ML / GenAI**

<p align="left">
  <img src="https://img.shields.io/badge/RAG%20Pipelines-6E5A7D?style=flat-square" />
  <img src="https://img.shields.io/badge/Hugging%20Face-6E5A7D?style=flat-square" />
  <img src="https://img.shields.io/badge/Sentence--Transformers-6E5A7D?style=flat-square" />
  <img src="https://img.shields.io/badge/Cross--Encoder%20Reranking-6E5A7D?style=flat-square" />
  <img src="https://img.shields.io/badge/Ragas%20(LLM%20Eval)-6E5A7D?style=flat-square" />
  <img src="https://img.shields.io/badge/LangChain-6E5A7D?style=flat-square" />
  <img src="https://img.shields.io/badge/Claude%20Code-6E5A7D?style=flat-square" />
</p>

**Cloud, Infra & Data**

<p align="left">
  <img src="https://img.shields.io/badge/AWS-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Docker-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Kubernetes-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Kafka-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Redis-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/PostgreSQL-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/MySQL-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Qdrant-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/CI%2FCD-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/OpenTelemetry-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/DAG%20Orchestration-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Distributed%20Grid%20Computing-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/OAuth2%20%7C%20JWT-46685C?style=flat-square" />
  <img src="https://img.shields.io/badge/Selenium-46685C?style=flat-square" />
</p>

<sub>*Also familiar with (self-study/personal projects): Apache Airflow, AWS IAM, AWS Lambda, MongoDB*</sub>

---

### 📊 GitHub Activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=vaibhaviphalle&show_icons=true&theme=default&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=vaibhaviphalle&layout=compact&hide_border=true" />
</p>
<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=vaibhaviphalle&hide_border=true" />
</p>

---

<p align="center"><i>Based in San Jose, CA · Open to Senior Backend & AI/GenAI Engineering roles</i></p>
