# First Task Graph Prompt

Copy, adapt, and paste this prompt into your AI system after attaching the packet surfaces.

## Starter prompt

```text
Use the attached AI Task Graph packet to generate a task graph for my task.

If I have also attached a project handoff, canonical build spec, or local contract, treat those as higher-precedence than the general orchestration packet.

My task:
[PASTE YOUR TASK HERE]

Requirements:
1. Classify the task type correctly.
2. Name the active standards stack in precedence order before generating the graph.
3. Identify the real fundamental unit of work, not just dependency order.
4. Decide whether a pilot sample is required before any scale-out.
5. If subjectivity is high, include a PILOT_SAMPLE node and a SCALE_OUT_READINESS_REVIEW node.
6. Identify what can safely run later in parallel and what must happen first.
7. Insert the right QA, merge, or graph-refresh nodes for this task type.
8. For each major node, explain:
   - purpose
   - why it exists
   - what it should produce
   - which governing standards it should consult
9. Do not jump straight to bulk execution. If the branch is not yet safe to scale, say so.
10. If the task is writing-heavy, include the relevant writing-aware review doctrine.
11. Require workers to report consulted standards and evidence, not just output.
12. End with the recommended first node to execute.
```

## What this prompt is trying to force

This prompt tries to stop a weak response such as:
- a loose checklist
- generic project-planning bullets
- immediate bulk execution
- missing calibration logic
- ignoring the real standards hierarchy

A stronger response should instead produce:
- a graph with node types
- unit-of-work logic
- scale-readiness logic
- branch-specific QA
- an explicit standards stack
- a clear first execution step

## Good follow-up prompt after the graph exists

```text
Run the first node of the graph only.
Show what this node resolves, what it unlocks, and what the next node should be.
Report which standards this node consulted.
Do not skip ahead to later execution.
```

## Good follow-up prompt when a pilot sample is required

```text
Run the PILOT_SAMPLE node only.
Then evaluate whether the branch is actually ready to scale or whether the graph should stay in calibration mode.
Report which standards and evidence were used for that readiness decision.
```
