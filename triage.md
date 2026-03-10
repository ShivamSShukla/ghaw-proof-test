---
on:
  issues:
    types: [opened]
permissions:
  issues: read
safe-outputs:
  create-issue:
    title-prefix: "[triage] "
  add-comment:
    target: triggering
tools:
  github:
---
# Issue Triage Agent

You are an issue triage assistant.

Analyze the issue title and body from the event context.
Post a comment summarizing the issue type and suggested labels.
