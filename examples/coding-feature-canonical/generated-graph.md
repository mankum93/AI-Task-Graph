# Generated Graph

This is the graph the framework should generate for the coding-feature task.

```mermaid
flowchart TD
    A[Frame the feature request] --> B[Inspect architecture, interfaces, and affected surfaces]
    B --> C[Resolve feature slice as the fundamental unit]
    C --> D{High subjectivity in API / UX / architecture?}
    D -->|Yes| E[PILOT_SAMPLE implementation slice]
    D -->|No| F[Direct EXECUTION graph]
    E --> G[SCALE_OUT_READINESS_REVIEW]
    G --> H{Safe to split further?}
    H -->|Yes| I[Parallel implementation branches]
    H -->|No| J[Single-branch implementation]
    F --> K[Dependency-aware execution]
    I --> L[MERGE_REVIEW]
    J --> L
    K --> L
    L --> M[QA_GATE]
    M --> N[PATCH_REGRESSION_QA]
    N --> O{Structural problem revealed?}
    O -->|Yes| P[GRAPH_REFRESH]
    O -->|No| Q[Final convergence]
```

## Why this graph shape is correct

The coding branch is governed by a different risk model than the writing branch.

The dominant problems are:
- interface misreads
- regression risk
- unsafe parallelism across shared surfaces
- local patching that hides a deeper structural issue

So the graph focuses on:
- feature-slice selection
- readiness for safe split
- merge review
- regression review
- graph refresh when architecture assumptions break

## Important judgment

This branch does **not** automatically require the full writing-aware review doctrine.

However, if the task includes strong judgment surfaces like:
- public API shape
- UX-heavy interaction flow
- architectural taste

then the graph may still use a `PILOT_SAMPLE` before scaling.

## Why dependency order is still not enough

A weak coding graph might say:
- backend first
- then frontend
- then tests

A stronger graph also asks:
- is the selected feature slice the right unit?
- is this branch safe to split yet?
- are merge-sensitive interfaces already understood?
- are we still dealing with a feature branch, or has the work become structural enough to refresh the graph?
