<h1 align="center">Hi, I'm Vaibhavi Phalle 👋</h1>
<h3 align="center"> Software Engineer · Distributed Systems · AI Infrastructure</h3>

<p align="left">
Software Engineer with 3+ years building distributed systems and high-throughput backend services at Bank of America, with strong fundamentals in OOP, data structures, distributed systems, and system design. I build end-to-end — from schema design to production monitoring — and have recently extended that rigor into AI infrastructure, shipping a retrieval-augmented generation system and a distributed rate limiter to production-grade quality.
</p>

---

### 🧭 Experience

**Independent Study & Project Development** — *Self-Directed, Backend & AI Infrastructure*
`Dec 2024 – Present`
- Relocated to the US in December 2024; used the work-authorization waiting period for structured upskilling and hands-on project development
- Completed 3 DataCamp courses and self-studied core LLM concepts — tokenization, embeddings, transformer architecture, and attention (Q/K/V) — building a solid foundation in modern AI systems
- Applied that foundation to sharpen backend engineering skills and build production-style systems/projects end-to-end, from architecture through evaluation

**Bank of America** — *SDE I*
`Jul 2023 – Nov 2024`
- Designed DAG-based orchestration pipelines for distributed data workflows, improving fault tolerance and cutting manual operations by 30%
- Built centralized observability, distributed logging, and automated alerting for production systems, cutting incident-detection time by 40%; owned on-call triage and incident response
- Refactored core services into modular, well-tested OOP components, improving team engineering productivity by 25%
- Implemented authentication and authorization flows (OAuth2, Bearer Token, JWT) for internal services, enforcing clear boundaries between identity and permissions

**Bank of America** — *Senior Tech Associate*
`Jul 2022 – Jul 2023`
- Designed and built a real-time transaction-processing service over a distributed key-value store, handling millions of daily transactions with low-latency ingestion
- Led migration to containerized Docker deployments on Kubernetes-adjacent CI/CD pipelines, strengthening release reliability

**LogisticsNow** — *Software Engineering Intern*
`Oct 2021 – May 2022`
- Built Kafka producer-consumer pipelines for asynchronous event processing
- Developed a Selenium-based automated test suite, catching production-blocking bugs pre-release

---

### 🚀 Featured Projects

<table>
<tr>
<td width="50%" valign="top">

**🔀 [Distributed Rate Limiter](https://github.com/VaibhaviPhalle/distributed_rate_limiter/blob/main/README.md)**

- A hybrid rate-limiting API gateway combining a global token bucket with per-tenant sliding-window counters, enforced atomically through Redis Lua scripts so correctness holds under concurrent load across gateway instances. 
- Cheap-first evaluation order rejects infrastructure-threatening bursts before a tenant is ever charged quota, with independently configurable fail-open/fail-closed strategy per layer. Tenant policies live in Postgres with a 60-second in-memory cache so changes propagate without a restart.

📊 Load-tested with Locust: **1,438 requests, 0 failures, 18ms P99** latency added by the rate-limit check.

`Python` `FastAPI` `Redis (Lua)` `PostgreSQL` `Docker Compose` `Locust`

</td>
<td width="50%" valign="top">

**📚 [RAG Docs Assistant](https://github.com/VaibhaviPhalle/DevDocs_Rag/blob/main/README.md)**

- A hybrid retrieval-augmented generation system answering questions over official FastAPI, Redis, and Kubernetes documentation, built with production-service rigor rather than as an LLM-wrapper demo. 
- Combines dense vector search and BM25 keyword search via reciprocal rank fusion, followed by cross-encoder re-ranking, with a two-layer citation enforcement system (chunk-ID existence check plus a Ragas-scored faithfulness check) that regenerates or refuses rather than returning an unsupported claim.

📊 CI-gated evaluation pipeline runs a **100–200 question golden set** on every merge, blocking regressions like a broken unit test. Fully self-hosted, zero paid APIs.

`Python` `FastAPI` `Qdrant` `Ollama` `Ragas` `Docker Compose` `GitHub Actions`

</td>
</tr>
</table>

---

### 🛠️ Skills

**Languages & Core Fundamentals**

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" />
  <img src="https://img.shields.io/badge/ReactJS-61DAFB?style=flat-square&logo=react&logoColor=black" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square" />
  <img src="https://img.shields.io/badge/Pydantic-E92063?style=flat-square" />
  <img src="https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/OOP%20%26%20Design%20Patterns-555555?style=flat-square" />
  <img src="https://img.shields.io/badge/Data%20Structures%20%26%20Algorithms-555555?style=flat-square" />
  <img src="https://img.shields.io/badge/REST%20API%20Design-555555?style=flat-square" />
</p>

**AI / ML / GenAI**

<p align="left">
  <img src="https://img.shields.io/badge/RAG%20Pipelines-FF6F00?style=flat-square" />
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/Sentence--Transformers-FF6F00?style=flat-square" />
  <img src="https://img.shields.io/badge/Cross--Encoder%20Reranking-FF6F00?style=flat-square" />
  <img src="https://img.shields.io/badge/Ragas%20(LLM%20Eval)-FF6F00?style=flat-square" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square" />
</p>

**Cloud, Infra & Data**

<p align="left">
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white" />
  <img src="https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white" />
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" />
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square" />
  <img src="https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white" />
  <img src="https://img.shields.io/badge/DAG%20Orchestration-425CC7?style=flat-square" />
  <img src="https://img.shields.io/badge/Distributed%20Grid%20Computing-425CC7?style=flat-square" />
  <img src="https://img.shields.io/badge/OAuth2%20%7C%20JWT-425CC7?style=flat-square" />
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white" />
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

### 📫 Let's Connect

<p align="left">
  <a href="mailto:vphalle82@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/vaibhaviphalle/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" /></a>
  <a href="https://github.com/vaibhaviphalle"><img src="https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=googlechrome&logoColor=white" /></a>
</p>

<p align="center"><i>Based in San Jose, CA · Open to Senior Backend & AI/GenAI Engineering roles</i></p>
