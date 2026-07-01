# Repository Documentation

This directory contains documentation **about this repository**, not about Agentic Engineering itself.

The documents here define how the knowledge base is organized, maintained and evolved over time.

If you're looking for engineering concepts, workflows or policies, start with the top-level directories such as `knowledge/`, `playbooks/`, `policies/`, `templates/` or `rfcs/`.

---

# Purpose

The goal of this documentation is to keep the repository consistent as it grows.

It defines:

- writing standards;
- repository structure;
- contribution guidelines;
- content organization;
- naming conventions;
- repository-level decisions.

---

# Repository Structure

```text
docs/
    ↓
defines how the repository is organized

knowledge/
    ↓
explains engineering concepts and principles

playbooks/
    ↓
describe practical engineering workflows

policies/
    ↓
define engineering decision rules

templates/
    ↓
provide reusable engineering artifacts

rfcs/
    ↓
incubate ideas before they become knowledge
```

Each directory has a single responsibility.

Keeping responsibilities separate makes the repository easier to navigate for both humans and AI coding agents.

---

# Current Documents

## [Repository Structure](repository-structure.md)

Explains how the repository is organized.

Topics include:

- responsibilities of each top-level directory;
- how new knowledge enters the repository;
- how to choose the right location for new content;
- design principles behind the repository structure.

---

## [Writing Guidelines](writing-guideline.md)

Defines how new content should be written.

Topics include:

- writing style;
- choosing examples;
- generalizing product-specific experience;
- keeping documents reusable across domains.

---

# Guiding Principle

Repository documentation describes **how to build the knowledge base**.

The knowledge base itself describes **how to build better software**.

Keeping these concerns separate helps both humans and AI agents understand where new information belongs.

---

# Contributing

Before creating new content, ask yourself what you're actually writing.

- Documentation about the repository → `docs/`
- Reusable engineering knowledge → `knowledge/`
- Practical engineering workflows → `playbooks/`
- Engineering decision rules → `policies/`
- Reusable engineering artifacts → `templates/`
- Ideas that still need discussion → `rfcs/`
