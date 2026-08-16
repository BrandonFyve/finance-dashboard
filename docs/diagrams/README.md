# Diagrams

Mermaid, in markdown files, so they render on GitHub and stay reviewable in diffs. A diagram that lives in a design tool goes stale silently; one that lives in git goes stale visibly.

## Five diagrams, and no more

| File | Level | Answers |
|---|---|---|
| `c4-context.md` | C4 L1 | What is this system and what does it touch? |
| `c4-container.md` | C4 L2 | What are the deployable pieces and how do they talk? |
| `erd.md` | — | What are the entities and how do they relate? |
| `transaction-lifecycle.md` | — | What happens to a transaction from import to stored balance? |
| `data-flow.md` | — | What data leaves this host, and to where? |

**C4 stops at Level 2.** Component and code-level diagrams describe things the code already describes, and they're wrong within a week. If you want to know what a module does, read the module.

**One sequence diagram, not a set.** `transaction-lifecycle.md` covers the hottest path. Other flows get diagrams only if a specific confusion demands one.

## Conventions

- Every external system on a C4 diagram has a stated reason for being there.
- Anywhere data crosses the trust boundary to a third-party LLM, mark it. That boundary is the point of `data-flow.md` and should be visible on the container diagram too.
