# Generate Task Graph

Use this when you want the AI to generate the graph for a real task.

```text
Use the attached AI Task Graph packet to generate a task graph for my task.

My task:
[PASTE TASK HERE]

Requirements:
1. Classify the task correctly.
2. Identify the real fundamental unit of work, not just dependency order.
3. Decide whether a pilot sample is required before any scale-out.
4. If subjectivity is high, include a PILOT_SAMPLE node and a SCALE_OUT_READINESS_REVIEW node.
5. Identify what can safely run later in parallel and what must happen first.
6. Insert the right QA, merge, and graph-refresh nodes for this task type.
7. For each major node, explain:
   - purpose
   - why it exists
   - what it should produce
8. Do not jump straight to bulk execution. If the branch is not yet safe to scale, say so.
9. If the task is writing-heavy, include the relevant writing-aware review doctrine.
10. End with the recommended first node to execute.
```

## Best used with
- `packet/v08/core_packet.md`
- `packet/v08/domain_profiles.md`
