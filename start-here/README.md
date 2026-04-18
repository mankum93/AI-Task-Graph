# Start Here

This directory is the shortest path from **understanding AI Task Graph** to **using AI Task Graph**.

## Open these first

If you are new to the framework, use this order:

1. [`quickstart.md`](quickstart.md) — what to attach, what prompt to paste, and what to check first
2. [`first-task-graph-prompt.md`](first-task-graph-prompt.md) — the starter prompt for generating your first graph
3. [`choosing-a-unit-of-work.md`](choosing-a-unit-of-work.md) — the key concept that decides whether the graph stays healthy under scale

After that:
4. inspect the reusable [`../prompts/`](../prompts/README.md) library
5. then inspect the most relevant [canonical example pack](../examples/README.md#which-pack-should-you-open-first)

## Pick the route that matches how you learn

- **I want to use it right now** → start with [`quickstart.md`](quickstart.md)
- **I want to see a full worked example first** → jump to [`../examples/README.md`](../examples/README.md)
- **I want the source-of-truth doctrine first** → open [`../packet/v08/README.md`](../packet/v08/README.md) and [`../packet/v08/provenance.md`](../packet/v08/provenance.md)

## What this section is for

The rest of the repo explains the framework, packet, wiki, and examples in depth.

This section is different.

It answers:
- what do I attach?
- what prompt do I paste?
- what kind of output should I expect?
- what do I do after the graph is generated?

## Minimal adoption path

If you want the shortest path:
- read [`quickstart.md`](quickstart.md)
- copy the prompt from [`first-task-graph-prompt.md`](first-task-graph-prompt.md)
- attach the packet or the relevant packet surfaces
- ask the AI to generate a task graph for your real task
- then use the prompts in [`../prompts/`](../prompts/README.md) as the graph advances

## After your first graph exists

Do not immediately ask the AI to do the whole project.

Instead:
- run the recommended **first node only**
- if the graph calls for calibration, run the **pilot sample** next
- use the reusable prompts only when the graph actually reaches those stages
- inspect the examples or wiki if you want help judging whether the graph shape looks right

## When to inspect more

Once you have a generated graph, use:
- the [packet](../packet/v08/README.md) for doctrine
- the [examples](../examples/README.md) for operational patterns
- the [prompts](../prompts/README.md) for reusable execution assets
- the [wiki](../wiki/README.md) for deeper understanding of why graph shapes differ by domain
