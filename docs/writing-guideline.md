# Writing Guidelines

These guidelines help keep the repository consistent, reusable and easy to navigate.

---

# Write for Reuse

Prefer examples that are easy to transfer between domains.

When possible:

- use generic engineering examples;
- avoid project-specific terminology;
- avoid product names;
- illustrate principles with multiple domains instead of one concrete application.

A reader should be able to recognize their own product in the example.

---

# Write as an Engineering Handbook

Repository documentation should read like engineering documentation rather than a personal blog.

Prefer:

- Overview
- Motivation
- Guiding Principle
- When to Use
- When to Avoid
- Trade-offs
- Related Topics

Avoid:

- "I think..."
- "I recommend..."
- "In my experience..."
- "Personally..."

The focus should remain on reusable engineering knowledge rather than the author.

---

# Explain Principles Before Tools

Describe engineering ideas independently of any specific AI tool.

Instead of:

> "Cursor should..."

Prefer:

> "An AI coding agent should..."

or

> "The engineering workflow should..."

Tools change quickly. Engineering principles last longer.

---

# Start from Real Engineering Problems

Knowledge should emerge from real engineering work.

Avoid inventing articles around abstract ideas.

A reusable engineering insight should follow this progression:

```text
Engineering Problem
        ↓
Generalization
        ↓
Knowledge Article
```

---

# Keep Articles Focused

Each article should explain one engineering concept well.

Prefer:

- one idea;
- practical examples;
- clear trade-offs;
- links to related topics.

Avoid combining multiple independent concepts into a single article.

---

# Build a Connected Knowledge Base

Articles should not exist in isolation.

Whenever possible, include:

- Related Topics
- Related Playbooks
- Related Policies

The repository should gradually evolve into a connected engineering knowledge base rather than a collection of independent markdown files.