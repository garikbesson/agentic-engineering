# Start With Orientation, Not Exploration

## Overview

Large engineering systems become difficult to navigate when humans or AI agents begin by exploring individual files.

Instead, every engineering system should provide a clear entry point.

The goal is not to reduce information.

The goal is to provide orientation.

Orientation is not documentation for its own sake.

Its purpose is to create a reusable mental model of the repository that can be shared across engineering sessions.

---

## Exploration

```
Repository

↓

Search

↓

Search

↓

Open file

↓

Search again
```

Exploration is reactive.

The agent only learns after reading many files.

---



## Orientation

```
Repository

↓

Repository Overview

↓

Architecture

↓

Navigation

↓

Relevant Context

↓

Implementation
```

Orientation should not be treated as a one-time activity.

Whenever possible, the understanding gained during orientation should be captured as reusable Repository Knowledge.

Unlike temporary session context, Repository Knowledge becomes a long-lived engineering asset that can support future engineering work.

---



## Examples

Repository orientation may be provided through one or more engineering artifacts.

Examples include:

- Repository Knowledge Base
- README
- Architecture Overview
- Module Index
- Repository Structure
- Knowledge Index
- Start Here
- Onboarding Guide

---



## Why It Matters

Orientation helps both humans and AI agents:

- build a mental model faster;
- reduce unnecessary search;
- avoid incorrect assumptions;
- find relevant context sooner;
- make better engineering decisions.

Over time, repository orientation can evolve into a reusable engineering asset rather than disposable documentation.

A well-maintained Repository Knowledge Base can support:

- engineering implementation;
- debugging;
- onboarding;
- architectural reviews;
- roadmap planning;
- engineering task generation.

Repository orientation is therefore not only a way to start engineering sessions—it can become shared engineering knowledge that evolves together with the project.

---



## Guiding Principle

Every engineering system should have a clearly defined entry point.

Reading should begin with understanding the system—not searching through it.

Repository orientation should create reusable knowledge rather than temporary context.

---



## Research Status

This engineering principle is currently being evaluated through real-world engineering projects.

Initial experiments suggest that repository orientation provides value beyond implementation by creating reusable engineering knowledge that benefits both AI agents and human engineers.

Further research is ongoing to better understand:

- which repository artifacts provide the highest long-term value;
- how Repository Knowledge should evolve as software changes;
- how Repository Knowledge can be maintained automatically;
- which engineering tasks benefit most from repository orientation.

