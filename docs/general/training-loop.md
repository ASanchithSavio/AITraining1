# Evidence-driven training loop

This repository is a memory system for prompt research. It does not run model tests automatically.

## Before research

1. Read the current benchmark rules and changelog.
2. Read `core-method.md`, `domain-strategies.md`, and the active domain pack.
3. Review retired candidates so failed architectures are not repeated.
4. Confirm current banned frameworks and source ecosystems privately.

## Candidate record

Keep exact candidates in ignored local notes with:

```text
candidate_id:
status: research | preflight_failed | ready_for_user_test | retired
seeded_domain:
prompt_version:
gold_answer:
terminal_source_and_location:
source_graph:
independent_hostnames:
known_distractors:
validity_risks:
difficulty_hypothesis:
```

## Preflight decision

Retire the candidate without testing if any of these is true:

- the gold answer is not directly proven;
- fewer than the required independent hosts are necessary;
- a clue is ambiguous, false, off-domain, or volatile;
- the question narrates the browsing path;
- the answer depends on arithmetic or unbounded counting; or
- the architecture copies a known exemplar.

## User-run test record

For every fresh run, record:

```text
model_and_mode:
memory_state:
fresh_chat:
prompt_pasted_exactly:
final_answer:
failure_label:
first_divergence:
sources_used_or_missed:
share_or_evidence_location_private_only:
```

Do not call a run a failure until the cited reasoning and gold source have been checked.

## Update rule

Promote only a causal lesson:

- **Observed:** what the model or reviewer did.
- **Cause:** the earliest verifiable divergence or rule failure.
- **Change:** the smallest architecture or wording repair.
- **Result:** what happened on the next authorized test.

Keep exact prompts, transcripts, private links, client language, and screenshots out of the public repository.
