# Personal Finance Dashboard

> **Status: planning.** No code yet. This repo currently holds design decisions and documentation. See [Current state](#current-state) below.

An AI-first personal finance app for a UK/Scotland context. Self-hosted, single user, built as a personal tool and a portfolio piece.

## The idea

Three things that mainstream personal finance apps don't combine:

1. **A clean, event-sourced ledger** — auditable transaction history rather than a mutable list of rows.
2. **A Scotland-specific tax engine** — Scottish taxpayers face six income tax bands and marginal-rate cliffs that don't exist elsewhere in the UK, including roughly 69.5% in the £100k–£125,140 personal allowance taper zone. No mainstream app encodes this.
3. **AI as an interface, not a feature** — natural-language querying over your own ledger, and an MCP server so the data is reachable from any LLM client, rather than a chat window bolted onto a dashboard.

Whether all three make it into the first version is [an open decision](docs/adr/).

## Current state

Planning is tracked in Linear. The work is sequenced across nine phases, P0 → P8, ending with the implementation backlog.

| Phase | Focus | Status |
|---|---|---|
| P0 | Ground rules and repo | In progress |
| P1 | Discovery and feature triage | Not started |
| P2 | Product definition | Not started |
| P3 | Architecture and data design | Not started |
| P4 | AI architecture | Not started |
| P5 | Security, privacy and data handling | Not started |
| P6 | Interface and UX definition | Not started |
| P7 | Delivery readiness | Not started |
| P8 | Planning review and backlog cut | Not started |

Start at [`docs/`](docs/) for the artifact index, or [`docs/adr/`](docs/adr/) for the decisions.

## Why the planning is visible

This repo is deliberately public from the planning phase rather than from first commit. Two reasons:

- **For me:** previous personal projects have died from over-engineering. Writing the reasoning down — and timeboxing it — is the guardrail. See [`docs/00-charter.md`](docs/00-charter.md).
- **For anyone reviewing it:** the decisions and their trade-offs are usually the interesting part, and they are normally invisible by the time a repo is worth looking at.

## Not yet written

Setup instructions, architecture overview, and screenshots land in P7, once there is something to run. This README gets rewritten then.

## Licence

MIT — see [LICENSE](LICENSE).

> **Note:** this is provisional. If [ADR-0001](docs/adr/) lands on forking an AGPLv3 project (Maybe/Sure), MIT is not available and this repo must be AGPLv3 too. Actual Budget (MIT) and building from scratch leave the choice open.

---

*This is a personal project. Nothing here is tax or financial advice.*
