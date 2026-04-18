# Task

## Incoming request

> Use the AI Task Graph framework to answer a current-reality analytical question where the answer depends on external facts and a correct framing of the real decision.

## What tends to go wrong without a graph

In this class of task, a weak AI workflow often fails by:
- assuming the question means something it does not
- answering from stale memory
- researching the wrong subproblem
- producing a polished answer to a nearby question

## What the graph must solve

The graph must decide:
- what exact decision the user wants answered
- how to cluster the investigation into meaningful route families or question groups
- when external grounding is mandatory
- when research has changed the framing so much that the graph should refresh

## Resolved task classification

- **Primary type:** research / analytical problem solving
- **External-fact dependence:** high
- **Subjectivity:** medium
- **Scale risk:** medium
- **Merge sensitivity:** medium if multiple investigative branches are synthesized

## Resolved fundamental unit

The framework selects a **question cluster** or **route family** as the default unit.

This means the graph should not start by synthesizing one giant answer. It should first break the problem into meaningful investigative routes that can be grounded and compared.
