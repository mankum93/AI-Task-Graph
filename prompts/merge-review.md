# Merge Review

Use this after parallel or independent branches have produced outputs that must be combined.

```text
Run the MERGE_REVIEW node only.

Inputs:
- the outputs of the relevant branches
- the shared standards stack
- any known merge-sensitive surfaces

Requirements:
1. Identify conflicting assumptions across branches.
2. Identify duplicated logic, duplicated content, or inconsistent conventions.
3. Identify hidden interface or terminology collisions.
4. State whether the issue is local or systemic.
5. Recommend whether the next step should be:
   - HARMONIZATION
   - local patching
   - branch-level regeneration
   - GRAPH_REFRESH
6. End with a merge-risk summary.
```

## Why this prompt exists
Parallel work is valuable only when the merge is governed. This prompt makes shared-surface risk explicit before convergence.
