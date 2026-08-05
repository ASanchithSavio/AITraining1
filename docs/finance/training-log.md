# Finance training log

## 2026-08-03 - acquisition, legal-entity, quarter, and Call Report coordinate

### Prior evidence used

- The strongest Science outcome combined wrong-record risk with a separate row-and-column decision.
- The retired Art candidate showed that a page break and neighbouring row alone may slow a model without producing a wrong final answer.
- The Finance search therefore targeted a transaction with sibling entities sharing a brand, a closing between quarter-ends, and a regulatory schedule containing adjacent amount and count columns.

### Research decisions

1. Rejected ordinary annual-report restatements because exact values appeared in search snippets or one filing contained the complete answer path.
2. Rejected failed-bank bid summaries whose terminal values were plainly indexed.
3. Selected a completed bank acquisition whose regulatory approval distinguishes a commercial bank, a savings association, and a fiduciary-service company with closely related names.
4. Used an independent closing filing to place the legal closing between two quarterly reporting dates.
5. Verified that the target institution, a similarly named savings association, and a later similarly named national bank have separate regulator identifiers and different historical rows.
6. Verified the decisive schedule visually: one item spans managed assets, non-managed assets, managed-account count, and non-managed-account count.
7. Verified the requested mnemonic in the Federal Reserve data dictionary and the directly reported value in the FDIC institution-level data.
8. Audited the sibling entity, the next quarter, and the three adjacent columns. Each produces a distinct, source-grounded wrong answer.
9. Removed the friendly field name after finding an indexed banking ranking page for that phrase. The final wording uses the official schedule coordinate, while the coordinate's meaning remains independently verifiable.
10. Ran exact searches combining the regulator identifier, report date, mnemonic, and proposed answer; no result joined the intended entity, period, and value.

### Current status

One 95-word Finance candidate passed the domain, atomicity, stability, independent-source, legal-entity, event-date, reporting-period, field-coordinate, unit, directly-printed-answer, shortcut, and grammatical-attachment gates. The exact prompt, answer, URLs, institution identifiers, adjacent-period values, and wrong-entity values remain in ignored local notes.

The difficulty hypothesis has three independent failure points after the acquisition is recognized: choose the commercial-bank subsidiary instead of two related institutions, choose the quarter immediately before the legal closing instead of the quarter after it, and choose the managed-asset amount rather than the neighbouring non-managed amount or account counts.

No target-model prompt was tested and no platform form was submitted by the agent. The candidate is ready for one fresh user-run GPT-5.5 extended-thinking test. It is not claimed to be empirically difficult until the final target answer is known.

### Reusable lessons

- Brand-name matching is unsafe in banking research; legal entity and regulator identifier must travel together.
- Approval date and closing date serve different purposes. Only the date named by the prompt should choose the reporting period.
- Historical names must be checked at the report date, not inferred from the institution's current name.
- A form coordinate can reduce search leakage without becoming arbitrary when an authoritative data dictionary defines the coordinate.
- Amount columns and account-count columns are separate semantic types even when they sit on the same schedule row.
- Search the friendly label before finalizing. Third-party ranking pages may expose fields that look obscure inside a regulator API.

## 2026-08-03 - first user-run target failure

### Outcome

The user reported that the required extended-thinking target model returned a wrong integer. A fresh comparison of the target institution, both adjacent quarter-ends, all four relevant schedule columns, and the similarly named institutions confirmed the stored gold answer. No target-model query or platform submission was made by the agent, and the platform-review status was not reported.

### First established divergence

The returned integer is absent from every relevant field on the correct institution's selected-quarter row. It is present in the requested field on more than one confusable legal-entity record. The supported diagnosis is therefore wrong legal entity, not merely wrong quarter or adjacent column. Without the target's reasoning trace, the evidence does not establish which confusable entity was used.

### Reusable lessons

- A shared financial-services brand must never replace a regulator identifier during the terminal lookup.
- Check whether a wrong answer exists on the correct entity before assigning a row or column failure label.
- Compare the wrong answer against sibling, predecessor, successor, and historical-name records; a matching value can reveal the first divergence.
- When several wrong records contain the same value, report only the common proven error class. Do not invent a precise model path from the final answer alone.
- This mechanism is worth preserving: entity hierarchy, event-bounded period selection, and a separate field-coordinate decision remained necessary after the transaction was identified.

## 2026-08-04 - source-format repair after platform review

### Review outcome

The platform reviewer considered the golden trajectory substantively good but returned it because the terminal value was cited from a JSON response and an intermediate field mapping was cited from YAML. The prompt, entity resolution, reporting-period logic, field coordinate, and gold answer were not challenged.

### Repair

1. Kept the prompt and gold answer unchanged.
2. Removed every JSON and YAML citation from the submission path, including a machine-readable institution lookup that the reviewer did not separately mention.
3. Replaced the identity lookup with an official human-readable regulator page.
4. Replaced the terminal API row with the official individual Call Report facsimile PDF available through the regulator's institution-report portal.
5. Visually verified the decisive page. The completed facsimile prints the institution, reporting date, schedule, item code, column heading, unit, and value together, so no schema mapping or field-name translation is needed.

The exact institution, identifiers, value, URLs, and PDF page remain in ignored local notes. No target-model prompt was run and no platform form was submitted by the agent.

### Reusable lessons

- Source-format compliance is a separate gate from factual correctness. A correct trajectory can still be rejected when its evidence is delivered in a prohibited serialized format.
- Do not wait for a reviewer to enumerate every instance of the same defect. If JSON or YAML is rejected, remove all such citations from the entire path.
- Prefer a completed human-readable regulatory facsimile over an API row when the facsimile prints the field mnemonic and value in the same cell.
- A schema file is redundant when the blank form and completed filing already establish the row, column, mnemonic, label, and unit.
- APIs can be useful for private discovery and cross-checking, but the submitted terminal source should be a permitted HTML page or PDF that a reviewer can inspect directly.

## 2026-08-04 - direct-terminal-URL repair after follow-up review

### Review outcome

The machine-readable evidence had been replaced successfully, but the follow-up review found that the terminal trajectory still ended at a regulator search portal. The instructions asked the reviewer to configure a report type, date, and identifier, generate the results, and then open the completed filing. The reviewer required the final citation to open the answer-bearing record directly.

### Repair

1. Kept the tested prompt and verified answer unchanged.
2. Removed the general facsimile-search portal from the submitted source list.
3. Removed every terminal instruction that asked the reviewer to build or execute a lookup.
4. Replaced the portal with the regulator's record-specific viewer URL, whose parameters fix the report family, historical institution, and reporting date.
5. Opened that URL in a fresh session and followed its embedded facsimile response.
6. Rendered the decisive page again and confirmed that the record identity, period, form, schedule, item, column, field mnemonic, unit, and final value are visible together.

No target-model query was run and no platform form was submitted by the agent.

### Reusable lessons

- A human-readable source can still fail review when its URL stops at a search form rather than the answer-bearing record.
- Distinguish URL query parameters that identify one fixed record from instructions that require a reviewer to construct and submit a search.
- The terminal trajectory should be reproducible with one click followed by page navigation, not a sequence of form selections.
- Test direct viewer URLs in a fresh session. A link that works only after a prior portal search is not a valid standalone final citation.
- Verify the embedded or returned document itself; an HTML viewer shell is acceptable only when the cited URL automatically loads the completed human-readable filing.
- When a reviewer identifies one remaining source-layer defect, freeze the prompt and answer and repair only the terminal access path.

## 2026-08-04 - successor-certificate and amount-versus-count candidate

### Research decisions

1. Re-read the full Finance candidate record, Finance review gates, cross-domain review diagnostics, and current status before selecting a new mechanism.
2. Rejected acquisition candidates whose difficulty ended after finding one plainly labelled Call Report cell.
3. Selected a completed holding-company acquisition whose approved bank combination distinguishes an acquired national bank from surviving state banks in two states.
4. Verified that a public merger table assigns different regulator certificates to the acquired bank and the surviving Louisiana bank. A current-name or successor-certificate lookup therefore opens the wrong historical reporter.
5. Used the completed transaction date to select the last quarter-end before consummation, rather than relying on the regulatory approval date.
6. Chose a temporary statutory deposit-insurance category whose completed filing presents a dollar amount and an account count as adjacent memorandum items.
7. Retrieved the official completed Call Report through the public facsimile interface. The target filing uses the domestic-and-foreign-offices form, while the surviving Louisiana bank uses the domestic-only form.
8. Rendered and visually inspected the target filing's cover and decisive page, plus the independent merger-table page. The terminal count, adjacent amount, institution name, report date, form type, and regulator identifiers are all visible in permitted human-readable sources.
9. Ran shortcut searches combining the historical institution, date, statutory category, and proposed value. No result exposed the intended institution-field-value join.

### Current status

One 129-word Finance candidate passed the entity, event-date, period, semantic-type, source-format, visual-verification, shortcut, grammatical-attachment, and process-instruction gates. Its difficulty does not depend on JSON, YAML, a large text export, Ctrl+F, arithmetic, or an obscure field code supplied without meaning.

The candidate retains four source-grounded failure points after the acquisition is recognized: acquired institution versus surviving institution, target certificate versus successor certificate, pre-consummation quarter, and account count versus adjacent dollar amount. The exact prompt, answer, identifiers, URLs, and distractor values remain in ignored local notes.

No target-model prompt was tested and no platform form was submitted by the agent. The candidate is ready for one fresh user-run GPT-5.5 extended-thinking test.

### Reusable lessons

- A surviving bank's certificate can silently redirect a historical lookup away from the acquired reporter even when the later brand name looks correct.
- Bank charter type and form type are useful cross-checks: a national bank with foreign offices should not be replaced by a state bank filing a domestic-only form.
- A statutory reporting category can create a meaningful semantic fork when the filing separately reports an amount and a count.
- State role labels are safer than repeated pronouns when a transaction involves several similarly named bank subsidiaries.
- The public facsimile's direct HTML URL is a reviewer-friendly terminal source because it renders the completed PDF while preserving institution and date parameters.

## 2026-08-04 - conversation-limit failure and evidence-safe diagnosis

### Outcome

The user manually ran the candidate in the required extended-thinking target. After more than ninety minutes, the session reached its conversation-length limit without a finalized response. One integer had been surfaced before the limit, but a fresh check of the official completed filing showed that integer was not the verified gold.

This is recorded as a failure to complete before the session limit. It is not recorded as a finalized wrong-answer run, and elapsed time alone is not the reason for the classification. No target-model query or platform submission was made by the agent.

### Diagnosis boundary

The official filing still proves the stored gold and separates the requested count from the adjacent dollar amount and other nearby counts. The incomplete run, however, does not provide enough reasoning evidence to locate the first internal divergence. A wrong institution, reporting period, or semantic field would all be possible stories, but none is established by the surfaced integer alone.

The golden package therefore explains only what the evidence supports: the target did not finish, its visible candidate is absent from the correct terminal cell, and the exact internal cause is unknown.

### Reusable lessons

- A long runtime is retrieval-cost evidence, not automatically a failure. A session-ending limit with no finalized response is a separate observable outcome.
- Keep `visible candidate`, `final answer`, and `platform result` as distinct fields in the test record.
- Reverify the gold after an incomplete run; do not assume that a stalled model makes the stored answer correct.
- Without a completed reasoning trace or a source-matched wrong value, stop the diagnosis at the first fact that can be proved.
- State uncertainty narrowly. Honest causal limits make a golden package stronger than a confident but invented wrong-path explanation.
- Preserve human-readable HTML/PDF evidence with exact page locations even when the model never reaches a terminal response.

## 2026-08-05 - process-instruction repair after prompt review

### Review outcome

A previously verified acquisition-and-filing prompt was returned because its wording did too much of the solver’s work. It used imperative entity-selection and exclusion clauses, assigned successive facts to named regulatory sources, disclosed the complete terminal form coordinate, and ended with an imperative integer-only instruction.

### Repair and lessons

- Freeze the verified answer, failure diagnosis, trajectory, and direct terminal source when the defect is prompt wording alone.
- State the transaction participants and geography as historical facts, then ask naturally for the semantically named financial figure.
- Remove agency-by-agency attribution, form number, schedule, item, column, mnemonic, certificate, and report date from the prompt when the evidence chain can discover them.
- Replace `select`, `exclude`, and `answer with` with an interrogative whose subject already fixes the legal entity, reporting period, field meaning, unit, and expected numeric type.
- Treat the repaired wording as a new prompt version. The old target response and share link cannot support it; a fresh user-run test is mandatory.
