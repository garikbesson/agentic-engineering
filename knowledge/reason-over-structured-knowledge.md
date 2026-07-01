# # Reason Over Structured Knowledge

**Tags:** AI, Architecture, Knowledge Representation, Reasoning

**Related:** [`knowledge/product-workflows-vs-feature-specifications.md`](../knowledge/product-workflows-vs-feature-specifications.md)

---

# Overview

Many AI applications follow a simple pipeline:

```text
Input
    ↓
LLM
    ↓
Output
```

This approach works well for simple tasks but becomes increasingly difficult to maintain as products grow.

A single prompt becomes responsible for:

- understanding the input;
- extracting relevant information;
- reasoning;
- generating the final artifact.

As prompts grow, outputs become less predictable, intermediate reasoning becomes invisible, and valuable knowledge is discarded after each request.

---

# A Better Approach

> **Generate artifacts only after reasoning has been performed on structured knowledge.**

Instead of generating artifacts directly from raw inputs, split the process into four distinct stages.

```text
Raw Input
        ↓
Knowledge Extraction
        ↓
Structured Knowledge

Target Input
        ↓
Knowledge Extraction
        ↓
Structured Knowledge

Structured Reasoning
        ↓
Generated Artifact
```

This separates four different responsibilities:

- extraction;
- representation;
- reasoning;
- generation.

Each stage becomes independently understandable, testable and reusable.

---

# Why It Matters

Structured knowledge can be:

- inspected;
- validated;
- reused;
- enriched over time;
- compared with other knowledge sources.

Generated artifacts usually cannot.

For long-lived products, structured knowledge often becomes a much more valuable asset than the documents originally used to create it.

---

# Example

Consider a system that generates implementation plans.

A naive implementation might look like this:

```text
Requirements
        +
Existing Codebase
        ↓
LLM
        ↓
Implementation Plan
```

Instead, transform both inputs into structured knowledge.

```text
Requirements
        ↓
Requirement Knowledge

Existing Codebase
        ↓
Architecture Knowledge

Requirement Knowledge
        +
Architecture Knowledge
        ↓
Reasoning
        ↓
Gap Analysis
        ↓
Implementation Plan
```

Now the system can answer questions such as:

- Which requirements are already supported?
- Which components are affected?
- Which capabilities are missing?
- Which assumptions need clarification?
- Which architectural decisions must be revisited?

Instead of immediately generating a plan, the system first builds an understanding of the problem.

---

# Benefits

## Reusable Knowledge

Structured knowledge can be reused across many generated artifacts.

For example:

- implementation plans;
- technical specifications;
- architecture proposals;
- migration plans;
- documentation.

The same knowledge can support many outputs.

---

## Explainable Reasoning

The system can explain *why* something was generated.

Instead of saying:

> "The model decided to include this."

it can explain which parts of the structured knowledge led to that decision.

---

## Gap Detection

Comparing structured knowledge makes missing information explicit.

Instead of returning a generic confidence score, the system can identify:

- missing information;
- conflicting information;
- unsupported requirements;
- assumptions requiring clarification.

This enables targeted follow-up questions before generation.

---

## Continuous Learning

Every interaction can improve the underlying knowledge rather than only the generated artifact.

Over time, the knowledge base becomes increasingly complete while generation becomes more accurate.

---

# When to Use

This pattern works well when:

- multiple artifacts are generated from the same information;
- knowledge evolves over time;
- reasoning is more important than text generation;
- explainability matters;
- users continuously refine their data.

---

# When Direct Generation Is Enough

Direct prompting is usually sufficient for:

- summarization;
- translation;
- rewriting;
- one-off content generation;
- disposable outputs.

Introducing structured knowledge adds complexity.

Only introduce that complexity when it creates long-term value.

---

# General Pattern

A useful mental model is:

```text
Documents
        ↓
Knowledge

Knowledge
        ↓
Reasoning

Reasoning
        ↓
Artifacts
```

The artifact should be the result of reasoning—not the place where reasoning happens.

---

# Guiding Principle

Treat structured knowledge as the primary asset.

Treat generated artifacts as one possible representation of that knowledge.
