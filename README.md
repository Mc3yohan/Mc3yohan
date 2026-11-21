# Víctor Yohan Betancourt Marín

**Language:** **English** · [Español (README.es.md)](README.es.md)

Backend & AI Automation Engineer based in Caracas (GMT-4, working remotely). I build multi-currency POS/ERP backends, WhatsApp Business Cloud API sales assistants, geospatial field platforms, and self-hosted Python data pipelines through [Quantico Systems](https://quanticosystems.com).

---

### Selected Public Projects

| Project | Summary | Links |
| :--- | :--- | :--- |
| **`quantico-censo`** | Geospatial retail census platform, offline-first encrypted mobile PWA (`Web Worker` + `PBKDF2-SHA256` + `AES-GCM-256` in `IndexedDB`), and Nginx/FastAPI/PostGIS/Redis CQRS command center with Docker E2E CI. | [Live Simulator](https://mc3yohan.github.io/quantico-censo/) · [Repository](https://github.com/Mc3yohan/quantico-censo) |
| **`whatsapp-ai-handoff-engine`** | FastAPI webhook service for Meta WhatsApp Business Cloud API featuring `X-Hub-Signature-256` HMAC verification, SQLite WAL `wamid` idempotency, `Decimal` pricing, and deterministic human handoff. | [Repository](https://github.com/Mc3yohan/whatsapp-ai-handoff-engine) |
| **`multicurrency-pos-ledger-api`** | Multi-currency POS ledger (`USD / VES / USDT`) with atomic SQLite WAL stock locking (`BEGIN IMMEDIATE`), immutable exchange-rate snapshots, API-key RBAC margin isolation, and idempotent CSV imports. | [Repository](https://github.com/Mc3yohan/multicurrency-pos-ledger-api) |
| **`python-ops-automation-pipeline`** | Zero-dependency Python ETL and webhook alerting pipeline with strict `Decimal` parsing, SHA-256 SQLite deduplication, quarantine CSVs, and Docker packaging. | [Repository](https://github.com/Mc3yohan/python-ops-automation-pipeline) |

*Commercial client systems built under Quantico Systems are hosted in private repositories; interactive vertical demos are available at [quanticosystems.com](https://quanticosystems.com).*

---

### Open Source Contributions

- **[hanzoai/cloud#58](https://github.com/hanzoai/cloud/pull/58)** *(Merged)* — Dependency-free Go (`CGO_ENABLED=0`) dual-control business-agent benchmark with optimistic CAS versioning and 27 race-tested cases.
- **[Get-Concord-AI/concord-mcp#388](https://github.com/Get-Concord-AI/concord-mcp/pull/388)** & **[#389](https://github.com/Get-Concord-AI/concord-mcp/pull/389)** — TypeScript/MCP fixes for Cursor stop-hook markers and forced recovery of stale tasks without a human owner.
- **[prooflinedev/sdk-python#73](https://github.com/prooflinedev/sdk-python/pull/73)** — Typed `ReviewFilters` OpenAPI parity (`audits` parameter) across sync and async Python SDK clients.

---

### Core Stack

- **Backend & Storage:** Python (`FastAPI`, `SQLAlchemy 2`, `Pydantic v2`, `pytest`), Go, PostgreSQL + PostGIS, Redis, SQLite (WAL), Docker, Nginx.
- **AI & Messaging Systems:** WhatsApp Business Cloud API, deterministic tool-calling & numeric guardrails, Gemini / OpenAI / Claude APIs, MCP servers, local inference on 24 GB VRAM GPUs for privacy-sensitive workloads.
- **Frontend & Edge:** TypeScript, Next.js / React, Leaflet GIS, offline-first PWAs (`IndexedDB` + Web Crypto), Cloudflare Workers & D1.

---

[quanticosystems.com](https://quanticosystems.com) · [yohanvictorb@gmail.com](mailto:yohanvictorb@gmail.com)
