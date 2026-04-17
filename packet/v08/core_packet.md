# Core Packet v08

This file is a GitHub-friendly merged summary of the v08 core packet.

## Included sources
- `00_Master_Packet_Guide_and_Reading_Order`
- `00_Quick_Reference_Usage_Sheet`
- `General_Task_Graph_Generation_and_Heavy_Turn_Orchestration_Standard`
- `How_to_Use_the_General_Orchestration_Spec_with_a_Domain_Handoff`
- `Parallel_Execution_Orchestrator_and_Worker_Protocol`
- `Adversarial_QA_Gates_Graph_Refresh_and_Final_Convergence_Standard`
- `Task_Graph_Prompt_Templates_and_Node_Schemas`

## Core doctrine
The packet governs how an AI agent should turn a problem into a structured execution graph rather than proceeding through loose continuation. It emphasizes heavy work units, explicit standards stacks, evidence reporting, review-node placement, merge discipline, and graph refresh when the problem turns out to be structural rather than local.

A strong v08 addition is **calibration-first scaling**:
- identify the true fundamental unit of work
- decide whether the branch is scale-safe
- if subjectivity is high, generate a pilot sample first
- run a scale-readiness review before fan-out
- expand only after the sample proves that the output shape is stable

## Fundamental unit logic
The packet requires the graph to identify the smallest meaningful unit that can succeed at high quality before deciding whether batching is safe. For books this is often a chapter. For coding it may be a feature or subsystem slice. For research or mathematics it may be a proof segment, claim, or decision memo.

Dependency order alone is not enough. The graph must also choose a healthy **unit of work**.

## Node families
### Execution and graph control
- `EXECUTION`
- `PILOT_SAMPLE`
- `SCALE_OUT_READINESS_REVIEW`
- `GRAPH_REFRESH`

### Research, merge, and review
- `QA_GATE`
- `DEEP_RESEARCH_AUDIT`
- `MERGE_REVIEW`
- `HARMONIZATION`

### Writing-aware quality doctrine
- `DETEMPLATIZATION_QA`
- `ADDENDUM_INTEGRATION_QA`
- `ASSIMILATION_BALANCE_QA`
- `META_CAPABILITY_DRIFT_ANALYSIS`
- `WHOLE_SYSTEM_COHERENCE_QA`
- `SOURCE_ALIGNMENT_QA`
- `COVERAGE_BALANCE_QA`
- `EXAMPLE_DIVERSITY_QA`
- `VISUAL_TEXT_ALIGNMENT_QA`
- `READER_EXPERIENCE_QA`
- `DENSITY_AND_BLOAT_QA`
- `PATCH_REGRESSION_QA`
- `REWRITE_VS_PATCH_DECISION`

## What every graph should do
- classify the task branch early
- identify the governing standards stack
- identify the fundamental unit
- decide whether pilot calibration is mandatory
- avoid unsafe scale before the output shape is proven
- require evidence and consulted standards from every worker
- place merge review and harmonization before combining overlapping outputs
- refresh the graph when defects are structural instead of endlessly patching

## Why this matters
The packet is explicitly designed for tasks where AI quality often collapses under scale: long writing runs, bulk chapter generation, merge-heavy parallel work, judgment-heavy design tasks, or any workflow where the agent starts well and then drifts.

In those cases, the graph should not ask only “what is next?” It should also ask:
- what is the right unit?
- is this branch calibrated?
- is fan-out safe?
- are we still following the source hierarchy?
- are we solving the right problem, or should we refresh the graph?
