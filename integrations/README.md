# Integrations

Integrations bridge reusable engineering practices and AI coding agents.

While Knowledge and Playbooks define reusable engineering concepts and workflows, Integrations make them directly usable by AI coding agents.

Each integration adapts the same engineering practices to the conventions of a specific tool.

---

# Philosophy

Engineering practices should be tool-independent.

Integrations are intentionally separated from:

- Knowledge
- Playbooks
- Templates

This allows the same engineering workflow to be reused across different AI tools without changing the underlying engineering guidance.

```text
Knowledge
        ↓
Playbook
        ↓
Integration
        ↓
AI Tool
```

---

# Structure

```text
integrations/

    cursor/
        repository-knowledge/

            skills/
                repository-knowledge-management/

            rules/
                repository-context-loading/

    claude-code/
        ...

    codex/
        ...
```

Each integration package is self-contained and typically includes:

- `README.md`
- `manifest.yaml`
- one or more integration artifacts (for example `SKILL.md` or `RULE.md`)

---

# Current Integrations

## Cursor

Currently available:

- [Repository Knowledge Management (Skill)](./cursor/repository-knowledge/skills/repository-knowledge-management/README.md)
- [Repository Context Loading (Rule)](./cursor/repository-knowledge/rules/repository-context-loading/README.md)

Future integrations may support:

- Claude Code
- Codex
- Aider
- Roo Code
- Windsurf
- other AI development tools

---

# Design Principles

An integration should:

- reuse existing Knowledge and Playbooks rather than duplicate them;
- remain specific to a single AI tool;
- be installable independently;
- evolve without changing the underlying engineering practices.

Whenever possible, integrations should contain only tool-specific instructions while keeping engineering knowledge inside the shared Knowledge Base and Playbooks.