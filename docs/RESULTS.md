# Published results and recovery notes

[← Overview](../README.md) · [Live results](https://frontier-bench-omar.vercel.app)

This snapshot reflects the completed configurations in the private repository's published website data on **October 24, 2026**, for release `long-horizon-v0.7`. Every row below contains 51 valid selected outcomes across 17 tasks. Incomplete or running evaluations are not represented as completed results.

| Model | Effort | Client | Success | Pass | Unsuccessful | Retained source infrastructure interruptions |
| :--- | :--- | :--- | ---: | ---: | ---: | ---: |
| Grok 4.7 | Low | Cursor SDK | 60.784% | 31 | 20 | 2 |
| Grok 4.7 | Medium | Cursor SDK | 54.902% | 28 | 23 | 1 |
| GPT-6 Luna | Medium | Codex CLI | 19.608% | 10 | 41 | 0 |
| GPT-6 Luna | Low | Codex CLI | 11.765% | 6 | 45 | 2 |

Unsuccessful includes valid failures and budget-exhausted outcomes. Retained infrastructure interruptions are historical source outcomes, separate from each completed campaign's 51 selected valid outcomes.

## Grok 4.7 · low

[Inspect the campaign](https://frontier-bench-omar.vercel.app/runs/grok47-low-completion-3885241c)

The completed development campaign includes two separately declared replacement attempts. The original two infrastructure interruptions remain in the incomplete source run. The declaration followed the start of the original evaluation and preceded the replacement outcomes. No valid failure was rerun.

## Grok 4.7 · medium

[Inspect the campaign](https://frontier-bench-omar.vercel.app/runs/grok47-medium-completion-284d5b0f)

The completed development campaign includes one separately declared replacement attempt. The original infrastructure interruption remains in the incomplete source run. The declaration followed the start of the original evaluation and preceded the replacement outcome. No valid failure was rerun.

## GPT-6 Luna · medium

[Inspect the run](https://frontier-bench-omar.vercel.app/runs/623df4c46a694e18806d0c9797727987)

This completed development run includes a post-start grading amendment: grading continued from an unchanged saved submission after an upload fault, without new model calls. The run page preserves that disclosure.

## GPT-6 Luna · low

[Inspect the campaign](https://frontier-bench-omar.vercel.app/runs/luna-low-completion-0a70b41cdaf4)

The completed development campaign includes two separately declared replacement attempts. The original two infrastructure interruptions remain in the incomplete source run. The declaration followed the start of the original evaluation and preceded the replacement outcomes. No valid failure was rerun.

## Comparison limits

These are development results, not official rankings. Client implementations and verifier fingerprints differ; the full configuration and exploratory uncertainty intervals are available on each run page. Requested model IDs are not independently attested backend identities. The repository's README rounds displayed percentages to one decimal place.
