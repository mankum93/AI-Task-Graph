# Choosing a Unit of Work

One of the most important ideas in **AI Task Graph** is that the graph must identify the right **unit of work**.

This is not the same as dependency order.

## Why this matters

Many bad AI workflows fail because the system scales the wrong unit.

Examples:
- writing 20 chapters instead of proving one chapter shape first
- changing an entire subsystem instead of proving one feature slice first
- trying to solve a whole proof at once instead of structuring lemmas
- analyzing a huge topic instead of breaking it into route comparisons

The right unit is the smallest meaningful slice that can:
- be judged well
- expose the real quality bar
- be repeated later if it proves stable

## Common units by domain

| Domain | Common good unit |
|---|---|
| Technical book | chapter |
| Novel / narrative | scene or chapter |
| Coding | feature slice or subsystem slice |
| Proof / math | lemma, claim, or proof segment |
| Analytical research | route family or question cluster |
| Product / UX | judged interaction slice |

## Questions to ask

When choosing a unit, ask:
- what is the smallest slice that still reveals the real quality bar?
- what slice can the user judge with confidence?
- what slice is safe to revise before scale-out?
- what slice would become dangerous if multiplied too early?

## Warning signs that the unit is wrong

The chosen unit is probably wrong if:
- it is so large that quality failure is expensive to detect
- it is so small that it hides the real problem
- it cannot be judged well on its own
- it encourages immediate bulk execution without proof of quality

## Why the graph cares

The framework is built on the idea that a good graph should not only ask:
- what comes first?

It should also ask:
- what size of work can still succeed well?

That is why unit selection happens early in the graph, before unsafe fan-out begins.
