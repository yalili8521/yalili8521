# Yali Li

Engineer who ships production AI systems end to end: from the first conversation with the
person who has the problem, to a service that runs unattended with a test suite and a
reconciler behind it. Six years in structural engineering (licensed P.E., Washington),
then since 2025 building LLM agent systems, trading infrastructure, and AI tools for
small businesses. Issaquah, WA.

## Selected work

| Repository | What it is | Why it matters |
|---|---|---|
| [auto-trader](https://github.com/yalili8521/auto-trader) | TradingView alerts to live futures orders: FastAPI webhook behind a Cloudflare tunnel, Tradovate REST executor, broker-vs-paper reconciler, NSSM Windows services, 65 mocked unit tests | Live on a real account since April 2026. The README lists four production incidents and the fix and test each one left behind. |
| [agent-bus](https://github.com/yalili8521/agent-bus) | Codex on tap inside Claude Code through a stdlib MCP server, plus a SQLite message bus that lets two LLM agents and a human work one task with explicit handoffs and a single execution authority | Two models reviewing each other, with the human as a first-class participant. The MCP bridge is in daily use. |
| [crypto-alpha-bench](https://github.com/yalili8521/crypto-alpha-bench) | Pre-registered research harness: 82 cross-sectional alphas, time-series momentum, funding-rate cross-section, long-short TSMOM on a 15-coin basket, 2024 to 2026 | Three honest negative results, each with the spec written before the run, the adversarial review, and the data to reproduce it. |
| [meibook](https://github.com/yalili8521/meibook) | Appointments, prepaid membership-card ledger and revenue PWA for one-person beauty studios; React 18, Vite 6, no backend | Shipped at v0.1 and deliberately held there until a distribution test says real owners want it. |
| [auctura-wechat-ai](https://github.com/yalili8521/auctura-wechat-ai) | AI auto-reply webhook for a WeChat Official Account inside WeChat's five-second deadline | Small, complete, tested: signature check, timeout budget, retry dedupe, echo mode without a key. |
| [quantitivestocks](https://github.com/yalili8521/quantitivestocks) | Earlier ML trading system for ETFs: LSTM return regression, XGBoost and LightGBM models, Alpaca paper trading | Where the trading work started. |

## How I work

- Write the evaluation before the feature. Pre-registered pass criteria, no in-sample
  winner selection, and negative results kept in the repository with their specs.
- Every outage becomes a fix and a regression test; the incident table in auto-trader
  is the record.
- Second-model review as a habit: Codex reads what Claude wrote before it ships.
- Python, FastAPI, SQLite, Windows services, Cloudflare tunnels, React, Pine Script;
  Claude API, Model Context Protocol servers, multi-agent orchestration, evaluation loops.

## Before this

Ph.D. in timber engineering (Mississippi State), M.S. structural engineering (Tongji),
licensed Professional Engineer in Washington. Designed seawalls, retaining walls and
bridges for municipal clients, evaluated engineered wood products against building
codes, and ran finite element models against lab data. Bilingual English and Mandarin.
