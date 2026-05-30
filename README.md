# Agentic-Work-OS

**[简体中文](README.zh-CN.md) | English**

> 多 AI 协作工作系统  
> A local-first, file-structure-driven workspace where AI agents can understand rules, route work, update state, and collaborate with you over time.

Agentic-Work-OS is not a note-taking template. It is a lightweight operating protocol for working with AI agents on your own computer.

Instead of keeping every project trapped inside a chat thread, Agentic-Work-OS gives agents a shared local workspace: rules, state, project logs, reusable resources, inputs, outputs, and demos. When a thread breaks, a model quota runs out, or you want another agent to take over, the next agent can read the workspace and continue.

## Quick Start

1. Copy this repository to a local folder.
2. Open it with an AI coding or file-aware agent.
3. Ask the agent:

```text
Read AGENTS.md and System/Core first. Then run one of the examples and explain how this workspace works.
```

4. Try one of the demos:
   - `examples/weekly-report-demo/`
   - `examples/agentic-work-os-research-demo/`

For a more guided first run, open each demo's `demo-walkthrough.md`. It gives you a copy-paste prompt, the expected agent behavior, the output shape, and the project log that should remain for the next agent.

## What Problem It Solves

Most AI workflows break in four predictable ways:

| Problem | What usually happens | What Agentic-Work-OS changes |
|---|---|---|
| Profile-level memory | The model remembers broad preferences, but not project-level decisions. | Project state and work logs make context precise and readable. |
| Probabilistic output | Formatting, tone, and structure drift between runs. | Rules and templates reduce drift and make outputs reviewable. |
| Isolated chats | Each thread becomes its own island. | Agents share the same workspace and project files. |
| Single-agent fragility | A broken thread, quota limit, or model switch can interrupt work. | A new agent can read the workspace and continue with limited context loss. |

## Core Ideas

- **Local-first**: your working context lives in files you can inspect, copy, version, and audit.
- **Agent-readable rules**: `AGENTS.md` and `System/Core/` tell agents how to behave before they act.
- **State over memory**: important project facts are written into files, not only remembered in chat.
- **Input and output routing**: raw materials enter through `input/`; finished or working outputs go to `output/`.
- **Project continuity**: active work lives in `System/Active_Projects/`.
- **Reusable knowledge**: stable references live in `System/Resources/`.
- **System growth**: logs, templates, and roadmap notes help the workspace improve over time.

## Repository Map

```text
Agentic-Work-OS/
  AGENTS.md
  System/
    Core/
    Active_Projects/
    Skills/
    Resources/
    System_Log/
  input/
  output/
  examples/
  docs/
```

## Demos

### Weekly Report Demo

A fictional user drops scattered weekly notes into the workspace. The agent turns them into a structured weekly report, records what happened, and shows how project continuity works.

Start with `examples/weekly-report-demo/demo-walkthrough.md`.

### Agentic Work OS Research Demo

A fictional user drops short research notes about AI collaboration systems. The agent creates a simple reference card explaining Agentic-Work-OS itself. This demo is self-explanatory: while running it, users learn what the system is.

Start with `examples/agentic-work-os-research-demo/demo-walkthrough.md`.

## What This Is Not

- Not a private second brain export.
- Not a real business workspace.
- Not a complete teaching sandbox.
- Not a vendor-specific agent framework.
- Not a RAG server or vector database.

## Safety Principle

Do not put private data, company documents, credentials, personal profiles, customer records, or confidential project files into a public repository.

See `docs/safety-and-sanitization.md`.

## Roadmap

See `docs/roadmap.md`.

## License

MIT
