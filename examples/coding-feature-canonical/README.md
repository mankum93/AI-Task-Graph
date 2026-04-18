# Coding Feature Canonical Example

This example pack shows how **AI Task Graph** applies to a software delivery task inside an existing codebase.

## Scenario

A user wants an AI agent to implement a meaningful feature in a real application:
- existing codebase
- existing architecture
- shared interfaces and regression risk
- tests expected
- quality matters more than brute-force code churn

## Why this example matters

The framework should not treat coding work the same way it treats long-form writing.

This example highlights the coding-specific strengths of the graph:
- selecting a meaningful feature slice instead of changing everything at once
- deciding whether a pilot slice is necessary when API / UX / architecture judgment is involved
- exposing merge-sensitive surfaces before parallel work expands
- inserting regression-aware review before final convergence

## Pack contents

- [`task.md`](task.md) — the incoming feature request and constraints
- [`generated-graph.md`](generated-graph.md) — the graph that should be generated for this task
- [`execution-and-merge.md`](execution-and-merge.md) — how workers, merge review, and regression checks behave
- [`final-convergence.md`](final-convergence.md) — how the graph closes the branch and when it refreshes instead of endlessly patching

## What this example proves

A naïve coding workflow often says:
- inspect codebase briefly
- implement feature everywhere
- patch regressions later

The graph instead says:
1. identify the real feature slice
2. decide whether a pilot slice is needed
3. expose dependency and interface surfaces
4. execute only ready branches
5. run merge review and regression review before convergence

This shows that the framework is not only for writing-heavy work. It also helps structured engineering tasks stay disciplined.
