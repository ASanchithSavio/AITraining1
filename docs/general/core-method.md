# Core method for difficult research prompts

This method separates three questions that are often confused:

1. **Validity:** Is the prompt factual, stable, unambiguous, and verifiable?
2. **Architecture:** Does solving it genuinely require several independent sources?
3. **Difficulty:** Does the target model repeatedly produce a meaningfully wrong final answer for a legitimate reason?

A prompt is not useful merely because it is long, obscure, or failed once. It has to clear all three layers.

## 1. Start from the answer

Mine a final fact before drafting the question. The best terminal facts are:

- printed directly in a stable source;
- short enough to grade atomically;
- poorly indexed but readable;
- surrounded by plausible distractors;
- tied to a completed event or dated publication; and
- provable without arithmetic, estimation, or subjective judgment.

Record the exact section, row, column, paragraph, or PDF page. Also record nearby entries so row-shift and scope mistakes can be detected.

## 2. Build a source graph backward

Treat the solution as a directed graph rather than a pile of clues:

```text
prompt clue -> intermediate fact -> narrower source -> intermediate fact -> terminal record -> answer
```

Every node must contribute a new, source-backed fact. Every edge must reduce the remaining candidate set. Remove a source if the next step does not consume its output.

Use genuinely independent sources. Multiple URLs from one site can still be a single source ecosystem; where a benchmark requires independent web domains, count hostnames rather than pages.

## 3. Use fair failure mechanisms

High-value mechanisms are error-prone but fully checkable:

- bounded enumeration of a clearly listed set;
- exact row or column selection in a long table;
- a named subgroup or scope that excludes a tempting popular answer;
- two similar names joined by an explicit identity bridge;
- old and new spellings reconciled by a source;
- a multi-hop chain in which each result becomes the next lookup key; and
- a final passage that must be read in context rather than copied from a snippet.

Avoid difficulty based on:

- vague superlatives or relationships;
- live prices, schedules, availability, rankings, or officeholders;
- calculations across source values;
- illegible scans or unreliable OCR;
- a huge unbounded counting task;
- obscure wording that merely causes refusal; or
- naming every source and narrating the research procedure.

## 4. Write one natural question

The final prompt should stand alone as a natural factual question. It should not read like a checklist, JSON/XML object, or browsing script. Keep referents explicit, attach each modifier to one noun, and replace vague words with measurable or named constraints.

The prompt should not reveal a terminal page through a distinctive title, quotation, source name, or answer-only search term. The research path belongs in private verification notes, not in the question.

### Constraint-substitution drafting

One useful drafting method begins with a single verified factual sentence containing the answer. Replace named entities one at a time with objective, source-backed descriptions until the combined constraints still identify exactly one entity. An individual clue may fit several candidates; uniqueness must come from the full intersection, not from vague adjectives such as `famous`, `important`, or `popular`.

- Preserve an exact quoted phrase when a common paraphrase would fit many records.
- Paraphrase rare evidence only when the new wording preserves the same scope and cannot attach to another entity.
- Keep table headings, legal categories, scientific fields, and other technical terms exactly as the controlling source labels them.
- Give a dated letter, report, or release its year when the clue otherwise depends on a moving present-time interpretation.
- Apply a five-year test: the answer should remain the same five years later because the question is anchored to a completed event, fixed edition, dated filing, or one-time occurrence.
- Cross-domain identity clues are useful only when they remain necessary and the final answer still belongs honestly to the seeded domain.
- Bounded counting, sorting, or ranking is acceptable when the set and rule are explicit and the trajectory can reproduce the operation quickly. Reject unbounded enumeration or difficulty based on tedious manual work.

This is a drafting aid, not permission to hide the answer behind unnatural prose. After substitution, rewrite the result as one ordinary question and rerun the uniqueness, grammar, source-necessity, and shortcut checks.

## 5. Verify before testing

Run deterministic checks first:

- one defensible answer;
- atomic output;
- every premise true;
- every hop remains in the seeded domain;
- all sources direct, stable, readable, and accessible;
- cited facts present as text or reliable selectable OCR;
- each source necessary;
- no arithmetic dependency;
- no moving time reference; and
- no copied exemplar structure.

Only after these checks should a model run consume time or tokens.

## 6. Diagnose a failure

A valid model failure is a wrong final answer produced despite a sound prompt and correct ground truth. Trace the first divergence:

- wrong entity identification;
- missed source handoff;
- scope error;
- row/column error;
- incomplete bounded enumeration;
- confusable-name substitution; or
- correct document, wrong contextual reading.

If the model is correct, the gold answer is wrong, or the prompt permits its answer, the run is not evidence of model failure. Repair or retire the prompt.
