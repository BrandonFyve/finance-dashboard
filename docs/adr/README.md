# Architecture Decision Records

Each file records one decision: what was decided, what else was considered, and what it costs.

Written in the [Nygard format](https://cognitect.com/blog/2011/11/15/documenting-architecture-decisions) — see [`template.md`](template.md).

## Rules

- **Numbered and immutable.** Once an ADR is accepted it isn't edited. If the decision changes, write a new ADR that supersedes it and mark the old one `Superseded by ADR-XXXX`.
- **Consequences are mandatory.** An ADR without a stated cost is a decision that wasn't really made.
- **Short.** One page. If it needs more, the decision is probably two decisions.

## Index

| ADR | Decision | Status |
|---|---|---|
| 0000 | Record architecture decisions | — |
| 0001 | Build from scratch vs fork | — |
| 0002 | MVP shape | — |
| 0003 | Ledger data model | — |
| 0004 | Multi-currency and FX | — |
| 0005 | Data ingestion strategy | — |
| 0006 | Tech stack | — |
| 0007 | LLM trust boundary | — |
| 0008 | LLM providers and local fallback | — |
| 0009 | Hosting, auth and secrets | — |
| 0010 | Primary interface split | — |

Status values: `Proposed` · `Accepted` · `Superseded by ADR-XXXX`
