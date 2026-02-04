# Strategies

Development strategies define the workflow from idea to implementation.

## Available Strategies

| Strategy | Use Case | Artifacts |
|----------|----------|-----------|
| [default.md](./default.md) | Standard projects | PRD → SPECIFICATION |
| rapid.md | Quick prototypes | SPECIFICATION only |
| enterprise.md | Large teams | PRD → ADR → SPECIFICATION |

## Selecting a Strategy

By default, Deft uses `strategies/default.md`. To use a different strategy:

```
Use the rapid strategy for this project.
```

Or specify in `project.md`:

```markdown
## Strategy
Use [strategies/rapid.md](../strategies/rapid.md) for this project.
```

## Creating Custom Strategies

A strategy file defines:

1. **When to use** — project types, team sizes, constraints
2. **Workflow phases** — ordered steps with transition criteria
3. **Artifacts** — what documents are produced
4. **Agent behavior** — how AI should conduct each phase
