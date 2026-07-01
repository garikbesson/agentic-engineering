# Repository Structure

This repository is organized around a simple principle:

> **Every top-level directory has a single, clearly defined responsibility.**

The goal is to make it obvious where new knowledge belongs—for both humans and AI coding agents.

---

# Directory Overview

| Directory | Purpose | Primary Question |
|-----------|---------|------------------|
| `docs/` | Repository documentation | How is this repository organized? |
| `knowledge/` | Engineering concepts and principles | What is this? |
| `playbooks/` | Practical engineering workflows | How do I do this? |
| `policies/` | Engineering decision rules | When should I do this? |
| `templates/` | Reusable engineering artifacts | What should this artifact look like? |
| `rfcs/` | Ideas under discussion | Should this become part of the knowledge base? |

---

# Responsibility of Each Directory

## docs/

Contains documentation **about the repository itself**.

Examples:

- repository structure;
- writing guidelines;
- contribution guidelines;
- style guides.

This directory should never contain engineering knowledge.

---

## knowledge/

Explains engineering concepts, principles and patterns.

Knowledge answers questions such as:

- What is this?
- Why does it matter?
- How does it relate to other concepts?

Knowledge builds understanding.

---

## playbooks/

Describe repeatable engineering workflows.

Playbooks answer questions such as:

- How should I approach this task?
- What sequence of steps works well?

Playbooks help engineers execute.

---

## policies/

Capture engineering decision rules.

Policies answer questions such as:

- When should I use this workflow?
- When should I stop and ask for clarification?
- When is an architectural decision required?

Policies help engineers decide.

---

## templates/

Provide reusable engineering artifacts.

Examples include:

- Product Workflow
- Feature Specification
- ADR
- Task Breakdown

Templates help engineers create consistent artifacts.

---

## rfcs/

RFCs are ideas that are still evolving.

They exist to encourage discussion before new concepts become part of the repository.

Not every RFC becomes knowledge.

Some are accepted.

Some are revised.

Some are rejected.

---

# How New Knowledge Enters the Repository

Most documents begin with a real engineering problem.

```text
Real Project
        ↓
Engineering Problem
        ↓
Engineering Decision
        ↓
Generalization
        ↓
RFC (optional)
        ↓
Knowledge
        ↓
Playbook
        ↓
Policy
```

Not every idea follows every stage.

The important part is that reusable knowledge grows from practical engineering experience.

---

# Choosing the Right Directory

Before creating a new document, ask yourself:

### Am I documenting the repository?

→ `docs/`

---

### Am I explaining a concept?

→ `knowledge/`

---

### Am I describing a workflow?

→ `playbooks/`

---

### Am I defining a decision rule?

→ `policies/`

---

### Am I creating a reusable artifact?

→ `templates/`

---

### Am I exploring an unfinished idea?

→ `rfcs/`

---

# Design Principles

The repository evolves according to a few simple principles.

## Single Responsibility

Every directory should have one clear purpose.

Avoid overlapping responsibilities.

---

## Generalization

Knowledge should not depend on a specific product.

Whenever possible, extract reusable engineering principles from real-world experience.

---

## Practicality

Every document should help solve a real engineering problem.

Avoid theory that cannot be applied.

---

## Evolution

The structure is expected to evolve.

New directories should only be introduced when they represent a genuinely new responsibility rather than a different way of organizing existing content.
