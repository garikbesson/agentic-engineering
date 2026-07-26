# Playbooks

This directory contains reusable engineering playbooks.

Playbooks describe repeatable engineering processes that can be executed by engineers, AI coding agents, or both working together.

Unlike knowledge articles, playbooks focus on **execution** rather than **understanding**.

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

### Repository Knowledge Management

- Create Repository Knowledge Base
- Update Repository Knowledge Base

### Implementation

- Plan a Feature
- Implement a Feature
- Refactor Existing Code

### Reviews

- Architecture Review
- Code Review

Additional playbooks should describe repeatable engineering activities rather than project-specific procedures.

---

# What does NOT belong here

This directory is **not** for:

- explaining engineering concepts → `knowledge/`
- defining engineering decision rules → `policies/`
- reusable engineering artifacts → `templates/`
- repository documentation → `docs/`
- ideas that still need discussion → `rfcs/`

---

# Writing Guidelines

A playbook should:

- solve a real engineering problem;
- describe a repeatable engineering process;
- remain independent of any specific product;
- focus on engineering decisions rather than tool-specific instructions;
- be easy to skim and apply.

Each playbook should clearly communicate:

- its objective;
- when it should be used;
- the engineering process to follow;
- important constraints;
- the expected outputs.

The exact document structure is intentionally flexible.

Choose the structure that best communicates the engineering process rather than following a rigid template.

Prefer checklists, numbered steps and decision points over long explanations.

---

# Relationship to Other Directories

```text
Knowledge
        ↓
explains

Playbooks
        ↓
execute

Policies
        ↓
constrain

Templates
        ↓
provide reusable artifacts

RFCs
        ↓
explore future ideas
```

Knowledge explains engineering concepts and principles.

Playbooks describe how engineering work is performed.

Policies define constraints and decision rules.

Templates provide reusable engineering artifacts.

RFCs explore ideas that may later evolve into knowledge, playbooks or policies.

---

# Future Evolution

As the collection grows, multiple playbooks may be composed into higher-level engineering workflows.

For example:

```text
Create Repository Knowledge Base
            ↓
      Engineering Work
            ↓
Update Repository Knowledge Base
            ↓
Create Pull Request
```

A workflow coordinates several playbooks to accomplish a larger engineering objective.

---

# Guiding Principle

A playbook should be something an engineer or AI coding agent can open while working on a real project and immediately start following.