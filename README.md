<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg" />
  <img alt="Víctor Yohan Betancourt Marín — Backend, Geospatial &amp; AI Automation Engineer" src="assets/banner-dark.svg" width="100%" />
</picture>

<p align="right">
  <strong>English</strong> · <a href="README.es.md">Español</a>
</p>

<p>
  <a href="https://quanticosystems.com"><img src="https://img.shields.io/badge/Quantico%20Systems-quanticosystems.com-1D4ED8?style=flat-square&logo=googlechrome&logoColor=white" alt="Website" /></a>
  <a href="https://www.linkedin.com/in/victor-yohan-betancourt-marin-2a648021b/"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:yohanvictorb@gmail.com"><img src="https://img.shields.io/badge/Email-yohanvictorb%40gmail.com-1E293B?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

I build multi-currency POS/ERP backends, WhatsApp Business Cloud API sales assistants, geospatial field platforms, and self-hosted Python data pipelines through **[Quantico Systems](https://quanticosystems.com)**.

---

### Featured Architecture — `quantico-censo`

<table>
  <tr>
    <td width="54%" valign="middle">
      <a href="https://mc3yohan.github.io/quantico-censo/">
        <img src="https://raw.githubusercontent.com/Mc3yohan/quantico-censo/main/assets/command-center-desktop.png" alt="Quantico Censo GIS Command Center" width="100%" />
      </a>
    </td>
    <td width="46%" valign="top">
      <p><strong>Geospatial Retail Census &amp; Offline Field PWA</strong></p>
      <p>
        <a href="https://github.com/Mc3yohan/quantico-censo/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/quantico-censo/actions/workflows/ci.yml/badge.svg" alt="Quantico Censo CI" /></a>
      </p>
      <ul>
        <li><strong>CQRS split behind Nginx:</strong> <code>backend-sync</code> write plane + <code>backend-read</code> read/WS plane bridged via Redis Pub/Sub.</li>
        <li><strong>PostGIS geofencing:</strong> <code>ST_Covers</code> / <code>ST_Distance</code> with <code>GiST</code> indexes, GPS drift quarantine, and <code>FOR UPDATE</code> locking.</li>
        <li><strong>Offline encrypted PWA:</strong> Strict TypeScript + Web Worker <code>PBKDF2-SHA256</code> / <code>AES-GCM-256</code> vault in <code>IndexedDB</code>.</li>
      </ul>
      <p>
        <a href="https://mc3yohan.github.io/quantico-censo/"><img src="https://img.shields.io/badge/Live%20Simulator-Open%20App-2563EB?style=flat-square" alt="Live Simulator" /></a>
        <a href="https://github.com/Mc3yohan/quantico-censo"><img src="https://img.shields.io/badge/Source%20%26%20Docker%20CI-Repository-1E293B?style=flat-square&logo=github&logoColor=white" alt="Repository" /></a>
      </p>
    </td>
  </tr>
</table>

---

### Backend & Automation Repositories

<table>
  <tr>
    <td width="33.3%" valign="top">
      <p><strong><a href="https://github.com/Mc3yohan/whatsapp-ai-handoff-engine">whatsapp-ai-handoff-engine</a></strong></p>
      <p><a href="https://github.com/Mc3yohan/whatsapp-ai-handoff-engine/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/whatsapp-ai-handoff-engine/actions/workflows/ci.yml/badge.svg" alt="CI" /></a></p>
      <p>FastAPI Meta WhatsApp Cloud API webhook service with <code>X-Hub-Signature-256</code> HMAC checks, atomic SQLite WAL <code>wamid</code> idempotency, <code>Decimal</code> pricing, API-key operator routes, and deterministic human handoff.</p>
    </td>
    <td width="33.3%" valign="top">
      <p><strong><a href="https://github.com/Mc3yohan/multicurrency-pos-ledger-api">multicurrency-pos-ledger-api</a></strong></p>
      <p><a href="https://github.com/Mc3yohan/multicurrency-pos-ledger-api/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/multicurrency-pos-ledger-api/actions/workflows/ci.yml/badge.svg" alt="CI" /></a></p>
      <p>Multi-currency POS ledger (<code>USD / VES / USDT</code>) with <code>BEGIN IMMEDIATE</code> stock locking, split-rounding defense, immutable rate snapshots, API-key RBAC margin isolation, and atomic CSV imports.</p>
    </td>
    <td width="33.3%" valign="top">
      <p><strong><a href="https://github.com/Mc3yohan/python-ops-automation-pipeline">python-ops-automation-pipeline</a></strong></p>
      <p><a href="https://github.com/Mc3yohan/python-ops-automation-pipeline/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/python-ops-automation-pipeline/actions/workflows/ci.yml/badge.svg" alt="CI" /></a></p>
      <p>Zero-dependency Python ETL &amp; alerting pipeline with strict <code>Decimal</code> parsing, SHA-256 SQLite WAL deduplication, quarantine CSV exports, non-root Docker image, and retryable JSON webhooks.</p>
    </td>
  </tr>
</table>

<sub>Client commercial systems built under Quantico Systems are maintained in private repositories; interactive demos are live at <a href="https://quanticosystems.com">quanticosystems.com</a>.</sub>

---

### Open Source Contributions

| Pull Request | Status | Scope |
| :--- | :---: | :--- |
| **[hanzoai/cloud#58](https://github.com/hanzoai/cloud/pull/58)** | ![Merged](https://img.shields.io/badge/MERGED-8957E5?style=flat-square) | Dependency-free Go (`CGO_ENABLED=0`) dual-control business-agent benchmark with CAS versioning and 27 race-tested cases |
| **[Get-Concord-AI/concord-mcp#388](https://github.com/Get-Concord-AI/concord-mcp/pull/388)** · **[#389](https://github.com/Get-Concord-AI/concord-mcp/pull/389)** | ![Open](https://img.shields.io/badge/OPEN-238636?style=flat-square) | TypeScript/MCP fixes for Cursor stop-hook markers and forced recovery of stale tasks without a human owner |
| **[prooflinedev/sdk-python#73](https://github.com/prooflinedev/sdk-python/pull/73)** | ![Open](https://img.shields.io/badge/OPEN-238636?style=flat-square) | Typed `ReviewFilters` OpenAPI parity (`audits` parameter) across sync and async Python SDK clients |

---

### Core Stack

<p>
  <img src="https://img.shields.io/badge/Python-111827?style=flat-square&logo=python&logoColor=38BDF8" alt="Python" />
  <img src="https://img.shields.io/badge/FastAPI-111827?style=flat-square&logo=fastapi&logoColor=10B981" alt="FastAPI" />
  <img src="https://img.shields.io/badge/Go-111827?style=flat-square&logo=go&logoColor=38BDF8" alt="Go" />
  <img src="https://img.shields.io/badge/TypeScript-111827?style=flat-square&logo=typescript&logoColor=60A5FA" alt="TypeScript" />
  <img src="https://img.shields.io/badge/Next.js-111827?style=flat-square&logo=nextdotjs&logoColor=FFFFFF" alt="Next.js" />
  <img src="https://img.shields.io/badge/PostgreSQL%20%2B%20PostGIS-111827?style=flat-square&logo=postgresql&logoColor=60A5FA" alt="PostgreSQL + PostGIS" />
  <img src="https://img.shields.io/badge/Redis-111827?style=flat-square&logo=redis&logoColor=F87171" alt="Redis" />
  <img src="https://img.shields.io/badge/SQLite%20WAL-111827?style=flat-square&logo=sqlite&logoColor=38BDF8" alt="SQLite WAL" />
  <img src="https://img.shields.io/badge/Docker-111827?style=flat-square&logo=docker&logoColor=38BDF8" alt="Docker" />
  <img src="https://img.shields.io/badge/Nginx-111827?style=flat-square&logo=nginx&logoColor=34D399" alt="Nginx" />
  <img src="https://img.shields.io/badge/Cloudflare%20Workers-111827?style=flat-square&logo=cloudflare&logoColor=F59E0B" alt="Cloudflare Workers" />
  <img src="https://img.shields.io/badge/WhatsApp%20Cloud%20API-111827?style=flat-square&logo=whatsapp&logoColor=22C55E" alt="WhatsApp Cloud API" />
</p>
