<h1 align="center">Nikolay Kononykhin</h1>

<p align="center">
  Backend Developer · Python · FastAPI & Django<br>
  Async REST APIs, LLM/RAG services, bots and background workers
</p>

<p align="center">
  <a href="mailto:kononikhinnikolay@gmail.com">
    <img src="https://img.shields.io/badge/Email-kononikhinnikolay@gmail.com-D14836?style=flat-square&logo=gmail&logoColor=white" alt="Email">
  </a>
  <img src="https://img.shields.io/badge/Open%20to-Junior%20Backend%20roles-2ea44f?style=flat-square" alt="Open to work">
</p>

---

### About

- Python backend developer focused on **FastAPI** (async SQLAlchemy, Pydantic) and **Django**.
- I care about clean layering, typed schemas, migrations and tests — not just "it works on my machine".
- Everything I build ships in **Docker Compose**: one command, migrations on startup, documented OpenAPI.
- Hackathons: **MAX hackathon** (case "Забота о людях"), **MTS True Tech Hack**, **IT Purple Hack**.

---

### Tech Stack

**Languages**

![Python](https://img.shields.io/badge/-Python%203.13-3776AB?style=flat-square&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/-SQL-4479A1?style=flat-square&logo=postgresql&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)

**Backend**

![FastAPI](https://img.shields.io/badge/-FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/-Django-092E20?style=flat-square&logo=django&logoColor=white)
![Pydantic](https://img.shields.io/badge/-Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/-SQLAlchemy%202%20(async)-D71F00?style=flat-square&logo=sqlalchemy&logoColor=white)
![Alembic](https://img.shields.io/badge/-Alembic-6BA81E?style=flat-square&logo=alembic&logoColor=white)
![Celery](https://img.shields.io/badge/-Celery-37814A?style=flat-square&logo=celery&logoColor=white)
![APScheduler](https://img.shields.io/badge/-APScheduler-555555?style=flat-square&logo=python&logoColor=white)
![HTTPX](https://img.shields.io/badge/-HTTPX-2F3E4E?style=flat-square&logo=python&logoColor=white)

**Data, Messaging & Search**

![PostgreSQL](https://img.shields.io/badge/-PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/-Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![RabbitMQ](https://img.shields.io/badge/-RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white)
![Qdrant](https://img.shields.io/badge/-Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white)

**AI / LLM**

![LLM API](https://img.shields.io/badge/-LLM%20API-412991?style=flat-square&logo=openai&logoColor=white)
![RAG](https://img.shields.io/badge/-RAG%20%26%20Embeddings-6E40C9?style=flat-square)
![pymorphy3](https://img.shields.io/badge/-pymorphy3-3776AB?style=flat-square&logo=python&logoColor=white)

**Tooling & Infra**

![Docker](https://img.shields.io/badge/-Docker%20Compose-2496ED?style=flat-square&logo=docker&logoColor=white)
![Caddy](https://img.shields.io/badge/-Caddy-1F88C0?style=flat-square&logo=caddy&logoColor=white)
![uv](https://img.shields.io/badge/-uv-DE5FE9?style=flat-square&logo=uv&logoColor=white)
![Poetry](https://img.shields.io/badge/-Poetry-60A5FA?style=flat-square&logo=poetry&logoColor=white)
![Pytest](https://img.shields.io/badge/-pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)
![Ruff](https://img.shields.io/badge/-Ruff-D7FF64?style=flat-square&logo=ruff&logoColor=black)
![Git](https://img.shields.io/badge/-Git-F05032?style=flat-square&logo=git&logoColor=white)

---

### Featured Projects

**[max-hackaton](https://github.com/kolykonon/max-hackaton)** — «Капля»: bot + mini app for blood donors in MAX messenger
Users learn donation rules, pick a donor center and a date on an interactive map, book a demo appointment, get reminders and generate a rest-day application after donating.
Async FastAPI backend with SQLAlchemy 2 + asyncpg over PostgreSQL 17, Alembic migrations and seed import on startup, APScheduler reminders, a separate long-polling bot process for the MAX Bot API, `initData` signature auth, PDF/DOCX document generation. OpenAPI contract, pytest suite (auth, booking flow, eligibility, groups…), whole stack — backend, bot, React SPA behind Caddy, optional Cloudflare tunnel — starts with one `docker compose up`.
`FastAPI` `SQLAlchemy async` `PostgreSQL` `Alembic` `APScheduler` `Caddy` `Docker` `pytest` `uv`

**[mts-true-tech-hack](https://github.com/kolykonon/mts-true-tech-hack)** — GPTHub: multi-model AI assistant (MTS True Tech Hack)
OpenAI-compatible FastAPI pipelines service behind Open WebUI. A router detects the task type (text, vision, image generation / editing) and picks the model; RAG over uploaded PDF / DOCX / XLSX (parsing, chunking, embeddings in Qdrant), long-term user memory, web search with page scraping, Redis caching, PostgreSQL storage. Covered by unit and integration tests.
`FastAPI` `LLM API` `RAG` `Qdrant` `Redis` `PostgreSQL` `Docker` `pytest`

**[it-purple-hack](https://github.com/kolykonon/it-purple-hack)** — Micro-category extraction service (IT Purple Hack)
Microservice that pulls additional services out of classified-ad text and generates draft listings. Heuristic candidate finder (pymorphy3 lemmatization) combined with an LLM generation layer; evaluation scripts report precision / recall / F1 — baseline reached **63% precision / 72% recall**.
`FastAPI` `LLM API` `pymorphy3` `Docker` `pytest`

**[fastapi-todo-list](https://github.com/kolykonon/fastapi-todo-list)** — Task Manager API
REST service with JWT auth, bcrypt password hashing and per-user access control. Async SQLAlchemy over PostgreSQL 16, Alembic migrations, Pydantic schemas, Swagger docs, full Docker Compose setup.
`FastAPI` `PostgreSQL` `SQLAlchemy` `Alembic` `JWT` `Docker`

**[internet-shop](https://github.com/kolykonon/internet-shop)** — E-commerce backend
Django 5 store with catalog, cart, orders and user accounts. Order confirmation emails are sent asynchronously by **Celery** workers through a **RabbitMQ** broker; PostgreSQL, server-rendered templates, Docker Compose.
`Django` `PostgreSQL` `Celery` `RabbitMQ` `Docker`

**[microservices-shop](https://github.com/kolykonon/microservices-shop)** — 🚧 *in progress*
Online shop split into services — auth, catalog, cart, inventory, order, payment, notifications — on FastAPI, communicating via RabbitMQ and deployed to Kubernetes.
`FastAPI` `SQLAlchemy` `RabbitMQ` `Kubernetes` `uv`

<sub>Also: [leet-code](https://github.com/kolykonon/leet-code) — algorithm & data-structure practice in Python.</sub>

---

### Currently

Building **microservices-shop**: service boundaries, message-driven communication with RabbitMQ, Kubernetes deployment.
Next up: Kafka, observability (Prometheus / Grafana), caching strategies with Redis.
Open to Junior Backend Developer roles — feel free to [reach out](mailto:kononikhinnikolay@gmail.com).

---

<p align="center">
  <img height="150" src="https://github-readme-stats.vercel.app/api?username=kolykonon&show_icons=true&hide_border=true&hide_title=true&theme=transparent&icon_color=4169E1" alt="GitHub stats">
  <img height="150" src="https://github-readme-stats.vercel.app/api/top-langs/?username=kolykonon&layout=compact&hide_border=true&theme=transparent&title_color=4169E1" alt="Top languages">
</p>
