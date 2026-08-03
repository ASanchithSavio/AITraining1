# Legal training log

## 2026-08-03 - first answer-first Legal candidate

### Research direction

1. Restricted the domain to completed official legal records and avoided advice, current-law questions, and live dockets.
2. Mined correction notices and errata before writing a prompt, looking for an original value, a corrected value, and a nearby plausible alternative.
3. Selected a source graph that moves from a Supreme Court referral to a parliamentary laying record and then to the issuing commission's report and separate errata.
4. Verified the original table and the correction visually, including the page, annexure, serial number, column, and direction of replacement.
5. Asked for an entity type that selects one title from a corrected cell containing two different kinds of legal bodies.

### Rejections

- Rejected ordinary appellate errata because exact case-name searches exposed the correction directly.
- Rejected a bail-report corrigendum whose most difficult candidate answer appeared to be another typographical error; that would make review harder without creating a better legal-research task.
- Rejected live statutory interpretation and current-law comparisons because later amendments could change the answer.

### Pre-test status

One 98-word candidate passed the ground-truth, historical-stability, source-handoff, row-and-column, answer-type, originality, and search-shortcut checks. Its exact prompt, answer, URLs, document locations, and distractor audit remain in ignored local notes. The final errata is a sharp one-page official image without a selectable text layer, so that accessibility limitation is explicitly retained as a review risk.

The difficulty hypothesis is a three-way scope error: a solver may retain the authority printed in the original report, take the corrected tribunal from the adjacent errata row, or return the non-officer body printed in the correct replacement cell. The prompt asks for the officer title, leaving one atomic answer. No model test or platform submission was performed by the agent.

### Manual target-model outcome

The user later reported that a fresh target-model session reached the correct gold answer in roughly 40 seconds. The candidate is retired for insufficient difficulty. This is a model success and a prompt-design failure, not a wrong-answer run.

### Causal diagnosis

- **Observed:** the model returned the correct atomic title quickly.
- **Cause:** once the report was identified, the prompt explicitly directed the solver to a separate one-page errata and supplied the annexure, serial, and column. The final task was therefore a bounded transcription, not a fragile scope decision.
- **Cause:** the requested entity type selected the only officer title in the replacement cell, neutralizing the nearby body as a distractor.
- **Cause:** the court and parliamentary sources authenticated the report but did not change which correction cell or version controlled the answer.
- **Change:** do not reuse this architecture. A future Legal candidate must retain at least two meaningful choices after record identification, avoid exact terminal coordinates in the prompt, and make upstream sources control terminal scope rather than merely identify the report.
- **Result:** no repaired version was authorized or tested; the exact outcome is preserved in ignored local notes.
