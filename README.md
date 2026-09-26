# dshiled

I build self-hosted systems and publish what they fail at.

---

## Building

### QA-Robot

Self-hosted governance for AI-generated tests. A QA tool that runs AI output
is a remote code execution engine with extra steps, so QA-Robot scans
generated tests for credential theft, data exfiltration and production side
effects before they execute, then keeps an append-only record of what ran.

Everything stays on your own hardware. No test traffic leaves the network.

`github.com/dshiled/qa-robot` - AGPL-3.0

### Market-systems research

Single-position, session-based strategies with explicit daily and total
drawdown halts, measured against a locked holdout and a Monte-Carlo gate.
The windows that failed are documented next to the ones that passed.
Private, in progress.

---

## How I work

- **Self-hosted first.** No test data and no market data leaves the box.
- **Measured claims only.** Holdout and Monte-Carlo, and the failures ship in
  the README, not just the passing numbers.
- **Append-only evidence** over dashboards and screenshots.
- **Small dependency surface.** Node built-ins and SQLite, no Docker, no cloud
  account, no database server.

---

## Stack

Node.js / TypeScript / Bun - Playwright - SQLite - Python (pandas, FastAPI) -
React
