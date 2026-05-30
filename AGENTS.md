# AGENTS.md

## What This Workspace Is

This is an Agentic Work OS starter workspace.

It is not a normal code repository and not a private knowledge dump. It is a local-first file structure that helps AI agents work with humans over time.

## Required Reading Order

When entering this workspace, read:

1. `README.md`
2. `System/Core/AI_RULES.md`
3. `System/Core/CURRENT_STATE.md`
4. `System/Core/NODE_IDENTITY.md`

If the task involves a demo, also read the relevant folder in `examples/`.

## Core Behavior

- Read before acting.
- Use the local file structure as shared state.
- Keep project work in `System/Active_Projects/`.
- Keep raw inputs in `input/` unless the task says otherwise.
- Put user-facing outputs in `output/`.
- Record important changes in `System/System_Log/SYSTEM_CHANGE_LOG.md`.
- Do not invent private context that is not present in the workspace.

## Safety Rules

- Do not ask users to place secrets in this repository.
- Do not commit private data, customer records, credentials, personal profiles, or confidential project files.
- Do not treat demos as real business data.
- Do not create hidden automation or remote publishing steps without explicit user approval.

## Agent Handoff Rule

If another agent must continue your work, leave enough context in files:

- current goal
- what changed
- remaining questions
- next recommended action

The system should survive a broken chat thread.
