# Product Workflows vs Feature Specifications

> Learn to recognize whether you're defining how a product works or how a single feature behaves.

---

## Why This Matters

One of the most common planning mistakes is starting a Feature Specification before the product itself has been clearly described.

When this happens, Feature Specifications gradually become responsible for:

- describing the overall user journey;
- defining product concepts;
- introducing shared terminology;
- documenting business rules unrelated to a single feature.

As the product grows, this leads to duplicated documentation, inconsistent behavior and poor context for both humans and AI coding agents.

Separating Product Workflows from Feature Specifications creates a clear engineering structure where each document has a single responsibility.

---

# Product Workflow

A Product Workflow describes how users achieve a goal across the entire product.

It focuses on the journey rather than individual implementation details.

A Product Workflow should answer questions like:

- What is the user's overall goal?
- What major stages exist?
- How does information move through the system?
- Which concepts remain stable across multiple features?

## Example

```
Create Account
        ↓
Verify Email
        ↓
Create First Project
        ↓
Invite Team Members
        ↓
Collaborate
```

Notice that this workflow does not describe individual screens or UI components.

It describes how the product works.

---

# Feature Specification

A Feature Specification describes a single capability within an existing Product Workflow.

It should answer questions like:

- What problem does this feature solve?
- How should it behave?
- What are the acceptance criteria?
- What edge cases should be handled?

## Example

Feature:

```
Invite Team Members
```

Questions answered by the Feature Specification:

- Who can send invitations?
- Can invitations expire?
- What happens if the email already belongs to an existing user?
- Can invitations be revoked?

Notice that the specification does **not** redefine the onboarding journey.

---

# How to Decide Which Document You Need

Ask yourself one question.

> Am I describing how the product works?

If the answer is **yes**, you probably need a Product Workflow.

---

> Am I describing how one capability should behave?

If the answer is **yes**, you probably need a Feature Specification.

---

# Relationship

```
Product Vision
        ↓
Product Workflow
        ↓
Feature Specifications
        ↓
Implementation Tasks
        ↓
Code
```

Each level provides context for the level below it.

Avoid duplicating information between them.

---

# Common Mistakes

## Writing the Product Workflow inside a Feature Specification

Instead of defining one capability, the document starts describing the entire product.

---

## Putting implementation details into the Product Workflow

A Product Workflow should remain stable even if the implementation changes.

---

## Duplicating business rules

Shared concepts belong in Product Workflows.

Feature Specifications should reference them instead of redefining them.

---

# Practical Checklist

Before writing a Feature Specification, ask:

- Has the overall product workflow already been defined?
- Does this document describe a single capability?
- Can another feature reuse the same Product Workflow?
- Am I accidentally introducing product-level concepts here?

If several answers are **no**, start by defining the Product Workflow instead.

---

# Key Takeaways

- Product Workflows describe how the product works.
- Feature Specifications describe how one capability behaves.
- Product Workflows provide context for Feature Specifications.
- Feature Specifications should not become product documentation.
- A clear separation improves maintainability and gives AI coding agents better context.
