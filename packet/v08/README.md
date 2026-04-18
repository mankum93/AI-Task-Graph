# Packet v08

This directory contains the unpacked **v08 task graph orchestration packet** in Markdown form for repository browsing and reuse.

## What this repo packet is

This is the **GitHub-friendly projection** of the v08 packet, not a byte-for-byte mirror of the original bundle.

The original packet was reorganized here into four Markdown entry surfaces so the framework can be browsed, linked, and reused more easily on GitHub:
- `README.md`
- `core_packet.md`
- `domain_profiles.md`
- `provenance.md`

## Files
- `README.md` — this guide
- `core_packet.md` — merged core packet text
- `domain_profiles.md` — merged domain profile text
- `provenance.md` — packet provenance, rendering model, and version-clarity notes

## Use this packet in the right order

### If you already have a project handoff
1. Treat your project handoff or canonical build spec as the highest-precedence source.
2. Treat local chapter, module, subsystem, or batch contracts as the next layer when they exist.
3. Use `domain_profiles.md` for reusable domain lenses.
4. Use `core_packet.md` for graph mechanics, review structure, worker discipline, and refresh logic.

### If you are here to understand the doctrine
1. Read [`provenance.md`](provenance.md) to understand what this repo packet represents.
2. Read [`core_packet.md`](core_packet.md) for the merged orchestration doctrine.
3. Read [`domain_profiles.md`](domain_profiles.md) for domain-specific adaptation.

### If you are updating the repo from a newer packet bundle later
1. Read [`provenance.md`](provenance.md).
2. Check which doctrinal changes belong in `core_packet.md`.
3. Check which domain changes belong in `domain_profiles.md`.
4. Then inspect downstream impact in `start-here/`, `prompts/`, `examples/`, and `wiki/`.

## Reading order inside this repo projection
1. `README.md`
2. `provenance.md`
3. `core_packet.md`
4. `domain_profiles.md`

## What the original bundle contained

The original v08 packet bundle was broader than this repo projection. It included source documents for:
- master packet guide and reading order
- quick reference usage sheet
- general orchestration standard
- domain-handoff combination guidance
- parallel execution protocol
- adversarial QA, graph refresh, and final convergence doctrine
- prompt templates and node schemas
- domain profile documents

Those surfaces are intentionally merged here into a smaller GitHub-native structure rather than being mirrored file-for-file.

## Highlights of v08
- calibration-first scaling
- pilot sample and scale-readiness review
- fundamental-unit selection
- worker/orchestrator protocol
- writing-aware review doctrine for templatization, integration quality, capability drift, and whole-system coherence
- domain profiles for books, coding, mathematics, and analytical work

## Important note

This repo’s `packet/v08/` directory is a **GitHub-friendly projection** of the v08 packet, not a raw archival mirror of every original source document.

Read [`provenance.md`](provenance.md) for:
- what this packet rendering represents
- how it relates to the original bundle
- how future packet versions should propagate into the repo
