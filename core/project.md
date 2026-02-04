# Deft Framework Project

Legend (from RFC2119): !=MUST, ~=SHOULD, ≉=SHOULD NOT, ⊗=MUST NOT, ?=MAY.

**⚠️ See also**: [main.md](../main.md) | [taskfile.md](../tools/taskfile.md)

## Principles (Non-Negotiable)

<!-- These govern ALL decisions. Amend formally, not casually. -->

- ! **Lazy Loading** — Only read files relevant to current task
- ! **Layer Precedence** — More specific rules override general ones (user > project > language > tool > main)
- ! **Spec-Driven** — Specifications drive implementation, not the reverse
- ! **Test-First** — No implementation without tests
- ⊗ **Premature Abstraction** — No wrappers or abstractions without proven need
- ⊗ **Future-Proofing** — Build for now, not hypothetical futures

<!-- Small team: keep 3-5 principles. Large org: expand into detailed articles. -->

---

## Project Configuration

**Tech Stack**: Pure Markdown (.md files)

**Project Type**: Agent Framework / Documentation System

**Purpose**: A layered framework for AI-assisted development with consistent standards and workflows

**Strategy**: [strategies/default.md](../strategies/default.md)

## 📋 Workflow

```bash
task validate      # Validate all markdown files
task lint          # Lint markdown files
task build         # Package framework for distribution
task clean         # Clean generated artifacts
```

## 📁 Directory Structure

- `core/` - Core framework files (user.md, project.md)
- `coding/` - Coding standards (coding.md, testing.md)
- `languages/` - Language-specific standards (python.md, go.md, typescript.md, cpp.md)
- `interfaces/` - Interface type guidelines (cli.md, rest.md, tui.md, web.md)
- `tools/` - Tool-specific guidelines (taskfile.md, telemetry.md)
- `scm/` - Version control (git.md, github.md)
- `swarm/` - Multi-agent coordination patterns
- `strategies/` - Development strategies (default.md, etc.)
- `templates/` - Templates and examples for specifications
- `meta/` - Meta/process files (lessons.md, ideas.md, suggestions.md)

## Standards

**Documentation Quality:**
- ! All filenames use hyphens, not underscores
- ! Use RFC2119 notation (!=MUST, ~=SHOULD, ≉=SHOULD NOT, ⊗=MUST NOT, ?=MAY)
- ~ Keep files focused and modular
- ~ Cross-reference related documents

**Version Control:**
- ! Use Conventional Commits
- ! Never force-push without permission
- ~ Create backup/ directory for significant refactors
