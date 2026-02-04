# Specification Generation (Legacy)

> **Note:** This file is maintained for backwards compatibility.
> For the full workflow, see [strategies/default.md](../strategies/default.md).

Quick reference for the DEFaulT strategy's specification phase.

Legend (from RFC2119): !=MUST, ~=SHOULD, ≉=SHOULD NOT, ⊗=MUST NOT, ?=MAY.

## Quick Start

```
I want to build [project name] that has the following features:
1. [feature]
2. [feature]
```

This triggers the [DEFaulT strategy](../strategies/default.md):
1. **Interview** → gather requirements
2. **PRD.md** → document what to build
3. **SPECIFICATION.md** → document how to build it

## Full Documentation

See [strategies/default.md](../strategies/default.md) for:
- Interview process and question areas
- PRD structure and guidelines
- SPECIFICATION structure and guidelines
- Transition criteria between phases

## Quick Reference

### Interview Rules
- ! Ask ONE question per step
- ! Include "other" option
- ! Indicate RECOMMENDED choice
- ⊗ Multiple questions at once

### Output Rules
- ! Generate PRD.md first (what)
- ! Generate SPECIFICATION.md second (how)
- ! Use RFC 2119 language
- ! Mark all dependencies
- ! Design for parallel work
- ⊗ Write code

### After Completion
```
implement SPECIFICATION.md
```
