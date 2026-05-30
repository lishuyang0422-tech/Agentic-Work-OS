# Agent Compatibility

## Single Source Of Truth

`AGENTS.md` is the single source of truth for agent behavior in this starter.

This project does not maintain separate official rule files for every AI tool.

## Why

Different agent tools change quickly. Duplicating rules across many tool-specific files creates drift.

The safer pattern:

1. keep the core behavior in `AGENTS.md`
2. let any file-aware agent read it
3. add lightweight notes for tool-specific setup only when needed

## Suggested Use

For any agent tool:

1. open the repository
2. ask the agent to read `AGENTS.md`
3. ask it to read `System/Core/`
4. ask it to run one demo

Example prompt:

```text
Read AGENTS.md and System/Core first. Then explain this workspace and run examples/agentic-work-os-research-demo.
```

## Community Notes

Community-maintained compatibility notes are welcome, but they should not duplicate the full rules. They should point back to `AGENTS.md`.
