# Engineering Milestones

This is a recruiter-safe record of notable engineering work by **Ripfumelo Vunene Ngobeni (Ginger / CodePhantom)**. Private strategy rules, credentials, customer data and signing material are intentionally excluded.

## October 2026

### Remote EA execution V1
- Built a Python MT5 execution layer with explicit `OFF`, `SHADOW` and `DEMO` modes.
- Added a hard account-mode guard that rejects REAL, CONTEST and unknown accounts.
- Added stop-distance position sizing through MT5 profit calculations.
- Added broker volume validation, spread checks, open-position limits and one-position-per-symbol protection.
- Added daily/total drawdown gates and a sticky emergency-stop path.
- Added `order_check` before broker submission.
- Added a durable signal-id journal to prevent duplicate execution across process restarts.
- Added a clean strategy-to-execution intent interface so research code never calls the broker directly.
- Expanded dedicated CI to **20 passing control/execution tests**.

### Remote quantitative research runner
- Operated a Windows self-hosted GitHub Actions runner for private MT5-backed research.
- Kept large market datasets and tick caches outside Git while attaching them to reproducible CI jobs at runtime.
- Added queued remote experiment execution and uploaded run reports/logs for auditability.
- Added causal M1/tick outcome validation, broker bid/ask spread diagnostics, robustness/concentration reports and portfolio policy replay.

### Prop-firm compatibility research
- Separated CodePhantom's own conservative portfolio stress rules from actual prop-firm rule sets.
- Added a dedicated frozen-ledger replay architecture for documented FTMO and FundedNext constraints.
- Preserved original strategy outputs while testing deployment compatibility independently from signal quality.
- Added support for loss limits, profit targets, minimum trading days and consistency-style rules without retroactively changing strategy entries.

### Research integrity
- Continued preserving failed and inconclusive strategy versions instead of deleting losing evidence.
- Used locked historical blocks, causal execution ordering, broker-specific cost checks and future/OOS gates before promotion.
- Kept Scanner/EA production behavior isolated from unpromoted research candidates.

## September 2026

### CodePhantom App
- Built a Flutter application targeting Android and PWA/browser delivery.
- Implemented registration/login/verification flows, role-aware UI, scanner review, signals, licensing, notifications and EA-control surfaces.
- Produced signed Android staging builds and automated release verification.

### CodePhantom Backend
- Built Node.js/TypeScript + Express APIs backed by PostgreSQL/Supabase.
- Implemented RBAC, permissions, entitlements, licensing, devices, scanner reviews, signals, EA accounts/commands, notifications and audit logs.
- Added rate limiting, feature flags, integration keys and authorization regression tests.
- Deployed staging/backend infrastructure and tightened CORS/host access.

### CodePhantom Scanner
- Built a Python/MT5 market scanner and research framework.
- Added multi-timeframe acquisition, signal review/publishing flows and deterministic research ledgers.
- Moved heavy/off-hours processing to cloud/remote infrastructure while preserving local reproducibility.

### Release and security hardening
- Hardened CI permissions and deployment configuration across CodePhantom repositories.
- Upgraded the public website stack and verified production/staging deployments.
- Kept signing secrets, credentials and production strategy implementation private.

## Ongoing projects

### CodePhantom Technologies
A broader software and quantitative-systems project spanning:
- trading research and automation;
- mobile/web products;
- backend/API engineering;
- cloud deployment and operational tooling;
- licensing and access control.

### Magical Conquest
Fantasy MMORPG prototype work using Unreal Engine, C++/Blueprint-oriented systems design, progression, combat, worldbuilding and multiplayer-oriented architecture.

## Engineering approach

The common pattern across these projects is end-to-end ownership:

**requirements -> architecture -> implementation -> automated tests -> deployment -> telemetry/operations -> iteration**

For quantitative systems specifically:

**frozen hypothesis -> deterministic data -> causal replay -> tick validation -> transaction-cost realism -> robustness -> independent/OOS evidence -> controlled shadow/demo deployment**

That process is intentionally designed to make failed experiments useful evidence rather than hide them.
