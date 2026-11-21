<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/banner-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="assets/banner-light.svg" />
  <img alt="Víctor Yohan Betancourt Marín — Ingeniero Backend, Geoespacial y de Automatización con IA" src="assets/banner-dark.svg" width="100%" />
</picture>

<p align="right">
  <a href="README.md">English</a> · <strong>Español</strong>
</p>

<p>
  <a href="https://quanticosystems.com"><img src="https://img.shields.io/badge/Quantico%20Systems-quanticosystems.com-1D4ED8?style=flat-square&logo=googlechrome&logoColor=white" alt="Sitio Web" /></a>
  <a href="https://www.linkedin.com/in/victor-yohan-betancourt-marin-2a648021b/"><img src="https://img.shields.io/badge/LinkedIn-Conectar-0A66C2?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:yohanvictorb@gmail.com"><img src="https://img.shields.io/badge/Email-yohanvictorb%40gmail.com-1E293B?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
</p>

Desarrollo sistemas POS/ERP multimoneda, asistentes comerciales sobre WhatsApp Business Cloud API, plataformas geoespaciales de campo y pipelines de datos en Python autoalojados a través de **[Quantico Systems](https://quanticosystems.com)**.

---

### Arquitectura Destacada — `quantico-censo`

<table>
  <tr>
    <td width="54%" valign="middle">
      <a href="https://mc3yohan.github.io/quantico-censo/">
        <img src="https://raw.githubusercontent.com/Mc3yohan/quantico-censo/main/assets/command-center-desktop.png" alt="Centro de Mando GIS de Quantico Censo" width="100%" />
      </a>
    </td>
    <td width="46%" valign="top">
      <p><strong>Censo Comercial Geoespacial y PWA Offline de Campo</strong></p>
      <p>
        <a href="https://github.com/Mc3yohan/quantico-censo/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/quantico-censo/actions/workflows/ci.yml/badge.svg" alt="Quantico Censo CI" /></a>
      </p>
      <ul>
        <li><strong>CQRS detrás de Nginx:</strong> plano de escritura <code>backend-sync</code> + plano de lectura/WS <code>backend-read</code> enlazados vía Redis Pub/Sub.</li>
        <li><strong>Geocercas PostGIS:</strong> <code>ST_Covers</code> / <code>ST_Distance</code> con índices <code>GiST</code>, cuarentena por desvío GPS y bloqueos <code>FOR UPDATE</code>.</li>
        <li><strong>PWA móvil cifrada:</strong> TypeScript estricto + bóveda <code>PBKDF2-SHA256</code> / <code>AES-GCM-256</code> en Web Worker e <code>IndexedDB</code>.</li>
      </ul>
      <p>
        <a href="https://mc3yohan.github.io/quantico-censo/"><img src="https://img.shields.io/badge/Demo%20en%20Vivo-Abrir-2563EB?style=flat-square" alt="Demo en Vivo" /></a>
        <a href="https://github.com/Mc3yohan/quantico-censo"><img src="https://img.shields.io/badge/C%C3%B3digo%20y%20CI-GitHub-1E293B?style=flat-square&logo=github&logoColor=white" alt="Repositorio" /></a>
      </p>
    </td>
  </tr>
</table>

---

### Repositorios de Backend y Automatización

<table>
  <tr>
    <td width="33.3%" valign="top">
      <p><strong><a href="https://github.com/Mc3yohan/whatsapp-ai-handoff-engine">whatsapp-ai-handoff-engine</a></strong></p>
      <p><a href="https://github.com/Mc3yohan/whatsapp-ai-handoff-engine/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/whatsapp-ai-handoff-engine/actions/workflows/ci.yml/badge.svg" alt="CI" /></a></p>
      <p>Servicio webhook en FastAPI para Meta WhatsApp Cloud API con verificación HMAC <code>X-Hub-Signature-256</code>, idempotencia atómica <code>wamid</code> en SQLite WAL, precios <code>Decimal</code>, rutas de operador con API-Key y traspaso humano determinista.</p>
    </td>
    <td width="33.3%" valign="top">
      <p><strong><a href="https://github.com/Mc3yohan/multicurrency-pos-ledger-api">multicurrency-pos-ledger-api</a></strong></p>
      <p><a href="https://github.com/Mc3yohan/multicurrency-pos-ledger-api/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/multicurrency-pos-ledger-api/actions/workflows/ci.yml/badge.svg" alt="CI" /></a></p>
      <p>Motor contable POS multimoneda (<code>USD / VES / USDT</code>) con bloqueo de stock <code>BEGIN IMMEDIATE</code>, protección contra redondeo en cuotas, snapshots inmutables de tasa, aislamiento de márgenes por API-Key RBAC e importador CSV atómico.</p>
    </td>
    <td width="33.3%" valign="top">
      <p><strong><a href="https://github.com/Mc3yohan/python-ops-automation-pipeline">python-ops-automation-pipeline</a></strong></p>
      <p><a href="https://github.com/Mc3yohan/python-ops-automation-pipeline/actions/workflows/ci.yml"><img src="https://github.com/Mc3yohan/python-ops-automation-pipeline/actions/workflows/ci.yml/badge.svg" alt="CI" /></a></p>
      <p>Pipeline ETL y de alertas en Python sin dependencias externas con parseo estricto <code>Decimal</code>, deduplicación SHA-256 en SQLite WAL, cuarentena en CSV, imagen Docker no-root y webhooks JSON con reintentos.</p>
    </td>
  </tr>
</table>

<sub>Los sistemas comerciales en producción de clientes bajo Quantico Systems se mantienen en repositorios privados; hay demos interactivas en vivo en <a href="https://quanticosystems.com">quanticosystems.com</a>.</sub>

---

### Contribuciones Open Source

| Pull Request | Estado | Alcance |
| :--- | :---: | :--- |
| **[hanzoai/cloud#58](https://github.com/hanzoai/cloud/pull/58)** | ![Fusionado](https://img.shields.io/badge/FUSIONADO-8957E5?style=flat-square) | Benchmark en Go sin dependencias (`CGO_ENABLED=0`) para agentes empresariales con control dual, versionado CAS y 27 pruebas bajo `-race` |
| **[Get-Concord-AI/concord-mcp#388](https://github.com/Get-Concord-AI/concord-mcp/pull/388)** · **[#389](https://github.com/Get-Concord-AI/concord-mcp/pull/389)** | ![Abierto](https://img.shields.io/badge/ABIERTO-238636?style=flat-square) | Correcciones en TypeScript/MCP para marcadores de cierre en Cursor y reasignación forzada de tareas huérfanas |
| **[prooflinedev/sdk-python#73](https://github.com/prooflinedev/sdk-python/pull/73)** | ![Abierto](https://img.shields.io/badge/ABIERTO-238636?style=flat-square) | Paridad tipada en `ReviewFilters` (`audits`) contra la especificación OpenAPI en los clientes Python síncrono y asíncrono |

---

### Stack Principal

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
