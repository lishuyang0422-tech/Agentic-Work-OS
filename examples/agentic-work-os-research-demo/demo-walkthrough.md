# Demo Walkthrough: Agentic Work OS Research

## What You Will Experience

This demo is self-explaining.

While running it, the agent uses fictional research notes to explain the system you are using. The point is to show that Agentic-Work-OS can route research input, synthesize a reference card, and leave a handoff trail.

## Copy-Paste Prompt

```text
Read AGENTS.md, System/Core/AI_RULES.md, System/Core/CURRENT_STATE.md, and this demo folder.

Use examples/agentic-work-os-research-demo/sample-research-notes.md as the raw input.

Create a concise reference card in the style of examples/agentic-work-os-research-demo/expected-reference-card.md.

Then explain:
1. what Agentic-Work-OS is,
2. why file-based state helps agent handoff,
3. what project log entry should remain for the next agent.
```

## Expected Agent Behavior

The agent should:

- identify the research notes as fictional input
- extract the main claims
- create a clear reference card
- describe the input -> synthesis -> output -> handoff loop
- suggest saving the reference card under `System/Resources/` or `output/`
- propose a handoff log similar to `project-log-after-demo.md`

## What Makes This A Self-Explaining Demo

The demo teaches the concept by performing the concept:

- it receives input
- it follows rules
- it produces a reusable artifact
- it explains handoff
- it leaves a trace

That is the core behavior of Agentic-Work-OS.
