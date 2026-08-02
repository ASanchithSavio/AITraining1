# AITraining1

Reusable, public-safe notes for designing difficult, verifiable multi-source research prompts.

## Confidentiality boundary

This repository intentionally excludes client/platform instructions, copied submissions, chat transcripts, screenshots, share links, and exact unsubmitted prompt candidates. Those materials belong only in the ignored `private/` directory of an authorized local checkout. Public notes record generalized methods and lessons only.

## Read order

Start with the reusable method:

1. [`docs/general/core-method.md`](docs/general/core-method.md)
2. [`docs/general/domain-strategies.md`](docs/general/domain-strategies.md)
3. [`docs/general/review-diagnostics.md`](docs/general/review-diagnostics.md)
4. [`docs/general/training-loop.md`](docs/general/training-loop.md)

Then load the active domain pack. For Travel:

1. [`docs/travel/review-gates.md`](docs/travel/review-gates.md)
2. [`docs/travel/failure-patterns.md`](docs/travel/failure-patterns.md)
3. [`docs/travel/design-rubric.md`](docs/travel/design-rubric.md)
4. [`docs/travel/candidate-architecture.md`](docs/travel/candidate-architecture.md)
5. [`docs/travel/training-log.md`](docs/travel/training-log.md)

## Working loop

1. Re-read the current rules and prior failure log.
2. Choose a stable, obscure, directly printed final fact before writing the question.
3. Verify the fact visually and textually in its authoritative source.
4. Build backward through source handoffs that each eliminate a real alternative.
5. Confirm that the required sources are independent, including separate web hosts when the benchmark requires them.
6. Run the deterministic review gates before spending a model test.
7. Test only with the required target model.
8. Record the exact outcome locally, including why the model or the prompt failed.
9. Promote only generalized, non-confidential lessons into this repository.
