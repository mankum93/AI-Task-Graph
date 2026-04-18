# Examples

This directory contains operational example packs that show how **AI Task Graph** would be applied to real tasks.

These are not only explanatory wiki pages. Each example pack is meant to show:
- the incoming task
- the governing standards and constraints
- the generated task graph
- why the graph takes that shape
- what each major node produces
- how calibration, scale-out, merge, and convergence behave

<p align="center">
  <img src="../assets/domain-graph-comparison.svg" alt="Rendered comparison chart showing how graph shape changes across writing, coding, research, and proof domains" width="100%" />
</p>

## Which pack should you open first?

| If your task looks like... | Start with... | Why |
|---|---|---|
| a technical book, course-like material, chaptered educational writing, or other quality-sensitive long-form content | [`technical-book-canonical/`](technical-book-canonical/README.md) | it shows the framework’s strongest calibration-first and writing-aware behavior |
| a feature, subsystem, implementation branch, or merge-sensitive code delivery path | [`coding-feature-canonical/`](coding-feature-canonical/README.md) | it shows execution, QA, merge review, and graph refresh in a real codebase-shaped flow |
| a current-reality question or analytical synthesis task grounded in external evidence | [`research-analysis-canonical/`](research-analysis-canonical/README.md) | it shows evidence-heavy analysis, audit behavior, and convergence on a reality-modeling branch |
| a theorem, proof-heavy problem, or dependency-sensitive mathematical argument | [`math-proof-canonical/`](math-proof-canonical/README.md) | it shows definition locking, lemma dependency order, proof-gap QA, and proof-route refresh |

## Example packs

- [`technical-book-canonical/`](technical-book-canonical/README.md) — canonical end-to-end example for a technical book project
- [`coding-feature-canonical/`](coding-feature-canonical/README.md) — canonical end-to-end example for a feature implementation branch in an existing codebase
- [`research-analysis-canonical/`](research-analysis-canonical/README.md) — canonical end-to-end example for a current-reality analytical question
- [`math-proof-canonical/`](math-proof-canonical/README.md) — canonical end-to-end example for a mathematics / proof branch

## How to read an example pack

1. Read the task statement.
2. Inspect the generated graph.
3. Review the key execution and review nodes.
4. Inspect how scaling, merge, and convergence behave for that domain.
5. Compare the pack to other domain packs to see how graph shape changes.

## Suggested reading strategy

If this is your first visit:
1. pick the pack closest to your real task
2. read that pack front to back
3. then compare it to one other domain pack
4. only then inspect the packet or wiki more deeply if you want doctrine-level detail

That gives most readers a faster trust-building path than trying to absorb the entire repo at once.

## How these relate to the rest of the repo

- Use [`../start-here/`](../start-here/README.md) if you are trying the framework for the first time.
- Use [`../prompts/`](../prompts/README.md) for reusable execution prompts.
- Use [`../packet/v08/`](../packet/v08/README.md) for doctrine and source-of-truth guidance.
- Use [`../wiki/`](../wiki/README.md) for deeper explanation of why graph shapes differ by domain.

## Why the examples matter

The framework is strongest when it is not only described but shown as a working execution discipline.

The repo started with one gold-standard example first. It now extends that pattern into multiple domains so visitors can see that the framework adapts to:
- writing-heavy work
- coding work
- research / analytical work
- mathematics / proof work

without collapsing into one rigid template.
