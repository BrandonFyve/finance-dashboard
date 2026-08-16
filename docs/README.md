# Documentation

Everything here is written to a deliberate bar: **good enough to start building**, not complete. See [`00-charter.md`](00-charter.md) for the rules this project holds itself to.

Unchecked items don't exist yet.

## Decisions

Numbered ADRs, in [`adr/`](adr/). These are the spine of the project — if you only read one thing here, read these.

ADR-0000 records the decision to keep ADRs at all. Ten further decisions are already identified; they will be written when they are made.

- [x] [ADR-0000](adr/adr_0000-record-architecture-decisions.md) — Record architecture decisions
- [ ] ADR-0001 — Build from scratch vs fork
- [ ] ADR-0002 — MVP shape
- [ ] ADR-0003 — Ledger data model
- [ ] ADR-0004 — Multi-currency and FX
- [ ] ADR-0005 — Data ingestion strategy
- [ ] ADR-0006 — Tech stack
- [ ] ADR-0007 — LLM trust boundary
- [ ] ADR-0008 — LLM providers and local fallback
- [ ] ADR-0009 — Hosting, auth and secrets
- [ ] ADR-0010 — Primary interface split

## Documents

| | Document | What question it answers |
|---|---|---|
| [ ] | `00-charter.md` | What stops this from being over-engineered? |
| [ ] | `01-jobs-to-be-done.md` | What do I actually need this to do for me? |
| [ ] | `02-vision-and-scope.md` | What is this, and what is it not? |
| [ ] | `03-mvp-definition.md` | What is in the first version — and explicitly out? |
| [ ] | `04-user-stories.md` | What does "working" mean, concretely? |
| [ ] | `05-roadmap.md` | Where do good ideas go so they stop competing with the MVP? |
| [ ] | `06-tax-rules-schema.md` | How are tax rates encoded so they survive each Budget? |
| [ ] | `07-ai-features.md` | Which AI capabilities are real, and which are gimmicks? |
| [ ] | `08-pii-redaction.md` | What gets stripped before anything reaches a model? |
| [ ] | `09-mcp-surface.md` | What tools does the ledger expose to an LLM? |
| [ ] | `10-ai-evaluation.md` | How do I know the AI is actually any good? |
| [ ] | `11-threat-model.md` | What realistically goes wrong, and what do I do about it? |
| [ ] | `12-code-structure.md` | Where does code live, and what may import what? |
| [ ] | `13-testing-strategy.md` | What gets tested — and what deliberately doesn't? |
| [ ] | `14-development.md` | How do I run this, and how do I know it broke? |
| [ ] | `15-risks.md` | What can't be answered yet, and what would warn me? |

## Diagrams

Five, planned in [`diagrams/`](diagrams/). Mermaid where possible, so they live in git and stay reviewable in diffs. None are written yet.

- [ ] `c4-context.md` — the system and everything it touches
- [ ] `c4-container.md` — the deployable pieces and how they talk
- [ ] `erd.md` — the domain model
- [ ] `transaction-lifecycle.md` — ingest → categorise → persist
- [ ] `data-flow.md` — every path data takes off the host

**Deliberately excluded:** C4 component and code levels, personas, journey maps, formal requirements specs, full sequence coverage. These go stale within a week of writing code and are exactly the over-engineering the charter exists to prevent.

## Research

- [ ] `research/` — competitive landscape review that seeded this project, plus verification notes

> Anything that lands in `research/` is a **snapshot**, not current fact. Tax figures change at each Budget and aggregator terms shift fast. Check the date header before relying on anything in there.
