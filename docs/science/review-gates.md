# Science & Technology review gates

Use these gates with the general method. Exact candidates, answers, record identifiers, URLs, and test outcomes remain in ignored local notes.

## Domain and answer

- The question is native to scientific or technical research rather than a historical identity chain with a scientific label.
- The answer is one directly printed value, name, code, or phrase from a completed, stable record.
- Units, precision, method, version, and field meaning are explicit wherever they can change the answer.
- No required step asks the solver to calculate, interpolate, convert, or infer an unprinted value.

## Source graph

- Use at least three genuinely independent publication ecosystems when the benchmark requires independent hosts.
- Prefer a scientific identity source, an original study or report, and a terminal dataset, catalog, standard, or appendix that each supplies a consumed selector.
- Do not count several files from one agency database as independent ecosystems.
- Reject an upstream source if the terminal dataset already contains the same discriminator or if the source merely confirms the record's identity.
- An original paper must change which specimen, method, version, mineral, calibration, or row controls the answer.

## Record and schema handling

- Verify the terminal record in the distributed data, not only in a landing-page description or search snippet.
- When a schema changed, prove the old-to-new field mapping from the authoritative crosswalk and identify which exported column actually carries the answer.
- For a correction-controlled candidate, verify that the historical source prints the superseded value and that the later authoritative record explicitly identifies the published value as erroneous. Do not infer a correction merely because two releases disagree.
- Keep correction provenance and field mapping independent: the correction must select the controlling version, while the crosswalk must still select the controlling column.
- Audit same-digit values in other current fields. A decay constant, count, density, age, or concentration that resembles the obsolete value must be documented as a wrong-field confuser, not silently ignored.
- After a target miss, search the returned value across the selected row and complete authoritative export. Label a row or field error only when the value has a real documented provenance; otherwise use an unsupported-value classification.
- Check that a report table does not already print the terminal answer; otherwise the database handoff is decorative.
- Audit every same-sample row, blank duplicate, mineral separate, whole-rock entry, and neighbouring value before claiming uniqueness.
- If parsing is needed, preserve the direct text or table as the final evidence and use code only to confirm uniqueness.
- When a report heading and detailed discussion assign different identifiers to the same described anomaly, do not choose silently. State which passage controls, verify both identifier meanings in an independent dictionary, and preserve the rejected identifier as a documented confuser.
- If a multi-page table has a conflicting continuation caption, inspect the preceding and following pages and prove that the row family and identifier prefix still place the target in the intended table section.

## Difficulty after identification

- At least two meaningful choices should remain after the main study or dataset is found.
- Strong mechanisms include specimen reconciliation, old/new schema mapping, mineral-versus-whole-rock selection, corrected-versus-original values, and version-scoped appendix lookup.
- A single sample number followed by one exact row is weak even when the database is large.
- A field-code clue is useful only when resolving it changes the selected column; unexplained jargon is not difficulty.
- Reject a corrected-value prompt if finding the correction leaves only one obvious field. Require a separate specimen, version, or schema decision after the relevant record is discovered.
- For a telemetry or format matrix, require independent evidence to select both axes. A prompt that directly supplies the channel and mode leaves only visual transcription.
- When two adjacent parameter rows are confusable, make the row choice depend on a verified semantic distinction such as component role, measurement state, or a comparison at one historical event.

## Accessibility and shortcut audit

- The primary study, terminal export, and field crosswalk must be readable without proprietary software.
- For a large terminal table, provide an official navigable format and an exact filter sequence. Reject instructions that rely on Ctrl+F or an unspecified search through a multi-megabyte flat file.
- Name the filter column, operator, and filter value for every large-table reduction, and confirm that the final filter leaves one row.
- Keep database identifiers, worksheet row numbers, and line numbers separate in both wording and verification notes.
- Visually inspect decisive PDF tables or figures when layout controls row or column alignment.
- For a decisive table inside a long PDF, record the physical page, printed page, table title, row selector, and column selector in the golden trajectory. Never make whole-document search the terminal method.
- Search the specimen description, field code, terminal value, and likely post-identification query combinations.
- Reject candidates whose answer appears in snippets, alternate table extractions, or an obvious exact query.
- Record publisher-access or author-copy dependencies as retrieval risks before testing.
- For an erratum-controlled answer, search the operation or specimen label together with the exact terminal interval and correction vocabulary. Reject the candidate if one erratum sentence gives the complete old-to-new replacement.
- Do not treat a superscript flattened by OCR as a sufficient confuser when the operation heading and terminal coordinates still isolate the correction.

## Prompt language and process

- State intermediate evidence as factual clues rather than assigning each clue to a named page, paper, report, and database.
- Reject wall-to-wall attribution patterns such as `the page states`, `the paper identifies`, followed by `the database records`; this narrates the lookup chain even when no imperative verbs appear.
- Name the terminal source only when its identity is part of the requested coordinate. Let the solver discover intermediate sources.
- After removing source names, confirm that all clues still select one entity and that every pronoun, modifier, and relationship has one grammatical attachment.
- A process-instruction repair must not change the answer, evidence graph, golden trajectory, rules, or sources unless the underlying facts also failed review.
- Factual prose can still reveal a research itinerary when successive sentences correspond in order to one page, paper, workbook, and database.
- Introduce two specimens, domes, instruments, or channels by name before using `both`; never rely on an implied second member.
- Place viewpoint clauses beside `viewpoint`, sample clauses beside `sample`, and field-mapping clauses beside `field`. Repeat the noun when a nearby feature could capture the modifier.
- A repaired prompt requires a fresh target-model response and matching share link. Reviewer evidence from the earlier wording cannot be carried forward.
- If the platform's active authorship check requires human-written wording, do not provide another submission-ready LLM rewrite or describe an LLM-edited version as human-written. Freeze the verified scientific evidence and gold answer, wait for independently authored wording, and limit subsequent assistance to factual, grammatical, attachment, and alignment review.

## Promotion gate

Promote a Science candidate only when all of these are true:

- the final row and field are unique;
- every source changes the selection state;
- the independent-host requirement is satisfied;
- the answer is printed rather than derived;
- the prompt does not narrate a complete lookup script;
- the exact-search audit does not expose the answer; and
- no agent-run target-model test or platform submission has occurred unless the user explicitly requests it.

After a user-run evaluation, record elapsed time only as context. Promotion depends on the correctness of the final response and the platform gates, not on how long the target spent researching.
