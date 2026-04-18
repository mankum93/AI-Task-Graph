# Math / Proof Canonical Example

This example pack shows how **AI Task Graph** applies to mathematics and proof work.

<p align="center">
  <img src="../../assets/proof-graph-flow.svg" alt="Rendered proof-graph flow showing theorem locking, dependency graph construction, lemma execution, proof-gap QA, harmonization, and graph refresh" width="100%" />
</p>

## Scenario

A user asks the framework to help an AI agent prove a theorem, solve a proof-heavy problem, or produce a rigorous argument with explicit dependencies.

In this class of task, the main risk is not writing collapse or stale external facts. It is:
- hidden proof gaps
- circular dependence between claims
- undefined or drifting notation
- proving a nearby claim instead of the actual target
- local correctness that does not assemble into a valid whole proof

## Why this example matters

This example highlights a graph style that is different from both writing and research analysis:
- early definition and notation locking
- decomposition into claims, lemmas, and proof segments
- dependency-ordered execution instead of loose continuation
- proof-gap QA at the local and global level
- graph refresh when a failed lemma changes the viable route

## Pack contents

- [`task.md`](task.md) — the incoming proof task and why ordinary continuation is risky
- [`generated-graph.md`](generated-graph.md) — the graph that should be generated for this domain
- [`dependency-and-proof-gap-qa.md`](dependency-and-proof-gap-qa.md) — how proof execution and validity checks behave
- [`final-convergence.md`](final-convergence.md) — how the branch closes and when graph refresh is triggered

## What this example proves

A weak system often tries to prove the theorem in one pass and only notices mistakes at the end.

This framework instead forces:
1. exact target and notation locking
2. decomposition into judgeable proof units
3. dependency-aware execution of claims and lemmas
4. explicit proof-gap QA before treating progress as real
5. global assembly only after the local proof chain is defensible

That is the core value of the graph in this domain.
