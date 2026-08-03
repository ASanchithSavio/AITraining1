# Politics training log

## 2026-08-03 - first answer-first Politics rebuild

### Prior evidence used

- The strongest local Politics examples produced meaningful wrong answers through a fragile identity or sequence handoff in completed official records.
- Their useful mechanisms were exact historical scope, spelling or tenure bridges, and plausible alternatives inside the correct record.
- The new design must preserve those causal properties without copying a debate-quotation or delimitation-adjacency architecture.

### Research decisions

1. Chose completed campaign-finance filings as a new native Politics source family.
2. Used an official result-certification date as a version boundary rather than a decorative clue.
3. Verified the full sequence of organization statements on both sides of that boundary.
4. Compared the relevant historical form pages visually and textually.
5. Selected a bank name that is added in the post-boundary amendment while a strong biographical association points toward the retained pre-boundary bank.

### Rejections

- Rejected a contested-election committee-report path because search extraction exposed nearly every distinctive count that could serve as an answer.
- Rejected current committee metadata because the overview page and snippets expose it directly.

### Current status

One 84-word candidate passed ground-truth, chronology, atomicity, source-ecosystem, originality, visual-verification, and shortcut checks. Its exact prompt, answer, source links, file numbers, images, and audit remain in ignored local notes. It has not been tested by the agent and has not been submitted anywhere.

The difficulty hypothesis is a historical version-selection error: the solver must locate the last organization statement before a state result certification and the first amendment after it, then identify one newly added field value. If the model accurately compares both forms, the candidate must be retired.

### Manual-test signal

The user later reported that a fresh target-model session spent about 25 minutes researching without reaching a final answer. This is a promising retrieval-resistance signal, but it is not yet recorded as a confirmed model failure: a run is classifiable only after the session returns a final answer or explicitly terminates without one. No agent-run model test or platform submission occurred.

## 2026-08-03 - additional answer-first mining

Several Politics branches were rejected before drafting a test candidate:

- A historical convention-ballot sequence failed the shortcut audit because an exact query surfaced the delegation and likely sequence.
- A modern roll-call delta collapsed after one participant's own official statement exposed the relevant vote change.
- A historical veto comparison produced a valid set of vote switchers, but the proposed biographical discriminator independently named the intended person. The roll-call comparison therefore became decorative.
- A preferential-election transfer path was not promoted because the accessible result pages did not preserve the complete intermediate distribution needed for a fair, reproducible terminal selection.

The reusable lesson is that a difficult comparison cannot be rescued by a clue that independently identifies its answer. For a future Politics candidate, the person or record should emerge only from the intersection of independently sourced sets, and at least two meaningful decisions should remain after the central event is known.
