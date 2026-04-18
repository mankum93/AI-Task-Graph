# Provenance and Version Clarity

This page explains what the `packet/v08/` directory in this repository represents.

## What `packet/v08/` is

`packet/v08/` is the **repo-friendly public rendering** of the v08 AI Task Graph packet.

It exists so that the framework can be:
- browsed on GitHub
- linked from the README
- read without downloading an archive first
- used as a practical attachment surface for future AI workflows

## What `packet/v08/` is not

It is **not** intended to be a byte-for-byte archival mirror of every original source document in its original file format.

Instead, it is a GitHub-oriented presentation layer that emphasizes:
- readability
- navigability
- reuse
- public explanation

## How the packet was rendered into the repo

The original packet was consolidated into a smaller set of repository-friendly Markdown files:
- `README.md`
- `core_packet.md`
- `domain_profiles.md`
- `provenance.md`

This means the repo packet is a **structured projection** of the packet, not a raw dump.

## What each file in `packet/v08/` means

### `README.md`
The packet entrypoint and reading-order guide.

### `core_packet.md`
A merged GitHub-friendly packet view covering the core orchestration doctrine, heavy-turn orchestration, review logic, worker/orchestrator protocol, and node/prompt schema surfaces.

### `domain_profiles.md`
A merged GitHub-friendly view of the domain profiles used to adapt the framework across writing, books, coding, mathematics, and analytical work.

### `provenance.md`
This page, which explains how the repo packet relates to the original bundle and how future packet upgrades should be reflected here.

## Why this projection approach was chosen

The repository is meant to act as a framework showcase and adoption surface.

A literal archive mirror is useful for storage, but not ideal for:
- repo browsing
- onboarding
- linking from examples and prompts
- public explanation

So the repo keeps a cleaner GitHub-native version of the packet while preserving the framework’s actual doctrine.

## Version meaning

`v08` refers to the packet version currently reflected in this repository.

The main doctrinal features represented here include:
- calibration-first scaling
- pilot sample and scale-readiness review
- fundamental-unit selection
- worker/orchestrator protocol
- graph refresh logic
- writing-aware QA doctrine for templatization, integration quality, capability drift, and whole-system coherence
- domain profiles for books, coding, mathematics, and analytical work

## Relationship between packet, examples, prompts, and wiki

These repository sections play different roles:

- `packet/` → authoritative doctrine/reference layer
- `examples/` → operational example packs showing how the doctrine is applied
- `prompts/` → reusable execution assets derived from the doctrine
- `start-here/` → onboarding path for first use
- `wiki/` → explanatory deep dives and domain walkthroughs

The packet is the reference base that the other surfaces build on.

## How future packet upgrades should propagate into the repo

When a future packet version appears, the update process should be:

1. inspect the new packet bundle
2. identify doctrinal changes, new node types, new standing rules, or new domain-profile logic
3. update the repo-friendly packet projection under a new version directory such as `packet/v09/`
4. update examples, prompts, and onboarding surfaces only where the doctrinal change actually affects them
5. avoid casual drift where the repo examples or prompts begin saying things the packet no longer governs

## Change-discipline rule

If the packet changes:
- `packet/` must be updated first
- then `examples/`, `prompts/`, and `start-here/` should be checked for downstream impact
- `wiki/` should be updated only if its explanations are now outdated

This keeps doctrine and public-facing usage assets synchronized.

## Practical takeaway

If you are using this repo operationally:
- use `packet/v08/` as the doctrine/reference layer
- use `start-here/` as the first-use path
- use `prompts/` as reusable execution tools
- use `examples/` and `wiki/` to understand how the framework behaves on real classes of work
