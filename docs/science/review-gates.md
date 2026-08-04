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
- Check that a report table does not already print the terminal answer; otherwise the database handoff is decorative.
- Audit every same-sample row, blank duplicate, mineral separate, whole-rock entry, and neighbouring value before claiming uniqueness.
- If parsing is needed, preserve the direct text or table as the final evidence and use code only to confirm uniqueness.

## Difficulty after identification

- At least two meaningful choices should remain after the main study or dataset is found.
- Strong mechanisms include specimen reconciliation, old/new schema mapping, mineral-versus-whole-rock selection, corrected-versus-original values, and version-scoped appendix lookup.
- A single sample number followed by one exact row is weak even when the database is large.
- A field-code clue is useful only when resolving it changes the selected column; unexplained jargon is not difficulty.
- Reject a corrected-value prompt if finding the correction leaves only one obvious field. Require a separate specimen, version, or schema decision after the relevant record is discovered.

## Accessibility and shortcut audit

- The primary study, terminal export, and field crosswalk must be readable without proprietary software.
- Visually inspect decisive PDF tables or figures when layout controls row or column alignment.
- Search the specimen description, field code, terminal value, and likely post-identification query combinations.
- Reject candidates whose answer appears in snippets, alternate table extractions, or an obvious exact query.
- Record publisher-access or author-copy dependencies as retrieval risks before testing.

## Promotion gate

Promote a Science candidate only when all of these are true:

- the final row and field are unique;
- every source changes the selection state;
- the independent-host requirement is satisfied;
- the answer is printed rather than derived;
- the prompt does not narrate a complete lookup script;
- the exact-search audit does not expose the answer; and
- no agent-run target-model test or platform submission has occurred unless the user explicitly requests it.
