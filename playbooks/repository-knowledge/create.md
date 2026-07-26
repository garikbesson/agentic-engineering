# Create Repository Knowledge Base

Your task is to build a reusable Repository Knowledge Base for this repository.

Before making any implementation changes, inspect the repository and create a set of documents that help future engineering sessions quickly understand the project.

> This playbook is self-contained.
>
> The article below explains the reasoning behind the playbook and is intended for readers who want additional background.
>
> - [Start with Orientation](../../knowledge/start-with-orientation.md)

## Objective

Create a Repository Knowledge Base that serves as long-lived engineering documentation for this repository.

The Repository Knowledge Base should help engineers and AI coding agents understand the project before making implementation changes.

The documentation should focus on reusable repository knowledge rather than implementation details of a particular feature.

## Repository Inspection

Inspect the repository before creating the documentation.

Use only information that can be derived from:

- repository structure;
- source code;
- specifications;
- documentation;
- configuration;
- existing implementation.

Do not invent undocumented behavior or product requirements.

When information is uncertain, explicitly state the uncertainty instead of making assumptions.

## Repository Knowledge Base

Create a new top-level directory:

knowledge/

Design the documentation structure that best represents the repository.

The exact document structure is not prescribed.

Instead, organize the documentation around the repository itself.

The Repository Knowledge Base should capture reusable knowledge such as:

- project purpose;
- architecture;
- repository structure;
- major components;
- domain terminology;
- product workflows;
- implementation boundaries;
- engineering conventions;
- important dependencies between components.

Avoid documenting temporary implementation details that are likely to become outdated after a single feature.

The documentation should remain useful across multiple future engineering sessions.

## Documentation Principles

The Repository Knowledge Base should be:

- reusable;
- concise;
- easy to navigate;
- fact-based;
- implementation-oriented.

Avoid:

- feature implementation history;
- speculative architecture;
- future ideas;
- design discussions;
- engineering conclusions.

Document what currently exists.

## Deliverables

Before creating any files:

1. Inspect the repository.
2. Propose the Repository Knowledge Base structure.
3. Explain the purpose of each document.
4. Wait for approval.

After approval:

1. Create the Repository Knowledge Base.
2. Populate every document with repository knowledge.
3. Ensure the documentation is internally consistent.

The Repository Knowledge Base will become the primary source of repository orientation for future engineering sessions.