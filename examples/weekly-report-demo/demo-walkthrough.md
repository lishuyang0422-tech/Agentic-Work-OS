# Demo Walkthrough: Weekly Report

## What You Will Experience

This demo shows the smallest useful loop of Agentic-Work-OS:

1. read rules
2. inspect input
3. produce an output
4. leave a project log for handoff

It is intentionally fictional.

## Copy-Paste Prompt

```text
Read AGENTS.md, System/Core/AI_RULES.md, System/Core/CURRENT_STATE.md, and this demo folder.

Use examples/weekly-report-demo/sample-input.md as the raw input.

Create a weekly report in the style of examples/weekly-report-demo/expected-output.md.

Then explain:
1. where the final report should be saved,
2. what project log entry should remain for the next agent,
3. how this demo reduces thread-loss risk.
```

## Expected Agent Behavior

The agent should not ask for hidden context. It should use the files already present.

It should:

- identify `sample-input.md` as raw input
- synthesize a weekly report
- suggest saving the report under `output/`
- create or propose a log entry similar to `project-log-after-demo.md`
- explain that another agent can continue by reading the saved report and log

## What Makes This An OS Demo

The value is not only the weekly report. The value is that the work leaves a trace.

A later agent should be able to answer:

- What was the input?
- What was produced?
- What did we learn?
- What should happen next?

That is the difference between a chat response and a work system.
