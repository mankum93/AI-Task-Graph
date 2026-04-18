# Execution and Merge

This page explains what happens once the coding-feature graph begins executing.

## Step 1: architecture and interface inspection

Before major implementation begins, the graph inspects:
- affected modules
- interface surfaces
- data flow boundaries
- likely regression zones

This prevents the system from treating a cross-cutting feature as a simple local edit.

## Step 2: pick the real feature slice

The graph chooses a slice that is:
- meaningful enough to expose real behavior
- small enough to judge safely
- small enough to revise before unsafe spread

Good examples:
- one backend contract slice
- one flow end-to-end for UI + data
- one migration-safe subsystem slice

## Step 3: decide whether a pilot slice is needed

A pilot slice is useful when the task contains judgment surfaces such as:
- public API ergonomics
- user-facing interaction quality
- architecture taste

If the branch is mostly mechanical and interfaces are already stable, the graph may skip pilot calibration.

## Step 4: execute only ready branches

If the graph approves split work, workers should only receive branches that are truly ready.

Each worker must report:
- standards or codebase rules consulted
- evidence checked
- new interface or merge-sensitive surfaces created
- carry-forward risks for the orchestrator

## Step 5: merge review before finalization

Parallel coding work often fails at the merge boundary.

That is why the graph inserts `MERGE_REVIEW` before final convergence.

`MERGE_REVIEW` looks for:
- conflicting assumptions
- duplicated logic
- inconsistent conventions
- interface collisions
- hidden integration problems

## Step 6: regression-aware review

After merge, the graph runs:
- `QA_GATE`
- `PATCH_REGRESSION_QA`

These check:
- correctness
- whether fixes caused side effects
- whether patching is still rational
- whether a deeper structural issue has appeared

## Why this matters

A weak coding workflow often postpones structure until after regressions appear.

This graph does the opposite:
- it chooses a safer unit early
- exposes merge surfaces early
- and checks whether the branch is still structurally healthy before calling it done
