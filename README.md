# Yali Li

Engineer who builds and operates LLM systems that have to keep running: a live futures
execution service with broker reconciliation and a regression suite, a scheduled agent fleet
graded by a critic agent, and a message bus that lets two models and a human share one task.
Five years in structural engineering (licensed P.E., Washington) before the move to software.
Issaquah, WA. Full write-ups with diagrams at [dearyali.com](https://dearyali.com).

## Selected work

| Repository | What it is | Why it matters |
|---|---|---|
| [auto-trader](https://github.com/yalili8521/auto-trader) | TradingView alerts to live futures orders: FastAPI webhook behind a Cloudflare tunnel, Tradovate REST executor, broker-vs-paper reconciler, NSSM Windows services, 76 mocked unit tests | Live on a real account since April 2026. The README lists four production incidents and the fix and test each one left behind. |
| [pain-finder-agent](https://github.com/yalili8521/pain-finder-agent) | Nightly agent that mines Reddit, Hacker News and GitHub for real user pain, drafts a ranked report, and has a separate critic agent score it against a rubric before anything is published | The spec, the rubric and a 17-run feedback log are in the repository. Evaluation before publication, as a habit. |
| [agent-bus](https://github.com/yalili8521/agent-bus) | Codex on tap inside Claude Code through a stdlib MCP server, plus a SQLite message bus that lets two LLM agents and a human work one task with explicit handoffs and a single execution authority | Two models reviewing each other, with the human as a first-class participant. The MCP bridge is in daily use. |
| [foundry-repo-explainer](https://github.com/yalili8521/foundry-repo-explainer) | Microsoft Foundry Agent Service demo: an agent with one function tool over the GitHub API and a graded ten-question cloud evaluation (tool-call accuracy and relevance) | Pass bar written before the run; 9 of 10 on both evaluators, and the one miss is documented rather than tuned away. |
| [subscription-tracker](https://github.com/yalili8521/subscription-tracker) | React and TypeScript front end, serverless API on Vercel with MongoDB, Google sign-in, and a Gmail import that asks a model whether each billing email is a subscription | Three days, 55 commits. A second-model review caught the full email body going to the model; the import now redacts it first. |
| [quantitivestocks](https://github.com/yalili8521/quantitivestocks) | ML trading research for ETFs: an LSTM that regresses expected return instead of predicting direction, XGBoost and LightGBM models, walk-forward backtests, Alpaca paper trading, public dashboard | The backtests said the edge was not there. The dashboard still shows the paper accounts, losses included. |

Also public: [meibook](https://github.com/yalili8521/meibook), a booking and prepaid-card ledger
app for one-person studios; [crypto-alpha-bench](https://github.com/yalili8521/crypto-alpha-bench),
three pre-registered crypto alpha tests with negative results kept; [auctura-wechat-ai](https://github.com/yalili8521/auctura-wechat-ai),
a WeChat auto-reply webhook that answers inside the five-second deadline; and two bootcamp React
stores, [funzmart](https://github.com/yalili8521/funzmart) and [salinaka](https://github.com/yalili8521/salinaka).

## How I work

- Write the evaluation before the feature. Pre-registered pass criteria, no in-sample
  winner selection, and negative results kept in the repository with their specs.
- Every outage becomes a fix and a regression test; the incident table in auto-trader
  is the record.
- Second-model review as a habit: Codex reads what Claude wrote before it ships.
- Python, FastAPI, SQLite, Windows services, Cloudflare tunnels, React and TypeScript,
  Pine Script; Claude API, Model Context Protocol servers, Microsoft Foundry Agent Service,
  multi-agent orchestration, evaluation loops.

## Before this

Ph.D. in timber engineering (Mississippi State), M.S. structural engineering (Tongji),
licensed Professional Engineer in Washington. Designed marine structures, seawalls, retaining
walls and bridges for ports and municipal clients, evaluated engineered wood products against
building codes, and ran finite element models against lab data.
