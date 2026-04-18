# Final Convergence

This page explains how the coding-feature branch closes.

## Final convergence is not just “merge and stop”

Even if the feature appears implemented, the graph still asks:
- are the branches consistent?
- did local patches hide a deeper issue?
- is the feature branch still structurally valid?

## Main closing nodes

### `MERGE_REVIEW`
Checks whether outputs can be combined safely.

### `QA_GATE`
Checks correctness and whether the feature actually satisfies the task.

### `PATCH_REGRESSION_QA`
Checks whether fixes introduced new breakage or technical debt.

### `GRAPH_REFRESH` if needed
If the feature branch turns out to be structurally wrong, the graph should refresh instead of pretending the original path is still good.

## Typical graph-refresh triggers in coding

- the chosen slice was too narrow or too broad
- interface assumptions were wrong
- the feature actually needs a deeper architectural seam first
- repeated patching is creating more complexity than it removes

## What successful convergence looks like

A successful coding convergence phase produces:
- a working feature branch
- interfaces that remain coherent
- manageable regression risk
- no obvious hidden structural problem left untreated

## What this example proves

This example shows that **AI Task Graph** is not only about long writing projects.

It is also a disciplined way to keep implementation work from drifting into:
- uncontrolled code churn
- unsafe branching
- merge pain discovered too late
- patching that should really have become a graph refresh
