# Charter

Previous personal projects have died from over-engineering, not from lack of interest or skill. This file exists so that the guardrail is something I can be held to rather than something I intended.

It is deliberately short. A long document about avoiding over-engineering would be a joke at its own expense.

## Rules

1. **Timeboxes are real.** Every planning task has one. When it runs out, ship what exists and move on. An unfinished doc that exists beats a perfect one that doesn't.

2. **No abstraction until the second use case.** Not the anticipated second — the actual one. Note the seam in an ADR and write the concrete thing.

3. **No feature enters the MVP without a pain it solves for me this month.** Not "would be useful." Not "every other app has it." A specific thing that annoyed me recently.

4. **Diagrams are for communication, not completeness.** Five diagrams, listed in `diagrams/README.md`. A sixth needs a specific confusion to justify it.

5. **One page means one page.** If a doc needs more, it is probably two docs — or one doc and a decision I haven't made yet.

6. **Deferred is not rejected.** Every good idea I say no to goes in `05-roadmap.md`. The parking lot is what makes saying no survivable.

7. **When two options look close, pick the reversible one.** Cheap to undo beats theoretically better. Spend the real thinking time only on the decisions that are genuinely expensive to reverse — the ledger model is the main one.

8. **Working beats complete.** Something usable end-to-end, however thin, before anything is finished properly.

## When a planning doc is done

**A planning doc is done when it answers its stated question well enough for me to start building — not when it is complete.**

Every planning artifact exists to unblock a decision or a piece of work. Once it does that, it is finished, regardless of what is still missing.

Practical tests:

- Can I take the next step without reopening this file? → Done.
- Am I adding detail that no upcoming task needs? → Stop. That is scope creep wearing a documentation costume.
- Am I still writing because it feels unfinished rather than because something is blocked? → Stop.
- Would deleting this file make any decision harder? → If no, delete it.

Docs are living files. Something genuinely missing can be added when the gap actually bites. Writing it now, speculatively, is the failure mode this rule exists to prevent.

---

*Reviewed at P8. If a rule here was quietly ignored throughout, it was the wrong rule — fix it or drop it, don't pretend.*
