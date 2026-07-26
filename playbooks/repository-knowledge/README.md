# Repository Knowledge Management

Repository Knowledge Management playbooks help AI coding agents build and maintain a reusable understanding of a software repository.

The goal is to reduce repeated repository exploration by keeping a Repository Knowledge Base up to date throughout the project's lifetime.

A Repository Knowledge Base serves as the primary source of repository orientation for future engineering sessions.

## Playbooks

### [Create Repository Knowledge Base](create.md)

Creates a Repository Knowledge Base from an existing repository.

Use this playbook when:

- starting work on a repository that does not yet contain a Repository Knowledge Base;
- introducing Repository Knowledge Management to an existing project.

The playbook inspects the repository, identifies reusable engineering knowledge and creates an initial `knowledge/` directory.

---

### [Update Repository Knowledge Base](update.md)

Updates an existing Repository Knowledge Base after implementation changes.

Use this playbook before opening a pull request or completing a feature.

The playbook reviews recent repository changes and updates only the affected knowledge documents while preserving the existing documentation structure.

## Repository Knowledge

Repository Knowledge should document stable information that helps future engineering sessions understand the repository.

Typical examples include:

- project purpose;
- repository structure;
- architecture;
- major components;
- terminology;
- engineering conventions;
- product workflows;
- implementation boundaries.

Repository Knowledge is intended to describe the current repository, not the history of its development.

Avoid documenting:

- implementation history;
- temporary feature details;
- speculative future designs;
- engineering conclusions.

## Lifecycle

Repository Knowledge Management is intended to become part of the normal engineering workflow.

```text
Create Repository Knowledge Base
            ↓
      Engineering Work
            ↓
Update Repository Knowledge Base
            ↓
Create Pull Request
```