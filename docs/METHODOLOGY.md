# How Frontier Bench works

[← Overview](../README.md) · [Live methodology](https://frontier-bench-omar.vercel.app/methodology)

## A task succeeds when the work succeeds

Each model configuration gets three attempts on each of 17 tasks in a frozen release. Every required check and milestone must pass. Partial check counts are diagnostic and do not earn fractional task success.

The score is **100 × the mean of the per-task success rates**. With three valid attempts on all 17 tasks, that is the number of successful attempts divided by 51, multiplied by 100.

## Fresh environments and executable grading

Each attempt starts in a fresh, isolated environment. The agent works through the allowed task terminal. Task inputs, resource limits, budgets, and grading behavior are fixed by the evaluation protocol.

The supplied reference solution must pass and the unchanged starter must fail before a task qualifies for evaluation. Hidden executable checks assess the work produced by the agent. A timeout is unsuccessful; an infrastructure failure is recorded separately.

## Preserve failures and interruptions

A valid unsuccessful attempt stays in the result. It is never retried to raise the score.

An infrastructure interruption prevents the original run from being complete. Where a separate completion campaign is published, its declaration fixes the selection of preserved outcomes and replacement attempts before those replacement outcomes exist. The original infrastructure records remain preserved. These campaigns explicitly disclose their recovery history and are not presented as an unchanged original run.

## Read a score in context

The website records model ID, reasoning effort, client, release, timing, and recovery information with each run. Different clients or verifier versions are meaningful differences. Seventeen tasks are a limited sample; these measurements do not establish performance across all engineering work.

The exploratory 95% intervals resample whole tasks, keeping repeated attempts together. Token and timing coverage can be incomplete. Unattributed cost does not mean zero cost. Requested model identity is not independent backend attestation.

## What stays private

The public presentation contains sanitized measurements and generic task identifiers. Actual task names, prompts, implementations, graders, reference solutions, candidate submissions, account credentials, and raw transcripts are not distributed here.

Current results are development measurements. Official eligibility and independent validation are separate from completing an evaluation.
