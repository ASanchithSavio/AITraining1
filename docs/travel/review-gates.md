# Travel prompt review gates

Run these gates in order. A candidate that fails an early gate should not consume a model test.

## 1. Ground-truth gate

- The final answer is visibly printed in an authoritative source.
- The row, column, page section, and spelling have been checked rather than trusted from OCR or a snippet.
- There is exactly one defensible answer under the stated scope.
- The answer is stable enough to remain verifiable; avoid live prices, current availability, ratings, and open-ended budgets.

## 2. Atomic-answer gate

- The answer is one name, number, date, time, place, or short phrase.
- It is looked up or selected, not derived through arithmetic.
- It is not a yes/no choice, an alternative pair, a range, or a sentence.
- Small OCR or rounding differences cannot decide whether the model passed.

## 3. Source-architecture gate

- Several distinct sources are genuinely needed.
- Count independent web hostnames, not just URL count; three pages on one host are not three independent source ecosystems.
- Each source contributes a new branch-reducing fact; repeated confirmation of the same entity does not count as a full hop.
- No single obvious query reveals the final answer together with all identifying context.
- The last source does not become obvious merely because its title, table name, or distinctive phrase was quoted in the question.
- The private verification path and the submitted source list match one-to-one.
- Verification URLs stay outside the prompt body unless a task rule explicitly requires them there.

## 4. Prompt-language gate

- The prompt reads as one natural factual question.
- It does not narrate a wall-to-wall research procedure or assign every lookup to a named source.
- Pronouns and relational words such as “former,” “latter,” “next,” and “same” have exactly one referent.
- Scope traps are explicit and fair: the relevant list, group, direction, or sequence is named precisely.

## 5. Domain gate

- Every clue, handoff, and the final answer remains about travel: destinations, routes, visitor facilities, accommodation, access, heritage travel, protected-area visitation, or comparable travel material.
- Biographical, political, financial, or historical facts are not used merely as unrelated puzzle glue.

## 6. Difficulty gate

Prefer difficulty caused by retrieval and selection:

- a buried row in a long table;
- a change of spelling that is explicitly bridged;
- adjacency within a precisely scoped group;
- a non-indexed but readable archival guide;
- a source handoff where a common name has to be disambiguated.
- a bounded enumeration over an explicitly listed set that a reviewer can reproduce quickly.

Do not treat verbosity, famous facts, multiple redundant clues, unbounded counting, calculation, or volatile information as difficulty.

Before promotion, run a shortcut audit:

- Search snippets do not expose the terminal answer or adjacent row.
- A single obvious query does not collapse the full chain.
- The terminal operation is not merely sorting, direction-following, or category filtering over a short list.
- The tempting wrong answer survives earlier constraints and is eliminated only by contextual reading.
- The final record is poorly indexed but still directly readable and reviewer-verifiable.
- A competing publication or edition cannot make the answer ambiguous; the prompt's date and title select exactly one record.

## 7. Failure-legitimacy gate

A usable model failure has a wrong final answer even though the prompt and gold answer are sound. Reject the candidate if the model is correct, if the difference is only formatting/rounding, or if ambiguity caused the error.
