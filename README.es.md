# Víctor Yohan Betancourt Marín

**Idioma:** [English (README.md)](README.md) · **Español**

Ingeniero Backend y de Automatización con IA radicado en Caracas (GMT-4, trabajo remoto). Desarrollo sistemas POS/ERP multimoneda, asistentes comerciales sobre WhatsApp Business Cloud API, plataformas geoespaciales de campo y pipelines de datos en Python autoalojados a través de [Quantico Systems](https://quanticosystems.com).

---

### Proyectos Públicos Destacados

| Proyecto | Resumen | Enlaces |
| :--- | :--- | :--- |
| **`quantico-censo`** | Plataforma geoespacial de censo comercial, PWA móvil offline-first cifrada (`Web Worker` + `PBKDF2-SHA256` + `AES-GCM-256` en `IndexedDB`) y centro de mando CQRS con Nginx, FastAPI, PostGIS, Redis y CI E2E en Docker. | [Simulador en Vivo](https://mc3yohan.github.io/quantico-censo/) · [Repositorio](https://github.com/Mc3yohan/quantico-censo) |
| **`whatsapp-ai-handoff-engine`** | Servicio webhook en FastAPI para Meta WhatsApp Business Cloud API con verificación HMAC `X-Hub-Signature-256`, idempotencia por `wamid` en SQLite WAL, precios en `Decimal` y traspaso determinista a operador humano. | [Repositorio](https://github.com/Mc3yohan/whatsapp-ai-handoff-engine) |
| **`multicurrency-pos-ledger-api`** | Motor contable POS multimoneda (`USD / VES / USDT`) con bloqueo atómico de inventario en SQLite WAL (`BEGIN IMMEDIATE`), *snapshots* inmutables de tasa, aislamiento de márgenes por API-Key RBAC e importador idempotente CSV. | [Repositorio](https://github.com/Mc3yohan/multicurrency-pos-ledger-api) |
| **`python-ops-automation-pipeline`** | Pipeline ETL y alertas en Python sin dependencias externas con parseo estricto `Decimal`, deduplicación SHA-256 en SQLite, cuarentena en CSV y empaquetado Docker. | [Repositorio](https://github.com/Mc3yohan/python-ops-automation-pipeline) |

*Los sistemas comerciales en producción de clientes en Quantico Systems se alojan en repositorios privados; puedes probar demos interactivas por industria en [quanticosystems.com](https://quanticosystems.com).*

---

### Contribuciones Open Source

- **[hanzoai/cloud#58](https://github.com/hanzoai/cloud/pull/58)** *(Fusionado)* — Benchmark en Go sin dependencias (`CGO_ENABLED=0`) para agentes empresariales con control dual, versionado CAS optimista y 27 pruebas verificadas bajo `-race`.
- **[Get-Concord-AI/concord-mcp#388](https://github.com/Get-Concord-AI/concord-mcp/pull/388)** y **[#389](https://github.com/Get-Concord-AI/concord-mcp/pull/389)** — Correcciones en TypeScript/MCP para marcadores de cierre en Cursor y reasignación forzada de tareas huérfanas.
- **[prooflinedev/sdk-python#73](https://github.com/prooflinedev/sdk-python/pull/73)** — Paridad tipada en `ReviewFilters` (`audits`) contra la especificación OpenAPI en los clientes Python síncrono y asíncrono.

---

### Stack Principal

- **Backend y Datos:** Python (`FastAPI`, `SQLAlchemy 2`, `Pydantic v2`, `pytest`), Go, PostgreSQL + PostGIS, Redis, SQLite (WAL), Docker, Nginx.
- **IA y Mensajería:** WhatsApp Business Cloud API, *guardrails* deterministas de herramientas y precios, APIs de Gemini / OpenAI / Claude, servidores MCP e inferencia local sobre GPU de 24 GB VRAM para cargas de trabajo con datos sensibles.
- **Frontend y Edge:** TypeScript, Next.js / React, Leaflet GIS, PWAs offline-first (`IndexedDB` + Web Crypto), Cloudflare Workers y D1.

---

[quanticosystems.com](https://quanticosystems.com) · [yohanvictorb@gmail.com](mailto:yohanvictorb@gmail.com)
