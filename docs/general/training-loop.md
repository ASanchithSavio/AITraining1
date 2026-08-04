# Evidence-driven training loop

This repository is a memory system for prompt research. It does not run model tests automatically.

## Before research

1. Read the current benchmark rules and changelog.
2. Read the complete general read order in the repository README, not only the file remembered from the previous session.
3. Read the complete active-domain pack, including its review gates and training log.
4. Read the ignored local candidate, test, pivot, and audit notes for that domain when they exist.
5. Review retired candidates so failed architectures are not repeated.
6. Confirm current banned frameworks and source ecosystems privately.

Do not substitute chat history for this reload. Public notes contain generalized, share-safe lessons; ignored private notes contain the exact prompts, answers, sources, and manual outcomes needed to avoid repeating a tested failure. If the private notes are absent in a fresh checkout, record that context gap before proposing a candidate.

## Candidate record

Keep exact candidates in ignored local notes with:

```text
candidate_id:
status: research | preflight_failed | ready_for_user_test | retired
seeded_domain:
prompt_version:
prompt_frozen: yes | no
gold_answer:
gold_frozen: yes | no
terminal_source_and_location:
source_graph:
independent_hostnames:
submitted_source_formats:
known_distractors:
validity_risks:
difficulty_hypothesis:
```

## Preflight decision

Retire the candidate without testing if any of these is true:

- the gold answer is not directly proven;
- fewer than the required independent hosts are necessary;
- a clue is ambiguous, false, off-domain, or volatile;
- a pronoun, possessive, relative clause, or modifier has more than one grammatical attachment;
- the question narrates the browsing path;
- the answer depends on arithmetic or unbounded counting; or
- the architecture copies a known exemplar.

Batch size never lowers these gates. When several prompts are requested, give every candidate its own answer-first verification, visual terminal check, source-consumption audit, shortcut audit, grammatical-attachment audit, and exact-wording freeze. Replace a weak candidate instead of retaining it to fill the requested count.

## User-run test record

For every fresh run, record:

```text
model_and_mode:
memory_state:
fresh_chat:
prompt_pasted_exactly:
intermediate_statuses:
elapsed_time_to_terminal_result:
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

Record discarded branches as well as promoted candidates. A search snippet that exposes the terminal pair, an obvious one-row transcription, or a result page that prints the answer is useful training evidence even though the candidate is never tested.

Do not classify a run from elapsed time or an intermediate status. Wait for the terminal model or platform result unless the live rules explicitly define a timeout as failure. A long search is retrieval-cost evidence, not proof that the model was stumped.

When a model eventually answers correctly, retire the architecture unless the run was contaminated, regardless of how long it took. Record the elapsed time as secondary evidence, then identify where the apparent multi-source chain collapsed into a deterministic final lookup. Do not repair such a candidate by adding prose or more upstream identity clues.

## Delivery and change control

Run `delivery-checklist.md` before returning any prompt, answer check, failure reason, golden trajectory, golden rules, or verification-source list.

- Freeze the exact prompt after a manual test. A wording edit creates a new prompt version even when the evidence graph is unchanged.
- Freeze a reverified gold answer independently from the prompt. A trajectory or source-format repair can leave both frozen components unchanged.
- Record exact entities, answers, URLs, and reviewer wording only in ignored local notes.
- Keep public updates causal and reusable: what failed, why it failed, what changed, and what the next preflight must check.
- When testing remains user-run, do not query the target model while researching, verifying, logging, or formatting the package.
- Before submission, classify every cited URL by actual content and remove all JSON and YAML sources from the submitted path.

## Domain-pivot gate

After each completed batch, compare the result with `domain-pivot.md`. Pause the domain when two consecutive batches are fully solved across at least two terminal-source families and three selection mechanisms. More obscure entities, longer clue chains, and noisier scans do not count as new mechanisms.

When another domain has locally observed failure evidence, prefer that evidence over an untested intuition that the current domain can be made harder. Preserve the retired domain notes so a future return begins only from a genuinely new architecture.
