# Scale Readiness Review

Use this after a pilot sample and its immediate review nodes have run.

```text
Run the SCALE_OUT_READINESS_REVIEW node only.

Inputs:
- the pilot sample output
- the results of the relevant QA nodes
- any user feedback on the sample

Requirements:
1. Decide whether the branch is:
   - not ready to scale
   - partially ready and needs more calibration
   - ready to scale
2. Explain why.
3. Do not treat one decent sample as automatic proof that batch or parallel execution is safe.
4. State what worker surfaces are now understood well enough, and what still remains risky.
5. End with the recommended next node.
```

## Use this to force the important question
The point is not “was the sample okay?”

The point is:
> did the sample prove a stable output shape that is safe to repeat?
