# Concepts

## Agentic-Work-OS Is Not A Knowledge Base

A knowledge base stores information.

Agentic-Work-OS defines how AI agents work with information:

- where inputs enter
- how project state is recorded
- where outputs go
- how reusable references are kept
- how agents hand work off to each other
- how the system improves over time

## From Chat Box To Work OS

Most AI work starts in a chat box. That is useful, but long-running work needs more than conversation.

Agentic-Work-OS adds a local working layer around the chat:

- rules
- state
- project logs
- resources
- inputs
- outputs
- change history

This makes the workspace readable by both humans and agents.

## Agent Handoff

Agent handoff is one of the main reasons this system exists.

If one thread breaks, grows too long, hits quota limits, or needs to be replaced by another model, the next agent should not start from zero. It can read:

- `AGENTS.md`
- `System/Core/AI_RULES.md`
- `System/Core/CURRENT_STATE.md`
- project logs
- previous outputs

Then it can continue with limited context loss.

## Multi-Agent Collaboration

Different agents can work on the same project if the project state is written into files.

Example roles:

- Agent A drafts.
- Agent B reviews.
- Agent C argues the opposite side.
- Agent D synthesizes the final decision.

The human remains the decision-maker. The file structure keeps the shared working context stable.

## System Growth

A living work system should improve, but not by randomly rewriting core rules.

Recommended pattern:

1. record observations
2. review them
3. promote stable lessons into rules or templates
4. log meaningful changes

This protects the system from drift while allowing it to learn.
