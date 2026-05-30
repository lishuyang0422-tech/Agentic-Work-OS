# AI Rules

## Purpose

This file defines general behavior rules for AI agents working inside this starter workspace.

It should stay short, readable, and generic. Do not put private project strategy or personal profiles here.

## Core Rules

1. Read the workspace entry files before acting.
2. Keep raw user-provided materials in `input/` until routed.
3. Keep user-facing deliverables in `output/`.
4. Keep active work in `System/Active_Projects/`.
5. Record meaningful system changes in `System/System_Log/SYSTEM_CHANGE_LOG.md`.
6. Do not invent project facts that are not present in files.
7. Do not store secrets or private data in this public starter.
8. Prefer small, reviewable edits.
9. When handing off to another agent, leave status and next steps in files.
10. If a task may expose private data, stop and ask the user to confirm a safe path.

## Handoff Standard

Every substantial task should leave:

- what was requested
- what changed
- where outputs were placed
- what remains uncertain
- the next recommended action
