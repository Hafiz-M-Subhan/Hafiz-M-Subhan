<h1 align="center">Hafiz Subhan</h1>
<h3 align="center">Senior Backend Laravel Developer · AI Integrations · High-Traffic Systems</h3>

<p align="center">
  <a href="mailto:ranasubhan8601@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
  <a href="https://hafiz-subhan.vercel.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white"/></a>
  <a href="https://www.linkedin.com/in/hafiz-muhammad-subhan-shahid-628a66183/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
  <img src="https://komarev.com/ghpvc/?username=Hafiz-M-Subhan&style=for-the-badge&color=brightgreen" alt="profile views"/>
</p>

---

### About Me

Senior Backend Laravel Developer with 4+ years building production systems — multi-tenant SaaS platforms, live trading backends, e-commerce at scale, and AI-powered APIs. I care about the internals: query plans, queue architecture, broadcasting at 30k concurrent connections, and shipping code that holds under real load.

Currently at **Droidor** building financial and e-commerce platforms for clients in Dubai, Lebanon, and Canada. Also the architect behind the **PSCA AI Chatbot** — a production AI system serving 110M+ citizens across Punjab, Pakistan.

---

### Tech Stack

| Layer | Tools |
|---|---|
| **Backend** | PHP 8.2, Laravel 11, Livewire, Sanctum, CodeIgniter |
| **Real-time** | Laravel Reverb, Laravel Echo, WebSockets, SSE Streaming |
| **Queue / Cache** | Redis, Laravel Horizon, Queue Workers, Jobs |
| **Search** | ElasticSearch, pgvector HNSW, PostgreSQL full-text |
| **Database** | MySQL 8, PostgreSQL 15, Eloquent ORM, query optimization |
| **Admin** | Laravel Filament 3 |
| **Frontend** | Vue 3, Nuxt 3, Next.js 15, TypeScript, Tailwind CSS |
| **AI** | GPT-4o, Claude, RAG pipelines, pgvector |
| **Infra** | Docker Compose, AWS, GitHub Actions, Laravel Telescope |

---

### Featured Projects

#### [laravel-precious-metals-platform](https://github.com/Hafiz-M-Subhan/laravel-precious-metals-platform)
> High-traffic Laravel platform for live precious metals trading

- **Laravel Reverb** broadcasting live XAU/XAG/XPT/XPD price ticks to 30,000+ concurrent WebSocket subscribers
- **Redis** multi-TTL caching strategy (5s price cache, 60s candle cache) cutting DB load by ~95% under burst
- **Event-driven order processing** — `ProcessOrder` job with `ShouldBeUnique`, atomic fill in DB transaction, 3-retry backoff
- **DCA Savings Plan engine** — automated monthly/weekly gold buys with compound projection chart API
- **Filament 3** admin panel with live-polled price table, order stats widget, savings plan management
- **Docker Compose** stack: MySQL 8, Redis, ElasticSearch, Reverb, Horizon, price simulator

`Laravel 11` · `Redis` · `WebSockets` · `ElasticSearch` · `Filament 3` · `Docker`

---

#### [psca-ai-chatbot](https://github.com/Hafiz-M-Subhan/psca-ai-chatbot)
> AI chatbot for Punjab Safe Cities Authority — 110M+ population

- Challan lookup (CNIC / vehicle number) bypasses AI stack entirely — direct DB query under **100ms**
- **Hybrid RAG** engine: pgvector HNSW cosine similarity + PostgreSQL `ts_rank` full-text, powered by GPT-4o
- **Graceful degradation** — falls back to keyword search when OpenAI is unavailable (100% uptime)
- **SSE streaming** responses, Next.js 15 admin dashboard with RBAC (Admin/Superadmin), JWT auth
- Full **Docker Compose** stack: FastAPI, PostgreSQL 15 + pgvector, Alembic migrations, unit + integration tests

`FastAPI` · `GPT-4o` · `pgvector` · `Next.js 15` · `PostgreSQL` · `Docker`

---

#### [laravel-multitenant-saas](https://github.com/Hafiz-M-Subhan/laravel-multitenant-saas)
> Production-ready Laravel multi-tenant SaaS boilerplate

- **Database-per-tenant isolation** via Spatie Multitenancy — subdomain resolves tenant, DB connection switches automatically
- **Stripe billing** — Checkout sessions, plan switching with proration, webhook handling, cancel-at-period-end
- **Async tenant provisioning** — `ProvisionTenant` job creates isolated DB, runs migrations, seeds roles, fires welcome event
- **Feature gates with Redis cache** — `canUseFeature()` cached per tenant, invalidated on plan change
- **Filament 3** superadmin — MRR widget, tenant suspend/reactivate, drag-to-reorder plans

`Laravel 11` · `Spatie Multitenancy` · `Stripe` · `Redis` · `Filament 3` · `RBAC`

---

#### [clinic360](https://github.com/Hafiz-M-Subhan/hospitalMS)
> Full-featured hospital & clinic management system

- **RBAC** — variadic `CheckRole` middleware for Admin, Doctor, Receptionist with clean workflow separation
- **Queue jobs** — automated appointment reminders, bill payment chasers, nightly analytics generation
- **Redis-cached dashboard** — `GenerateDailyReport` job pre-computes all metrics at midnight; dashboard loads from cache, zero DB hits per page load
- **Mail notifications** — `AppointmentReminder` and `BillPaymentDue` queued with exponential backoff (3 retries)
- **Laravel scheduler** — cron-less: reminders at 08:00, bill chasers at 09:00, report regeneration at 00:00

`Laravel 10` · `MySQL` · `Redis` · `Livewire` · `Queues` · `RBAC`

---

### Latest Article

[![DEV.to Article](https://img.shields.io/badge/DEV.to-How_I_Built_a_Real--Time_Price_Feed_for_30k_Users_in_Laravel-0A0A0A?style=for-the-badge&logo=devdotto&logoColor=white)](https://dev.to/rana_subhan/how-i-built-a-real-time-precious-metals-price-feed-for-30000-concurrent-users-in-laravel-4gjg)

---

### GitHub Stats

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Hafiz-M-Subhan&theme=tokyonight&no-frame=true&no-bg=true&margin-w=8&column=4"/>
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=Hafiz-M-Subhan&theme=tokyonight&hide_border=true&date_format=j%20M%5B%20Y%5D"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Hafiz-M-Subhan&theme=tokyo-night&hide_border=true&area=true"/>
</p>

---

<p align="center"><em>Open to senior backend roles. Reach me at ranasubhan8601@gmail.com or on LinkedIn.</em></p>
