# AITraining1

Reusable, public-safe notes for designing difficult, verifiable multi-source research prompts.

## Confidentiality boundary

This repository intentionally excludes client/platform instructions, copied submissions, chat transcripts, screenshots, share links, and exact unsubmitted prompt candidates. Those materials belong only in the ignored `private/` directory of an authorized local checkout. Public notes record generalized methods and lessons only.

## Read order

Start with the reusable method:

1. [`docs/general/core-method.md`](docs/general/core-method.md)
2. [`docs/general/golden-trajectory-format.md`](docs/general/golden-trajectory-format.md)
3. [`docs/general/delivery-checklist.md`](docs/general/delivery-checklist.md)
4. [`docs/general/domain-strategies.md`](docs/general/domain-strategies.md)
5. [`docs/general/review-diagnostics.md`](docs/general/review-diagnostics.md)
6. [`docs/general/training-loop.md`](docs/general/training-loop.md)
7. [`docs/general/domain-pivot.md`](docs/general/domain-pivot.md)

Then load the active domain pack. For Travel:

1. [`docs/travel/review-gates.md`](docs/travel/review-gates.md)
2. [`docs/travel/failure-patterns.md`](docs/travel/failure-patterns.md)
3. [`docs/travel/design-rubric.md`](docs/travel/design-rubric.md)
4. [`docs/travel/candidate-architecture.md`](docs/travel/candidate-architecture.md)
5. [`docs/travel/training-log.md`](docs/travel/training-log.md)

For Politics:

1. [`docs/politics/review-gates.md`](docs/politics/review-gates.md)
2. [`docs/politics/training-log.md`](docs/politics/training-log.md)

For Legal:

1. [`docs/legal/review-gates.md`](docs/legal/review-gates.md)
2. [`docs/legal/training-log.md`](docs/legal/training-log.md)

For Science & Technology:

1. [`docs/science/review-gates.md`](docs/science/review-gates.md)
2. [`docs/science/training-log.md`](docs/science/training-log.md)

For Art:

1. [`docs/art/review-gates.md`](docs/art/review-gates.md)
2. [`docs/art/training-log.md`](docs/art/training-log.md)

For Business:

1. [`docs/business/review-gates.md`](docs/business/review-gates.md)
2. [`docs/business/training-log.md`](docs/business/training-log.md)

For Finance:

1. [`docs/finance/review-gates.md`](docs/finance/review-gates.md)
2. [`docs/finance/training-log.md`](docs/finance/training-log.md)

This read order is a required reload, not an optional reference. Use it before designing a candidate and again before delivering a prompt, answer confirmation, failure reason, golden trajectory, golden rules, or verification sources. Read the general method, the complete active-domain pack, and the ignored local records for that domain (when present). Public files preserve reusable lessons; ignored `private/` files preserve exact candidates, gold answers, manual test outcomes, reviewer feedback, source repairs, and shortcut audits. Do not rely on chat memory in place of this reload. In a checkout without the private records, note that limitation and use the public files as the minimum safe baseline.

## Working loop

1. Re-read the current rules, every relevant general note, the complete active-domain pack, and its local private failure log.
2. Choose a stable, obscure, directly printed final fact before writing the question.
3. Verify the fact visually and textually in its authoritative source.
4. Build backward through source handoffs that each eliminate a real alternative.
5. Confirm that the required sources are independent, including separate web hosts when the benchmark requires them.
6. Run the deterministic review gates before spending a model test.
7. Test only with the required target model.
8. Record the exact outcome locally, including why the model or the prompt failed.
9. Promote only generalized, non-confidential lessons into this repository.
10. Before sending any golden package, run the delivery checklist and freeze any prompt or answer the user asked to keep unchanged.
