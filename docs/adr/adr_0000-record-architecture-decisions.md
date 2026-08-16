# ADR-0000 — Record architecture decisions

**Status:** Accepted
**Date:** 2026-08-16

## Context

This is a solo project built in evenings and weekends, with gaps between sessions. Two problems follow from that.

The first is memory. Decisions made in one session are invisible by the next month. Without a record, past decisions get silently re-litigated, or worse, quietly contradicted — a data model chosen for one reason gets extended in a way that breaks that reason, because the reason was never written down.

The second is that this repo is a portfolio piece. The code will eventually show *what* was built. It will not show what else was considered, or what the choice cost. That reasoning is usually the more interesting thing, and it is normally invisible to anyone reading a finished repo.

Both problems are solved by the same cheap habit: write the decision down when it is made, in a file, in the repo, next to the code it constrains.

## Options considered

**Nothing — rely on commit messages and memory.** Free. Commit messages record what changed, not what was rejected and why. Memory does not survive a three-week gap.

**A single running decisions document.** One file, append-only. Simple, but it grows into something nobody reads, and there is no natural unit to link to from an issue or a code comment.

**Numbered ADRs in the Nygard format.** One file per decision, immutable once accepted, superseded rather than edited. Standard enough that reviewers recognise it immediately. Some ceremony, but the format is four headings and one page.

**A heavier format (MADR, Y-statements, decision records with formal criteria matrices).** More rigour than a single-developer project can sustain. Would become the thing that stops decisions being recorded at all.

## Decision

Use numbered ADRs in the lightweight Nygard format, stored in `docs/adr/`, one file per decision, using [`template.md`](template.md).

Rules:

- **Numbered sequentially and immutable.** Once accepted, an ADR is not edited. If a decision changes, write a new ADR and mark the old one `Superseded by ADR-XXXX`. The history of a changed mind is itself worth keeping.
- **Consequences are mandatory.** An ADR with no stated cost is a decision that was not really made — it is a preference with a paragraph attached.
- **One page.** If it needs more, it is probably two decisions.
- **Written when the decision is made**, not reconstructed later. A reconstructed ADR records the justification, not the reasoning, and those are different things.

Ten decisions are already identified in the planning project (ADR-0001 through ADR-0010). Others will be written as they arise, including during implementation.

## Consequences

**Good:**

- Decisions survive the gaps between working sessions.
- A reviewer can read `docs/adr/` and understand the shape of the project without reading any code.
- Linking an ADR from a code comment gives future-me the reason for something that otherwise looks arbitrary.
- Writing the Consequences section forces the trade-off to be named, which occasionally changes the decision.

**Costs:**

- Roughly 30–45 minutes per significant decision. Against a project that has previously died from over-engineering, this is a real tax and needs watching.
- Risk of ADRs becoming a substitute for progress. Mitigated by the one-page limit and the timeboxes in the charter.
- Risk of the log going stale — decisions made in code but never recorded. There is no automated defence against this; it depends on the habit holding.

**Accepted risk:** the log will probably be incomplete for small decisions made mid-implementation. That is fine. The bar is "would I want to know why, in six months" — not "every choice is documented."
