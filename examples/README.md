# Examples

This directory contains operational example packs that show how **AI Task Graph** would be applied to real tasks.

These are not only explanatory wiki pages. Each example pack is meant to show:
- the incoming task
- the governing standards and constraints
- the generated task graph
- why the graph takes that shape
- what each major node produces
- how calibration, scale-out, merge, and convergence behave

## Example packs

- [`technical-book-canonical/`](technical-book-canonical/README.md) — canonical end-to-end example for a technical book project
- [`coding-feature-canonical/`](coding-feature-canonical/README.md) — canonical end-to-end example for a feature implementation branch in an existing codebase
- [`research-analysis-canonical/`](research-analysis-canonical/README.md) — canonical end-to-end example for a current-reality analytical question

## How to read an example pack

1. Read the task statement.
2. Inspect the generated graph.
3. Review the key execution and review nodes.
4. Inspect how scaling, merge, and convergence behave for that domain.
5. Compare the pack to other domain packs to see how graph shape changes.

## Why the examples matter

The framework is strongest when it is not only described but shown as a working execution discipline.

The repo started with one gold-standard example first. It now extends that pattern into multiple domains so visitors can see that the framework adapts to:
- writing-heavy work
- coding work
- research / analytical work

without collapsing into one rigid template.
