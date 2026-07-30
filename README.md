# <img src="https://img.shields.io/badge/👋-6A0DAD?style=flat-square" height="26"/>&nbsp; Hi, I'm Vaibhavi Phalle

[![](https://img.shields.io/badge/Email-vphalle82%40gmail.com-6A0DAD?style=for-the-badge)](mailto:vphalle82@gmail.com) [![](https://img.shields.io/badge/LinkedIn-vaibhaviphalle-C9A227?style=for-the-badge)](https://www.linkedin.com/in/vaibhaviphalle/)

### *Software Engineer · Distributed Systems · AI Infrastructure*

Software Engineer with 3 years building distributed systems and high-throughput backend services at Bank of America, with strong fundamentals in OOP, data structures, distributed systems, and system design. I build end-to-end, from schema design to production monitoring, and have recently extended that rigor into AI infrastructure, shipping a retrieval-augmented generation system and a distributed rate limiter to production-grade quality.

---

## <img src="https://img.shields.io/badge/🧭-6A0DAD?style=flat-square" height="26"/>&nbsp; Experience

**Independent Study & Project Development** &nbsp;<img src="https://img.shields.io/badge/Self--Directed-9B72CF?style=flat-square"/>&nbsp; `Dec 2024 – Present`

- Relocated to the US in December 2024; used the work-authorization waiting period for structured upskilling and hands-on project development
- Completed 3 DataCamp courses and self-studied core LLM concepts, including tokenization, embeddings, transformer architecture, and attention (Q/K/V), building a solid foundation in modern AI systems
- Applied that foundation to sharpen backend engineering skills and build production-style systems and projects end-to-end, from architecture through evaluation

**Bank of America** &nbsp;<img src="https://img.shields.io/badge/SDE%20I-6A0DAD?style=flat-square"/>&nbsp; `Jul 2023 – Nov 2024`

- Architected DAG-based pipeline orchestration for distributed data workflows, using the same jobs-as-code pattern as Airflow. Added automated failure recovery so jobs self-healed without manual restarts, cutting intervention by 30%.
- Built centralized observability, including log aggregation, alerting thresholds, and real-time dashboards, then owned on-call triage against that instrumentation, cutting mean incident-detection time by 40%.
- Engineered REST APIs in FastAPI and Redis, powering a real-time dashboard with multi-table aggregations. Reduced page load latency by 60%, from 3.5s to under 1.2s.
- Designed RBAC and ABAC access control for a trader-facing dashboard, gating data by role and team attribute so traders, developers, and other teams each saw only their own view of the data.
- Refactored core services into modular, well-tested OOP components, redesigning interfaces so schema changes no longer touched downstream consumers, choosing queues for ordered dispatch and dictionaries for fast lookups as part of that redesign. Lifted engineering productivity by 25% and cut CPU lock-wait time by 40% under concurrent load.
- Built a trader-facing dashboard in ReactJS that replaced a firehose of roughly 1,000 emails per minute during peak windows with dedicated, filterable views, reading data directly from the database and rendering it across multiple visualization sub-panels.

**Bank of America** &nbsp;<img src="https://img.shields.io/badge/Senior%20Tech%20Associate-C9A227?style=flat-square"/>&nbsp; `Jul 2022 – Jul 2023`

- Built a real-time transaction-processing service on a distributed, document-oriented key-value store, comparable to MongoDB. Handled millions of daily transactions at sub-10ms p95 write latency with synchronous write acknowledgment for durability.
- Used Redis as a distributed caching layer for report-generation queries, cutting database read time by nearly 90%, from 1.5 minutes to under 10 seconds.
- Took ownership of unit and integration test coverage across every production repository, raising it from 70% to 90–95%, making regressions a pre-deploy problem instead of a production one.
- Implemented authentication and authorization for internal services using OAuth2, Bearer Token, and JWT, laying the identity layer that the RBAC and ABAC system was later built on.
- Led the migration to containerized Docker deployments on Kubernetes-adjacent CI/CD pipelines, strengthening release reliability.

**LogisticsNow** — *Software Engineering Intern* `Oct 2021 – May 2022`

- Built Kafka producer-consumer pipelines for asynchronous event processing
- Developed a Selenium-based automated test suite, catching production-blocking bugs pre-release

---

## <img src="https://img.shields.io/badge/🚀-C9A227?style=flat-square" height="26"/>&nbsp; Featured Projects

**🔀 [Distributed Rate Limiter](https://github.com/VaibhaviPhalle/distributed_rate_limiter/blob/main/README.md)**

A hybrid rate-limiting API gateway combining a global token bucket with per-tenant sliding-window counters, enforced atomically through Redis Lua scripts so correctness holds under concurrent load across gateway instances. Cheap-first evaluation order rejects infrastructure-threatening bursts before a tenant is ever charged quota, with independently configurable fail-open/fail-closed strategy per layer. Tenant policies live in Postgres with a 60-second in-memory cache so changes propagate without a restart.

📊 Load-tested with Locust: **1,438 requests, 0 failures, 18ms P99** latency added by the rate-limit check.

`Python` `FastAPI` `Redis (Lua)` `PostgreSQL` `Docker Compose` `Locust`

**📚 [RAG Docs Assistant](https://github.com/VaibhaviPhalle/DevDocs_Rag/blob/main/README.md)**

A hybrid retrieval-augmented generation system answering questions over official FastAPI, Redis, and Kubernetes documentation, built with production-service rigor rather than as an LLM-wrapper demo. Combines dense vector search and BM25 keyword search via reciprocal rank fusion, followed by cross-encoder re-ranking, with a two-layer citation enforcement system (chunk-ID existence check plus a Ragas-scored faithfulness check) that regenerates or refuses rather than returning an unsupported claim.

📊 CI-gated evaluation pipeline runs a **100–200 question golden set** on every merge, blocking regressions like a broken unit test. Fully self-hosted, zero paid APIs.

`Python` `FastAPI` `Qdrant` `Ollama` `Ragas` `Docker Compose` `GitHub Actions`

---

## <img src="https://img.shields.io/badge/🛠️-6A0DAD?style=flat-square" height="26"/>&nbsp; Skills

🟣 **Languages & Core Fundamentals**

![](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white) ![](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white) ![](https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black) ![](https://img.shields.io/badge/ReactJS-61DAFB?style=flat-square&logo=react&logoColor=black) ![](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white) ![](https://img.shields.io/badge/SQLAlchemy-D71F00?style=flat-square) ![](https://img.shields.io/badge/Pydantic-E92063?style=flat-square) ![](https://img.shields.io/badge/pandas-150458?style=flat-square&logo=pandas&logoColor=white) ![](https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white) ![](https://img.shields.io/badge/OOP%20%26%20Design%20Patterns-555555?style=flat-square) ![](https://img.shields.io/badge/Data%20Structures%20%26%20Algorithms-555555?style=flat-square) ![](https://img.shields.io/badge/REST%20API%20Design-555555?style=flat-square)

🟡 **AI / ML / GenAI**

![](https://img.shields.io/badge/RAG%20Pipelines-FF6F00?style=flat-square) ![](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black) ![](https://img.shields.io/badge/Sentence--Transformers-FF6F00?style=flat-square) ![](https://img.shields.io/badge/Cross--Encoder%20Reranking-FF6F00?style=flat-square) ![](https://img.shields.io/badge/Ragas%20(LLM%20Eval)-FF6F00?style=flat-square) ![](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white) ![](https://img.shields.io/badge/Claude%20Code-D97757?style=flat-square)

🟣 **Cloud, Infra & Data**

![](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white) ![](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white) ![](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white) ![](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white) ![](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white) ![](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white) ![](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white) ![](https://img.shields.io/badge/Qdrant-DC244C?style=flat-square) ![](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white) ![](https://img.shields.io/badge/CI%2FCD-2088FF?style=flat-square) ![](https://img.shields.io/badge/OpenTelemetry-425CC7?style=flat-square&logo=opentelemetry&logoColor=white) ![](https://img.shields.io/badge/DAG%20Orchestration-425CC7?style=flat-square) ![](https://img.shields.io/badge/Distributed%20Grid%20Computing-425CC7?style=flat-square) ![](https://img.shields.io/badge/OAuth2%20%7C%20JWT-425CC7?style=flat-square) ![](https://img.shields.io/badge/Selenium-43B02A?style=flat-square&logo=selenium&logoColor=white)

*Also familiar with (self-study/personal projects): Apache Airflow, AWS IAM, AWS Lambda, MongoDB*

---

## <img src="https://img.shields.io/badge/📊-C9A227?style=flat-square" height="26"/>&nbsp; GitHub Activity

![](https://github-readme-stats.vercel.app/api?username=vaibhaviphalle&show_icons=true&hide_border=true&count_private=true&bg_color=00000000&title_color=6A0DAD&icon_color=C9A227&text_color=333333) ![](https://github-readme-stats.vercel.app/api/top-langs/?username=vaibhaviphalle&layout=compact&hide_border=true&bg_color=00000000&title_color=6A0DAD&text_color=333333)

![](https://github-readme-streak-stats.herokuapp.com/?user=vaibhaviphalle&hide_border=true&background=00000000&ring=6A0DAD&fire=C9A227&currStreakLabel=6A0DAD)

---

## <img src="https://img.shields.io/badge/📫-6A0DAD?style=flat-square" height="26"/>&nbsp; Let's Connect

[![](https://img.shields.io/badge/Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:vphalle82@gmail.com) [![](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/vaibhaviphalle/) [![](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=googlechrome&logoColor=white)](https://github.com/vaibhaviphalle)

*Based in San Jose, CA · Open to Senior Backend & AI/GenAI Engineering roles*
