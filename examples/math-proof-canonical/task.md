# Task

## Incoming request

> Use the task graph framework to help an AI agent produce a rigorous proof of a theorem. The work already has a target statement, accepted mathematical background, and some candidate intermediate ideas, but the route is not yet fully trusted.

## What already exists

- a target theorem or proof-heavy problem statement
- accepted definitions and notation, or at least a draft of them
- some possible intermediate claims or lemma ideas
- a requirement for rigor rather than persuasive prose alone

## What tends to go wrong without a graph

In this class of task, an unconstrained AI often fails in predictable ways:
- notation shifts mid-proof
- a hidden assumption appears without being declared
- later claims depend on earlier claims that were never really established
- the proof jumps from intuition to conclusion without a valid bridge
- the system proves a nearby fact and treats it as equivalent to the real target
- local proof fragments look plausible but do not assemble into a coherent dependency chain

## What the graph must solve

The graph must not only schedule work. It must decide:
- what the real proof target is
- which definitions and admissible tools must be locked first
- what the dependency order of claims and lemmas actually is
- what the right proof unit is for execution and checking
- when a failed lemma means local patching is enough versus when the route itself must refresh

## Resolved task classification

- **Primary type:** mathematics / proof
- **Secondary type:** structured reasoning and exposition
- **Subjectivity:** low to medium for correctness, higher for explanatory presentation
- **External-fact dependence:** low
- **Scale risk:** medium
- **Merge sensitivity:** medium to high when multiple proof fragments or routes exist

## Resolved fundamental unit

The framework selects **claim / lemma** as the fundamental unit.

This is because a claim or lemma is:
- small enough to check for actual validity
- large enough to carry meaningful proof progress
- the right unit for dependency ordering
- the right place to surface hidden assumptions or proof gaps before they infect the entire theorem

## Immediate implication

The graph should not begin by writing a full theorem proof in one pass.

It should first:
1. lock the target statement, definitions, notation, and allowed tools
2. decompose the route into claims or lemmas
3. execute and check them in dependency order
