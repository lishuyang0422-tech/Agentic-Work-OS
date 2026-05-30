# Reference Card: What Is Agentic-Work-OS?

## One-Sentence Definition

Agentic-Work-OS is a local-first workspace protocol that helps AI agents understand rules, share project state, route inputs, create outputs, and hand work off across threads or models.

## Why It Exists

Normal AI chats are powerful but fragile. They keep too much context inside a single conversation. When that conversation breaks, grows too long, or needs to be replaced by another model, work continuity suffers.

Agentic-Work-OS moves the most important working context into local files.

## Core Mechanisms

- `AGENTS.md`: tells agents how to behave.
- `System/Core/`: stores rules, state, and workspace identity.
- `input/`: receives raw materials.
- `output/`: stores user-facing deliverables.
- `System/Active_Projects/`: keeps ongoing project context.
- `System/Resources/`: stores reusable references.
- `System/System_Log/`: records meaningful changes.

## What This Demo Shows

This demo turns research notes into a reference card. In doing so, it demonstrates the core loop:

1. input enters the workspace
2. the agent reads rules and state
3. the agent synthesizes an output
4. the output can be reviewed or reused
5. another agent can continue from the files

## Practical Value

The system reduces context loss, supports multi-agent collaboration, and makes AI work easier to inspect.
