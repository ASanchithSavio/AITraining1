# Review and failure diagnostics

Use this taxonomy to identify whether a rejection came from prompt validity, evidence quality, or insufficient model difficulty.

## Prompt defects

- **Ambiguous:** more than one entity or interpretation fits.
- **Ambiguous grammatical attachment:** a pronoun, possessive, relative clause, or trailing modifier can grammatically point to more than one nearby entity, even when subject knowledge suggests the intended reading.
- **Factual error:** a premise, date, relationship, or scope statement is false.
- **Not timeless:** the answer changes with the reader's clock or a live source.
- **Off-domain:** one or more clues or the answer leave the seeded domain.
- **Unnatural process instructions:** the prompt tells the solver what to search, which page to open, or which table to read.
- **Underconstrained:** the answer is obvious, general knowledge, or available from one or two lookups.
- **Unnecessary constraint:** a clue adds words but eliminates no candidate.
- **Reference leak:** a source name, distinctive phrase, or unsurfaced answer is embedded in the question.
- **Terminal-coordinate leak:** the prompt identifies the terminal document and supplies the exact page, row, serial, or column, reducing the final task to transcription.
- **Post-identification collapse:** the upstream chain looks long, but after the central entity or document is identified only one obvious selection remains.
- **Type-filter leak:** the requested answer type uniquely reveals which phrase to copy from a small terminal cell without requiring another evidence decision.

## Grammatical attachment preflight

Run this check on the final prompt text, not on an earlier draft:

1. Mark every `it`, `its`, `they`, `their`, `this`, `that`, `which`, `former`, `latter`, and possessive phrase.
2. For each marked word, list every grammatically possible antecedent in the same sentence and the preceding sentence.
3. If more than one antecedent is possible, repeat the exact noun: `the study`, `the mineral separate`, `the filing`, or `the field`.
4. Check every phrase after a comma, semicolon, or dash. A nearby noun can capture a modifier that was intended for the sentence's earlier subject.
5. Check tense and ownership separately. A study can examine a province, but neither a value nor a specimen owns a study merely because the intended research chain makes that relationship guessable.
6. Recount the words and confirm that the explicit-noun repair did not reveal an answer, terminal identifier, or source path.

Deliberate noun repetition is preferable to elegant pronouns when several entities of the same number appear close together.

## Answer defects

- incorrect gold value;
- sentence, explanation, range, alternative pair, or binary answer;
- arithmetic-derived value instead of a printed fact;
- answer not provable from a live authoritative source; or
- answer outside the seeded domain.

## Trajectory defects

- a prompt constraint has no evidence step;
- a search uses information not present in the prompt or a prior step;
- a source location is missing or imprecise;
- the cited intermediate fact is absent from the source;
- a step does not narrow the field;
- the described path does not reach the cited page;
- the final step does not defend uniqueness; or
- the trajectory contains filler and does not match the URL list one-to-one.

## Source defects

- broken, gated, region-blocked, or paywalled URL;
- homepage/search result rather than the direct destination;
- cited fact removed or on a different page;
- answer visible only inside an image, chart, or illegible scan;
- repeated pages from too few independent web hosts; or
- extra URL that is not needed to solve the question.

## Model-evaluation defects

- correct final answer incorrectly labelled as a failure;
- formatting, unit equivalence, or harmless abbreviation counted as failure;
- failure caused by ambiguity or arithmetic;
- incomplete accounting across runs; or
- reused context, memory, hints, or altered prompt text contaminating the test.

## Interpreting an automated difficulty rejection

A prompt can be technically valid yet fail a multi-run automated threshold because the model answers it correctly too often. Treat that as a probability signal:

1. Do not add random verbosity.
2. Locate the hop the model solved reliably.
3. Replace that hop with a less-indexed but equally verifiable handoff.
4. Add only a constraint that removes a real competing answer.
5. Prefer a bounded selection or enumeration error over a retrieval dead end.
6. Re-run deterministic validation before another expensive test.

Measure difficulty after the main record has been identified. A candidate is weak when the remaining work is a one-page correction, one exact coordinate, or one type-filtered transcription. Upstream sources count toward difficulty only when they change the terminal selection or eliminate a live competing answer; sources that merely confirm the record's identity add provenance, not resistance.

The objective is a repeatable, legitimate wrong answer—not a refusal and not a lucky one-off miss.
