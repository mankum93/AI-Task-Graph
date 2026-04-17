# Technical Book Canonical Example

This is the first gold-standard example pack for **AI Task Graph**.

It shows how the framework handles a task that is both large and quality-sensitive:
- a 20-chapter technical book
- a strong governance packet already exists
- chapter specs and standards exist
- diagrams matter
- the main risk is not missing content, but **quality collapse under scale**

## Why this example comes first

This example highlights the framework’s most differentiated strengths:
- choosing the real unit of work
- forcing pilot calibration before fan-out
- using writing-aware QA nodes
- shrinking back when later quality degrades
- merging chapter work into a coherent whole

## Pack contents

- [`task.md`](task.md) — the incoming task and constraints
- [`generated-graph.md`](generated-graph.md) — the graph that should be generated and why
- [`pilot-sample.md`](pilot-sample.md) — what the pilot chapter node does and how it is judged
- [`scale-readiness-review.md`](scale-readiness-review.md) — how the graph decides whether to scale
- [`worker-prompts.md`](worker-prompts.md) — worker and review prompts used after readiness is proven
- [`final-convergence.md`](final-convergence.md) — merge, coherence review, and shrink-back behavior

## What this example proves

A naïve AI workflow might try to write all 20 chapters directly.

This framework instead forces a more disciplined path:
1. identify chapter as the real unit of work
2. produce one representative chapter sample
3. review it through writing-aware QA
4. decide if scaling is actually safe
5. only then create controlled worker branches
6. shrink back if later chapter quality degrades

That is the operational value this example is meant to make obvious.
