# Fictional Research Notes: AI Collaboration Systems

## Note A: Chat Threads Are Fragile

AI chat threads are useful, but they are fragile containers for long-running work. A thread can become too long, lose focus, hit a model limit, or simply become hard to audit.

## Note B: Files Make State Portable

When rules, decisions, project status, and outputs are written into local files, another agent can inspect the workspace and continue. This makes work less dependent on one chat session.

## Note C: Agent Handoff Needs Protocol

Multiple agents can collaborate if they share a simple protocol:

- where to read rules
- where to find current state
- where raw inputs go
- where outputs should be saved
- where decisions are recorded

## Note D: The System Must Grow Carefully

A useful AI work system should improve over time, but not by randomly rewriting its core rules. Observations should first be logged, reviewed, and then promoted into stable rules only when appropriate.
