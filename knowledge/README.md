# Knowledge

This directory contains reusable engineering knowledge.

Unlike playbooks or policies, documents in this directory focus on **understanding** rather than **execution**.

The goal is to explain engineering concepts, principles and patterns that help developers make better decisions while building software with AI.

---

# Purpose

Knowledge articles answer questions such as:

- What is this concept?
- Why does it matter?
- When should I use it?
- When should I avoid it?
- How does it relate to other engineering concepts?

The emphasis is on building understanding rather than prescribing a workflow.

---

# What belongs here

Examples include:

- Context Engineering
- Product Workflows
- Feature Specifications
- Memory
- Planning
- Tool Calling
- Multi-Agent Systems
- Model Context
- Human-in-the-Loop

---

# What does NOT belong here

This directory is **not** for:

- step-by-step workflows → `playbooks/`
- engineering decision rules → `policies/`
- reusable document templates → `templates/`
- repository documentation → `docs/`
- early ideas and proposals → `rfcs/`

---

# Writing Guidelines

Every document should answer a real engineering question.

Prefer explaining principles over describing specific tools.

Use examples that can be applied across different domains rather than examples tied to a single product.

A good knowledge article should still be useful even if today's AI tools no longer exist.

---

# Relationship to Other Directories

```text
Knowledge
        ↓
helps engineers understand concepts

Playbooks
        ↓
show how to apply those concepts

Policies
        ↓
help decide when to apply them

Templates
        ↓
provide reusable artifacts

RFCs
        ↓
explore ideas before they become knowledge
```

Understanding should come before execution.

Knowledge provides the foundation that playbooks, policies and templates build upon.
