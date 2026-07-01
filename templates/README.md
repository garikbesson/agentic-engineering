# Templates

This directory contains reusable engineering artifacts.

Templates provide a consistent starting point for documents created during the software development process.

Unlike knowledge, playbooks or policies, templates are intended to be copied, adapted and used directly in real projects.

---

# Purpose

Templates answer questions such as:

- What should this document look like?
- Which sections should it contain?
- What information is important to capture?
- How can teams create consistent engineering artifacts?

The goal is to reduce repetitive work while improving consistency.

---

# What belongs here

Examples include:

- Product Workflow
- Feature Specification
- Architecture Decision Record (ADR)
- Task Breakdown
- Bug Report
- Design Proposal
- Planning Prompt
- Review Prompt

---

# What does NOT belong here

This directory is **not** for:

- explaining engineering concepts → `knowledge/`
- describing engineering workflows → `playbooks/`
- defining engineering decision rules → `policies/`
- repository documentation → `docs/`
- ideas that still need discussion → `rfcs/`

---

# Recommended Structure

Every template should include:

- Purpose
- When to Use
- Instructions (if necessary)
- Reusable structure

Templates should contain as little project-specific content as possible.

The goal is to provide a flexible starting point rather than a finished document.

---

# Writing Guidelines

A good template should:

- be easy to copy into a real project;
- encourage consistent engineering practices;
- avoid unnecessary complexity;
- remain applicable across different domains;
- focus on reusable structure rather than examples.

Whenever possible, keep placeholders descriptive rather than prescriptive.

---

# Relationship to Other Directories

```text
Knowledge
        ↓
explains concepts

Playbooks
        ↓
describe workflows

Policies
        ↓
define decision rules

Templates
        ↓
provide reusable artifacts

RFCs
        ↓
propose future ideas
```

Understanding guides execution.

Policies guide decisions.

Templates help engineers produce consistent engineering artifacts.

---

# Guiding Principle

A template should save time without removing engineering thinking.

It should provide structure, not decisions.
