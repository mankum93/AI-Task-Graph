# Final Convergence

This page explains how the mathematics / proof branch closes.

## Final convergence is not just “the proof looks finished”

Even if the theorem appears proved, the graph still asks:
- do the local claims really assemble into the theorem?
- did any hidden assumption enter late?
- did a patch fix one lemma while breaking the route logic elsewhere?
- is the final proof actually proving the target statement and not a nearby variant?

## Main closing nodes

### `HARMONIZATION`
Assembles the proven claims and lemmas into one coherent proof route.

This is not cosmetic. It checks whether the dependency chain actually fits together.

### `QA_GATE`
Checks global validity and proof exposition.

At this stage the question is no longer only “is each local claim plausible?” but also:
- does the global argument close the theorem?
- are all cases covered?
- did any dependency remain unproved or merely asserted?

### `GRAPH_REFRESH` if needed
If the current proof route turns out to be structurally wrong, the graph should refresh instead of pretending the original route can be saved by endless patching.

## Typical graph-refresh triggers in proof work

- a supposedly central lemma is false
- the route depends on a stronger claim than the standards stack allows
- the theorem needs a different decomposition into cases or lemmas
- repeated local repairs still leave a global gap

## What successful convergence looks like

A successful proof convergence phase produces:
- a theorem or target claim that is actually established
- an explicit dependency chain that holds together
- no obvious unresolved proof gap left untreated
- a proof that is not only locally plausible but globally valid

## What this example proves

This example shows that **AI Task Graph** is useful not only for writing, coding, or research-heavy work.

It is also a disciplined way to keep proof work from drifting into:
- intuition presented as proof
- circular routes hidden by fluent prose
- local patches that never restore global validity
- theorem proofs that should really have triggered a graph refresh earlier
