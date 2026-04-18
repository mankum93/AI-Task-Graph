# Generate Task Graph

Use this when you want the AI to generate the graph for a real task.

```text
Use the attached AI Task Graph packet to generate a task graph for my task.

If I have also attached a project handoff, canonical build spec, or local contract, treat those as higher-precedence than the general orchestration packet.

My task:
[PASTE TASK HERE]

Requirements:
1. Classify the task correctly.
2. Name the active standards stack in precedence order before generating the graph.
3. Identify the real fundamental unit of work, not just dependency order.
4. Decide whether a pilot sample is required before any scale-out.
5. If subjectivity is high, include a PILOT_SAMPLE node and a SCALE_OUT_READINESS_REVIEW node.
6. Identify what can safely run later in parallel and what must happen first.
7. Insert the right QA, merge, and graph-refresh nodes for this task type.
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

## Best used with
- your project handoff or local contract, if one exists
- `packet/v08/core_packet.md`
- `packet/v08/domain_profiles.md`
- `packet/v08/provenance.md` when precedence or packet role needs to be made explicit
