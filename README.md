<h1 align="center">Nikolay Kononykhin</h1>

<p align="center">
  <b>Python Backend Developer</b><br>
  FastAPI · Django · PostgreSQL · async services, LLM/RAG integrations, bots and background workers
</p>

<p align="center">
  <a href="mailto:kononikhinnikolay@gmail.com"><img src="https://img.shields.io/badge/Email-kononikhinnikolay%40gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email"></a>
  <a href="https://github.com/kolykonon?tab=repositories"><img src="https://img.shields.io/badge/GitHub-kolykonon-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"></a>
</p>

---

## About

Backend developer building production-style Python services: async REST APIs on **FastAPI**, web backends on **Django**, background processing with **Celery** and **APScheduler**, message queues with **RabbitMQ** and LLM-powered features with **RAG** over vector search.

Hackathons as **team lead and backend developer**: **MAX Hackathon** · **MTS True Tech Hack** · **IT Purple Hack** — owning the backend architecture, task split and delivery under tight deadlines.

---

## Tech Stack

| Area | Tools |
|---|---|
| **Languages** | Python 3.13, SQL, Bash |
| **Frameworks** | FastAPI, Django 5, Pydantic, HTTPX |
| **Data** | PostgreSQL, SQLAlchemy 2 (async), Alembic, Redis, Qdrant |
| **Async & messaging** | Celery, RabbitMQ, APScheduler, asyncio |
| **AI / LLM** | LLM APIs, RAG, embeddings, pymorphy3 |
| **Infrastructure** | Docker, Docker Compose, Caddy, Kubernetes (learning) |
| **Tooling** | uv, Poetry, pytest, Ruff, mypy, pre-commit, GitHub Actions, Git |

---

## Featured Projects

### 🩸 [Kaplya — blood donor assistant](https://github.com/kolykonon/max-hackaton)
<sub>MAX Hackathon · case «Забота о людях» · team lead & backend</sub>

Bot and mini app for the MAX messenger: users learn donation rules, choose a donor center and a slot on an interactive map, book an appointment, receive reminders and generate a rest-day application after donating.

- Async **FastAPI** backend on **SQLAlchemy 2 + asyncpg** over **PostgreSQL 17**; **Alembic** migrations and seed import on startup
- Separate long-polling **bot** process for the MAX Bot API; mini app auth via `initData` signature validation
- **APScheduler** reminders, PDF/DOCX document generation, OpenAPI contract
- **pytest** coverage for auth, booking flow, eligibility rules and groups
- Full stack (backend, bot, React SPA behind **Caddy**, optional Cloudflare tunnel) starts with a single `docker compose up`

`FastAPI` `SQLAlchemy` `PostgreSQL` `Alembic` `APScheduler` `Caddy` `Docker` `pytest` `uv`

### 🤖 [GPTHub — multi-model AI assistant](https://github.com/kolykonon/mts-true-tech-hack)
<sub>MTS True Tech Hack · team lead & backend</sub>

OpenAI-compatible pipelines service behind Open WebUI that routes each request to the right model.

- Task router: text, vision, image generation and editing — each mapped to a dedicated model
- **RAG** over uploaded PDF / DOCX / XLSX: parsing, chunking, embeddings stored in **Qdrant**
- Long-term user memory, web search with page scraping
- **Redis** response caching, **PostgreSQL** storage

`FastAPI` `LLM API` `RAG` `Qdrant` `Redis` `PostgreSQL` `Docker`

### 🏷️ [Micro-category extraction service](https://github.com/kolykonon/it-purple-hack)
<sub>IT Purple Hack · team lead & backend</sub>

Service that detects additional services in classified-ad text and generates draft listings for each of them.

- Heuristic candidate finder with **pymorphy3** lemmatization + LLM generation layer with local fallback
- Evaluation scripts with precision / recall / F1 reporting
- Heuristic baseline on 2,477 ads: **63% precision · 72% recall · 0.67 F1**

`FastAPI` `LLM API` `pymorphy3` `Docker` `pytest`

### Other projects

| Project | Description | Stack |
|---|---|---|
| [onec-python](https://github.com/kolykonon/onec-python) 🚧 | Library for describing 1C:Enterprise configurations as Python code: generates Configurator-format XML with deterministic UUIDs and loads it into an infobase in batch mode. CI/release workflows, typed API, SemVer changelog | Python, uv, pytest, mypy, GitHub Actions |
| [microservices-shop](https://github.com/kolykonon/microservices-shop) 🚧 | Online shop split into auth, catalog, cart, inventory, order, payment and notification services with event-driven communication | FastAPI, SQLAlchemy, RabbitMQ, Kubernetes |
| [internet-shop](https://github.com/kolykonon/internet-shop) | E-commerce backend: catalog, cart, orders, accounts; order emails sent asynchronously by Celery workers | Django 5, PostgreSQL, Celery, RabbitMQ |
| [fastapi-todo-list](https://github.com/kolykonon/fastapi-todo-list) | Task manager REST API with JWT auth, bcrypt hashing and per-user access control | FastAPI, async SQLAlchemy, PostgreSQL, Alembic |

---

## Currently

- 🔨 Building **microservices-shop** — service boundaries, message-driven communication via RabbitMQ, Kubernetes deployment
- 📚 Next up: Kafka, observability with Prometheus / Grafana, Redis caching strategies

**Open to Python Backend Developer roles** — [get in touch](mailto:kononikhinnikolay@gmail.com).
