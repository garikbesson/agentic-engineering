# Repository Context Loading

This Cursor rule makes the Repository Knowledge Base the primary entry point for project context.

Instead of exploring the repository immediately, Cursor first loads:

`knowledge/README.md`

The README then guides the agent to the Repository Knowledge documents relevant to the current task.

This reduces unnecessary repository exploration and improves architectural understanding before reading source code.

## Installation

Copy `RULE.md` to:

.cursor/rules/repository-context-loading.md