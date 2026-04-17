# Scale Readiness Review

This page explains how the framework decides whether the technical-book graph is safe to expand after the pilot chapter.

## Purpose

`SCALE_OUT_READINESS_REVIEW` is the gate between:
- one good chapter
- and many chapters being generated

Its purpose is to stop the graph from making the classic mistake:

> The first chapter looks good, so let’s generate everything.

The framework treats that as unsafe reasoning.

## Inputs to the review

The readiness review consumes:
- the pilot chapter itself
- results from `DETEMPLATIZATION_QA`
- results from `VISUAL_TEXT_ALIGNMENT_QA`
- results from `READER_EXPERIENCE_QA`
- results from `META_CAPABILITY_DRIFT_ANALYSIS`
- any explicit user feedback on the pilot sample

## Questions the review must answer

### 1. Did the pilot prove the shape of good work?
Not just “is this chapter acceptable?”

Instead:
- is the structure strong enough to repeat?
- is the pedagogy actually good enough to scale?
- does the voice feel deliberate rather than generic?

### 2. Is the output stable, or was this just one lucky sample?
A single good chapter is not always enough.

The review must judge whether:
- the chapter type is representative enough
- the quality seems stable enough to fan out
- another calibration chapter is needed first

### 3. Are the worker surfaces now understood well enough?
If scaling is approved, workers will need:
- a clear output contract
- the approved sample as reference
- shared standards and chapter doctrine
- merge-sensitive warnings

If these are still fuzzy, readiness is not proven.

## Decision outputs

### Outcome A — Not ready
Use this when:
- the pilot still feels too generic
- writing-aware QA found meaningful problems
- the chapter shape is not stable enough to replicate
- the user feedback says the sample is not yet the right model

Action:
- revise the pilot
- keep the graph in single-unit calibration mode

### Outcome B — Partially ready
Use this when:
- the pilot is promising
- but the book may have very different chapter families
- or the style is subjective enough that one sample is not sufficient

Action:
- create one or two more calibrated chapter samples
- then rerun readiness review

### Outcome C — Ready to scale
Use this when:
- the pilot demonstrates the desired quality bar
- the graph now understands the chapter output shape
- the supporting QA confirms the sample is strong enough
- worker prompts can now be derived safely

Action:
- create controlled parallel chapter workers
- keep merge review and whole-book coherence review in place

## Decision matrix

| Signal | Not ready | Partially ready | Ready |
|---|---|---|---|
| Pilot chapter quality | weak / generic | strong but incomplete proof | strong and representative |
| Templatization risk | visible already | low but not fully tested | low and controlled |
| User confidence in sample | low | medium | high |
| Chapter-family diversity | unresolved | likely varied | sufficiently modeled |
| Worker prompt clarity | unclear | improving | clear |

## Important principle

This review is intentionally conservative.

It is better to spend extra effort proving the right chapter shape than to generate fifteen weak chapters under false confidence.

That is exactly the kind of loss the framework exists to prevent.
