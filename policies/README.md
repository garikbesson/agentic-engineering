# Policies

This directory contains engineering decision rules.

Unlike knowledge articles that explain concepts or playbooks that describe workflows, policies help engineers decide **when** a particular practice should be applied.

The goal is to make engineering decisions more consistent for both humans and AI coding agents.

---

# Purpose

Policies answer questions such as:

- When should this workflow be used?
- When should an agent stop and ask for clarification?
- When is a Feature Specification required?
- When is an ADR worth creating?
- When should human approval be required?

Policies reduce ambiguity by defining consistent decision rules.

---

# What belongs here

Examples include:

- Planning Policy
- Context Management Policy
- Code Review Policy
- Refactoring Policy
- Testing Policy
- Architecture Decision Policy
- Human Approval Policy

---

# What does NOT belong here

This directory is **not** for:

- explaining engineering concepts → `knowledge/`
- describing engineering workflows → `playbooks/`
- reusable engineering artifacts → `templates/`
- repository documentation → `docs/`
- ideas that still need discussion → `rfcs/`

---

# Recommended Structure

A policy should typically include:

- Purpose
- Decision Rule
- Rationale
- Exceptions
- Related Knowledge
- Related Playbooks
- Related Templates

The focus should be on helping engineers make better decisions, not documenting every possible edge case.

---

# Writing Guidelines

A good policy should:

- define a clear decision;
- explain why the rule exists;
- describe known exceptions;
- remain independent of specific tools or products;
- be simple enough to apply during everyday development.

Policies should guide engineering decisions, not replace engineering judgment.

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

Understanding should guide execution.

Policies help engineers choose the right workflow at the right time.

---

# Guiding Principle

A policy should help answer a real engineering decision that would otherwise depend on personal preference or inconsistent judgment.
