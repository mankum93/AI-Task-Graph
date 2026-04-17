# Quickstart

This is the shortest practical path to using **AI Task Graph** on a real task.

## What you need

You need three things:

1. a real task
2. the packet or the relevant packet surfaces
3. a prompt that tells the AI to generate a task graph instead of continuing loosely

## Step 1 — Pick a real task

Good starter tasks:
- write a chapter or small book plan
- implement a coding feature in an existing codebase
- analyze a current-reality question
- solve a structured proof or reasoning problem

Avoid starting with a huge uncontrolled task if you are just learning the framework.

## Step 2 — Attach the right packet surfaces

### Minimal attachment set
Attach:
- `packet/v08/core_packet.md`
- `packet/v08/domain_profiles.md`

### Better attachment set
Also inspect:
- `examples/technical-book-canonical/README.md`
- the relevant wiki page for your domain

## Step 3 — Paste the starter prompt

Use the prompt from [`first-task-graph-prompt.md`](first-task-graph-prompt.md).

The point of the prompt is to force the AI to:
- classify the task
- identify the fundamental unit of work
- decide whether pilot calibration is needed
- propose explicit nodes, dependencies, and review points

## Step 4 — Check the generated graph

A decent first graph should tell you:
- what the task type is
- what the real unit of work is
- whether a pilot sample is required
- what can be parallelized later
- what QA or merge nodes are required
- what would trigger graph refresh

If the graph skips those things, it is probably too shallow.

## Step 5 — Execute the first node, not the whole task

Do **not** immediately ask the AI to do everything.

Instead:
- run the first framing or setup node
- then run the pilot-sample node if the graph calls for it
- then evaluate the scale-readiness decision

This is where the framework differs from ordinary continuation.

## Step 6 — Scale only when the graph earns it

If the graph says the branch is not ready to scale, do not force fan-out.

Improve the pilot.
Re-run readiness review.
Only then expand.

## What success looks like

After one pass, you should have:
- a graph
- a clearly identified unit of work
- either a pilot sample path or a direct execution path
- explicit review nodes
- a clearer execution strategy than “continue”

## Suggested next reading

After your first attempt:
- inspect [`choosing-a-unit-of-work.md`](choosing-a-unit-of-work.md)
- inspect the [canonical example](../examples/technical-book-canonical/README.md)
- inspect the [wiki](../wiki/README.md) if you want to understand domain-specific graph differences more deeply
