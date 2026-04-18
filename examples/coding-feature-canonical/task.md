# Task

## Incoming request

> Use the AI Task Graph framework to help an AI agent implement a feature in an existing product codebase. The feature spans a few layers, has regression risk, and should be implemented cleanly rather than as a pile of patches.

## What already exists

- a real codebase
- existing interfaces and architecture
- testing expectations
- implicit or explicit product constraints

## What tends to go wrong without a graph

In this class of task, a weak AI workflow often fails by:
- changing too much at once
- underestimating interface surfaces
- creating hidden merge conflicts across branches
- patching regressions after the fact instead of structuring execution well
- treating architectural judgment as if it were a purely mechanical edit

## What the graph must solve

The graph must decide:
- what the real implementation unit is
- whether the task needs a pilot slice before wider execution
- what can safely be worked on in parallel
- which review nodes must appear before merge and finalization
- whether the feature is still a patchable branch or actually needs graph refresh

## Resolved task classification

- **Primary type:** coding / software implementation
- **Secondary type:** possibly design-heavy if API or UX judgment is strong
- **Subjectivity:** medium
- **External-fact dependence:** low
- **Scale risk:** medium
- **Merge sensitivity:** medium to high

## Resolved fundamental unit

The framework selects a **feature slice** as the default unit.

That slice should be large enough to expose real implementation behavior, but small enough to:
- judge safely
- integrate safely
- revise before the whole feature branch expands
