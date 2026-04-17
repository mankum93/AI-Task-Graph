# Graph Refresh

Use this when the problem appears to be structural rather than local.

```text
Run the GRAPH_REFRESH node only.

Context:
[PASTE CURRENT GRAPH OR RELEVANT BRANCH]

Reason refresh is being considered:
[PASTE ISSUE]

Requirements:
1. Explain why the current graph or branch is no longer healthy.
2. Distinguish between local patchable issues and structural issues.
3. Propose a revised graph or revised branch sequence.
4. State which previous nodes remain valid and which are invalidated.
5. Keep useful work where possible, but do not preserve a bad structure only because work has already been done.
6. End with the recommended next node under the refreshed graph.
```

## Typical triggers
- the wrong unit of work was chosen
- scaling began too early
- merge-sensitive surfaces were underestimated
- research changed the real framing of the task
- repeated patching is no longer rational
