# Hi, I'm Ginger / CodePhantom 👋

Software developer building **CodePhantom Technologies** — a collection of
software, trading-research and automation projects.

## What I'm building

- **CodePhantom App** — Flutter Android/PWA client for scanner, signals,
  licensing, notifications and remote-EA controls.
- **CodePhantom Backend** — Node.js/TypeScript + PostgreSQL/Supabase API with
  auth, permissions, entitlements, licensing, integrations and audit trails.
- **CPT Scanner / Research Framework** — Python + MT5 research platform with
  deterministic datasets, causal M1/tick audits and chronological replication.
- **Remote EA Platform** — mobile control plane + Windows/Azure MT5 execution
  agent, starting in shadow/demo mode with hard risk controls.
- **Magical Conquest** — Unreal Engine fantasy game prototype.
- **CodePhantom Website** — public Next.js company/project site.

## Recent engineering milestones

- **2026-10-03 — Remote EA execution V1:** completed a fail-closed Python/MT5 execution layer with OFF/SHADOW/DEMO modes, hard demo-account enforcement, stop-distance risk sizing, spread/drawdown/position gates, idempotent execution journaling and backend command integration. Dedicated execution/control CI: **26 tests passing** after adding prop-firm-aware risk profiles and concurrent-risk enforcement.
- **2026-10-03 — Remote quantitative research runner:** operationalized a Windows self-hosted GitHub Actions runner connected to local MT5 research data, allowing reproducible causal M1/tick audits, broker bid/ask spread diagnostics, robustness reports and remote experiment queues without committing market datasets to Git.
- **2026-10-03 — Deriv public API research bridge:** connected the Windows runner directly to Deriv's unauthenticated WebSocket market-data API, dynamically resolved 20/22 target instruments (including BTC, ETH, gold and silver), verified M30/H1/D1 candle access, and added persistent paged historical acquisition for cross-feed strategy research.
- **2026-10-03 — Mobile EA control plumbing:** merged CodePhantom App controls for pause/resume, risk commands, disable-new-entries and emergency stop into the backend command queue, while keeping production visibility and backend feature flags fail-closed.
- **2026-10-03 — Prop-firm research + execution profiles:** separated custom portfolio stress policies from real firm rule emulation, added frozen-ledger FTMO/FundedNext rule replay, and merged named FTMO/FundedNext risk profiles into the demo EA without changing strategy logic.
- **2026-09 — CodePhantom mobile/backend platform:** built a Flutter Android/PWA client and Node.js/TypeScript backend covering authentication, RBAC, scanner review, signals, licences, notifications, EA control surfaces, audit logging and PostgreSQL/Supabase persistence.
- **2026-09 — Release/deployment hardening:** shipped signed Android staging builds, web/PWA delivery, backend deployment controls, CORS/host hardening and least-privilege CI changes across the CodePhantom repositories.
- **2026 — Research discipline:** built deterministic strategy experiments with causal lower-timeframe validation, tick-level outcome ordering, out-of-sample separation, cost sensitivity and preserved failed hypotheses rather than post-hoc backtest tuning.

See [ENGINEERING_MILESTONES.md](./ENGINEERING_MILESTONES.md) for the longer recruiter-safe timeline.

## Tech

Python · Java · C# · TypeScript · Flutter/Dart · Next.js · Node.js ·
PostgreSQL · Supabase · GitHub · Linux · MetaTrader 5 · Unreal Engine

## How I work

I like building systems end-to-end: research, backend, client apps, deployment,
testing and operational tooling. For quantitative work I keep failed experiments
in the record and require fresh replication instead of tuning a strategy until a
backtest looks good.

## Public work

Start with the **CodePhantom website repository** and its
`docs/ENGINEERING_PORTFOLIO.md` for a recruiter-safe overview of the private
production systems.

> Production trading logic, credentials, signing material and customer data stay
> private by design.


---

## Current engineering focus

- Building a remote MT5 execution control plane for the existing CodePhantom app/backend.
- Researching reproducible intraday strategies with causal lower-timeframe and tick validation.
- Expanding the public CodePhantom website into a safe shop/portfolio surface.
- Maintaining recruiter-safe public documentation while production trading logic and credentials remain private.

> This profile README is maintained as the public index for ongoing CodePhantom engineering work. New public-safe projects and milestones can be added here as they mature.
