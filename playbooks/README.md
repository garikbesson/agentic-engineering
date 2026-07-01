# Playbooks

This directory contains reusable engineering workflows.

Unlike knowledge articles, playbooks focus on **execution** rather than **understanding**.

The goal is to help engineers consistently perform common software engineering tasks while working with AI.

---

# Purpose

Playbooks answer questions such as:

- How should I approach this task?
- What sequence of steps works well?
- Which engineering artifacts should be created?
- What should happen before implementation?
- What should happen afterwards?

A playbook is intended to be followed, adapted and reused.

---

# What belongs here

Examples include:

- Planning a Feature
- Redesigning an Existing User Flow
- Architecture Review
- Code Review
- Bug Investigation
- Refactoring
- Introducing AI into an Existing Project
- Starting a New Project

---

# What does NOT belong here

This directory is **not** for:

- explaining engineering concepts → `knowledge/`
- defining engineering decision rules → `policies/`
- reusable engineering artifacts → `templates/`
- repository documentation → `docs/`
- ideas that still need discussion → `rfcs/`

---

# Recommended Structure

A playbook should typically include:

- Goal
- When to Use
- Prerequisites
- Recommended Workflow
- Expected Outputs
- Common Mistakes
- Related Knowledge
- Related Policies
- Related Templates

Not every playbook needs every section, but each should be practical enough to follow during real development.

---

# Writing Guidelines

A good playbook should:

- solve a real engineering problem;
- describe a repeatable workflow;
- remain independent of any specific product;
- focus on engineering decisions rather than tool-specific instructions;
- be easy to skim and apply.

Prefer checklists, numbered steps and decision points over long explanations.

---

# Relationship to Other Directories

```text
Knowledge
        ↓
explains why

Playbooks
        ↓
explain how

Policies
        ↓
define when

Templates
        ↓
provide reusable artifacts

RFCs
        ↓
explore what might come next
```

Understanding should come before execution.

Execution should lead to consistent engineering outcomes.

---

# Guiding Principle

A playbook should be something an engineer can open while working on a real project and immediately start following.
