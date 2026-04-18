# Dependency Lock and Proof-Gap QA

This page explains how execution behaves once the proof graph exists.

## The graph does not treat “looks plausible” as progress

In mathematics and proof work, apparent progress is cheap.

A proof fragment may sound persuasive while still containing:
- a hidden assumption
- an unlicensed theorem use
- a quantifier shift
- a circular dependency
- a claim that is weaker or stronger than the target actually needs

So the graph requires explicit proof-gap checking at the local-claim level.

## What the first execution layer does

Before proving anything substantial, the branch should lock:
- the exact target statement
- the active definitions
- notation and variable conventions
- the admissible toolset, prior results, or theorem library

This matters because many later “proof errors” are really earlier framing errors.

## What a claim / lemma worker should report

A worker proving one claim or lemma should report:
1. the exact claim being established
2. which earlier claims, definitions, or tools it depends on
3. whether the proof fully establishes the claim or only a subcase
4. any unresolved gaps or conditions
5. whether the claim should be split, weakened, or reformulated

This makes it possible for the orchestrator to tell the difference between:
- real proof progress
- promising intuition
- a route that now needs refresh

## What the `QA_GATE` checks locally

For each claim or lemma, the proof QA layer should ask:
- Is the claim stated precisely enough to judge?
- Were all dependencies already established or explicitly allowed?
- Does the proof actually establish the claim as stated?
- Is there any circularity?
- Did notation or assumptions drift mid-proof?
- Did the proof silently change the domain, quantifiers, or cases?
- Is there an unresolved gap disguised as “clearly” or “it follows”?

## Common triggers for local proof failure

- the claim was underspecified
- a needed lemma was missing from the dependency map
- the proof only covered a special case
- the route relied on a theorem that is not admissible in the current standards stack
- the claim is true but not the right claim for the theorem route

## When local patching is enough

Local patching is usually enough when:
- the missing step is small and does not change downstream structure
- the claim is correct but needs tighter wording
- a dependency citation was omitted but the dependency is already established

## When `GRAPH_REFRESH` is the right move

Refresh the graph when:
- a key lemma is false or cannot be proved with the allowed tools
- the dependency ordering itself was wrong
- the theorem should be decomposed differently
- the current route repeatedly produces patchy local fixes without restoring global validity

## What this example proves

A proof branch should not be managed like one long monologue.

It should be managed like a dependency-sensitive structure where each claim earns the right to support later claims.
