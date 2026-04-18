# Prompts

This directory contains reusable prompt assets for operating the **AI Task Graph** framework.

These prompts are not the whole framework by themselves. They are meant to be used **with** the packet and, where relevant, the domain profiles and example packs.

## Best entrypoint

If you are new to the framework, start with:
- [`../start-here/README.md`](../start-here/README.md)
- [`../start-here/quickstart.md`](../start-here/quickstart.md)

Then use the prompts in this directory as the graph advances.

## Included prompts

- [`generate-task-graph.md`](generate-task-graph.md) — ask the AI to generate a graph for a real task
- [`pilot-sample.md`](pilot-sample.md) — run only the pilot sample node
- [`scale-readiness-review.md`](scale-readiness-review.md) — decide whether the branch is safe to scale
- [`worker-execution.md`](worker-execution.md) — execute one worker node under the graph discipline
- [`merge-review.md`](merge-review.md) — review parallel outputs before harmonization
- [`graph-refresh.md`](graph-refresh.md) — restructure the graph when the problem is no longer local

## How to use these

Typical flow:
1. attach the packet surfaces
2. use `generate-task-graph.md`
3. run the first node
4. if the graph requires calibration, use `pilot-sample.md`
5. use `scale-readiness-review.md` before fan-out
6. use worker, merge, and graph-refresh prompts only when the graph reaches those stages

## Where to see these in context

If you want to see how these prompts fit into real graph execution, inspect:
- [`../examples/README.md`](../examples/README.md)
- [`../examples/technical-book-canonical/README.md`](../examples/technical-book-canonical/README.md)
- [`../examples/coding-feature-canonical/README.md`](../examples/coding-feature-canonical/README.md)
- [`../examples/research-analysis-canonical/README.md`](../examples/research-analysis-canonical/README.md)

## Important note

These prompts are deliberately structured to reinforce the framework’s doctrine:
- find the real unit of work
- calibrate before unsafe scale-out
- force explicit review and reporting
- refresh the graph when patching the current path is the wrong move
