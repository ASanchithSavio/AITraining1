# Science & Technology training log

## 2026-08-03 - cross-ecosystem database and schema candidate

### Prior evidence used

- A previously successful technical-table design showed that a model can choose a nearby value when calibration, row scope, and column meaning all matter.
- The general domain ranking therefore favors cross-version joins, renamed fields, and footnote-controlled scientific records over a simple fact from an obscure report.

### Research decisions

1. Mined a completed federal geochronology database answer-first because its static text exports contain one-to-many specimen records and an authoritative old-to-new schema appendix.
2. Rejected an initial specimen design after discovering that all decisive evidence came from one agency host and that the source report duplicated several tempting terminal values.
3. Rebuilt the source graph across three ecosystems: a park geology source identifies a formation, an original peer-reviewed study selects between scientific mineral records, and a fixed federal database plus schema crosswalk supplies a database-only identifier.
4. Made the original study's concentration comparison control the terminal mineral row rather than merely name the study.
5. Verified the complete location and analysis exports programmatically, then checked the decisive report and schema pages visually or against the primary full text.
6. Confirmed that the descriptive clue matches one location record, the scientific selector matches one mineral row, and the final identifier is unique in the selected record.
7. Ran exact searches using the location clue, schema code, mineral, concentration, and likely combined queries; none exposed the answer.

### Current status

One 90-word Science candidate passed the domain, atomicity, source-independence, schema-mapping, row-uniqueness, directly-printed-answer, and shortcut gates. Its exact prompt, gold answer, source URLs, record identifiers, field mapping, and verification path remain in ignored local notes.

The difficulty hypothesis is a three-stage reconciliation: resolve a formation from a location clue, use a primary paper to choose between two nearby mineral separates, and translate a historical schema clue into the correct field of a large static export. The terminal answer is an identifier printed by the database, not a value calculated from the paper.

No ChatGPT prompt was tested by the agent and no platform form was submitted. The candidate is ready for one fresh user-run target-model test, not claimed to be empirically difficult until that result is returned.

### Remaining risks

- The publisher page for the historical paper may require access even when an author-posted full-text copy is readable elsewhere. A failure caused only by access should not be confused with a reasoning failure.
- The database is old but fixed; a solver may still discover a highly efficient text-export route and answer correctly.
- The schema clue must be interpreted as a field mapping, not as a request to reconstruct an obsolete database value.

## 2026-08-03 - first user-run target failure

### Outcome

The user tested the verified Science candidate in a fresh extended-thinking target-model session. The model returned a meaningfully wrong integer. A fresh audit of the primary paper, schema crosswalk, and every row in the matching database record confirmed that the stored gold answer was correct. No agent-run model test or platform submission was made.

### First divergence

The wrong integer belongs to a blank duplicate whole-rock row inside the correct database record. The requested row was the unique mineral-separate row selected by the larger of two concentrations printed in the primary paper. This indicates a terminal row-scope error rather than failure to identify the broad study or database record.

### Reusable lessons

- A wrong value drawn from the correct record can be stronger evidence than an unrelated guess: it shows that retrieval succeeded while schema and row selection failed.
- Carry semantic scope all the way to the terminal row. `Mineral separate` excludes rows explicitly classified as `whole rock`, even when their sample labels look like abbreviations for minerals.
- Audit all duplicate and blank companion rows before accepting an analysis number from a one-to-many export.
- Use the primary paper's comparison before reading the identifier field. Reversing those operations encourages selection of a convenient nearby row.
- A historical-to-current field crosswalk controls the column only; it does not identify the correct row. Column mapping and row selection are separate decisions, and both must be verified.

### Current status

The candidate initially appeared to have one user-reported target failure. The later grammatical-attachment rejection returned the wording to preflight, so that model result is provisional rather than a valid benchmark failure. Exact wording, answer values, record identifiers, URLs, and test details remain in ignored local notes.

## 2026-08-03 - grammatical attachment rejection and repair

### Observed

The platform's grammatical attachment check rejected the tested Science wording. Three singular pronouns in one clue sentence could each point to more than one nearby entity. The scientific chain and gold answer remained verified, but the prompt did not pass the validity gate.

### Cause

The wording compressed a specimen, a database value, a volcanic province, and a study into one semicolon-linked sentence. Reusing possessive and subject pronouns required the reader to infer the intended owner from scientific context rather than from grammar alone.

### Change

The repaired version uses separate sentences and repeats the controlling nouns: the database field, the mineral separate, and the study. It preserves every selector and does not reveal the formation name, mineral name, record number, concentration values, or terminal field name.

### Result and rule

The revised prompt remains within the word limit and is ready for a fresh attachment check. The earlier wrong target answer is provisional and cannot be credited to the revised wording until the new version is evaluated.

For future candidates, run an explicit antecedent audit after all content edits. If two singular entities appear near `it` or `its`, replace the pronoun even when the intended reading feels obvious. Grammatical validity must be established before model difficulty is counted.

## 2026-08-03 - explicit-noun repair accepted

### Outcome

The user confirmed that the revised wording fixed the immediate problem. This records success of the grammatical repair only. No fresh target-model answer or terminal platform judgment for the revised candidate was reported, so the candidate's empirical difficulty remains unevaluated.

### Why the repair worked

- The revision removed every disputed `it` and `its` attachment.
- Each sentence names the controlling entity directly: field, mineral separate, formation, or study.
- The scientific selectors and the gold answer did not change, so the repair improved validity without making the research chain easier.
- The prompt no longer asks a reader or an automated checker to recover ownership from scientific context.

### Reusable rule

Treat exact-noun repetition as precision, not stylistic redundancy, in benchmark prompts. After drafting, list every pronoun, possessive, relative clause, and trailing modifier. If a phrase could attach to two preceding nouns under ordinary grammar, replace it with the intended noun before any model test.

## 2026-08-04 - correction-controlled fission-track candidate

### Research decision

After a Business directory design collapsed to one row lookup, research returned to a fixed scientific database with a materially different terminal mechanism. The new answer-first design begins with a historical analysis whose published density is explicitly marked erroneous by the later database. The corrected row also contains a different field beginning with the same digits as the obsolete value, creating a grounded same-record confuser rather than arbitrary nearby noise.

The source graph uses three independent ecosystems. A public scientific-interpretation page identifies the physical feature, a historical compilation identifies the specimen and prints the superseded value, and a federal database plus its authoritative appendix supply the correction and old-to-current field mapping. Each source changes the selection state.

### Verification performed

- Matched the historical specimen description, mineral, locality, laboratory identifier, and citation to one location record and one analysis row.
- Proved from the appendix that the requested legacy label maps to the corrected density field, not the decay constant, track count, adjacent density, age, or concentration fields.
- Rendered the historical analytical entry and schema table at original resolution to verify row and column alignment.
- Confirmed that the answer is directly printed in a human-readable static export and requires no conversion or calculation.
- Ran exact and combined shortcut searches across the feature description, laboratory identifier, correction wording, legacy label, current field, and candidate value. The corrected entity-field pair was not exposed, while the obsolete published value remained an accessible temptation.
- Repeated explicit nouns and removed ambiguous singular pronouns. The prompt withholds the feature name, specimen identifier, record number, both competing values, and current field name.

### Current status

The candidate passed source necessity, independent-host, correction provenance, schema mapping, row uniqueness, direct-answer, visual alignment, accessibility, grammatical attachment, and shortcut gates. No agent-run target-model test or platform submission occurred. Exact wording, values, identifiers, URLs, locators, and confusers remain in ignored local notes for one fresh user-run evaluation.

### Reusable lessons

- A historical correction is strong only when the old source actually prints the wrong value and the later authoritative record explicitly marks it as erroneous.
- Pair correction control with field control. Finding the corrected record should not by itself reveal which of several related fields answers the question.
- Same digits in a wrong current field create a particularly credible failure path: a solver can notice the correction but still choose the wrong schema coordinate.
- Preserve at least two post-discovery decisions: reconcile the historical specimen to the current row, then translate the legacy field label to the current column.
- Treat the original value, corrected value, and similarly shaped current values as separate provenance claims and verify each before release.

## 2026-08-04 - first user-run result for the correction candidate

### Outcome

The user-run extended-thinking target model returned a decimal different from the verified database value. The agent did not run a target-model test and no platform submission was reported. A fresh source audit confirmed the historical entry, database row, analytical correction comment, and legacy-to-current field mapping.

### Failure classification

The returned decimal does not appear in the selected row or anywhere in the complete fixed analysis export. It is not one of the documented wrong-field or obsolete-value confusers. The supported label is therefore an unsupported corrected-value substitution, not a proven row-selection or column-selection error.

The model may have understood that the published value was obsolete but failed to ground the replacement in the exact current cell. That mechanism remains an inference from the terminal answer, so it should not be presented as known internal reasoning.

### Reusable lessons

- Search the returned value across the entire authoritative export before assigning a failure class.
- If the value belongs to a real neighbouring row or field, diagnose the precise scope error. If it appears nowhere, record unsupported numeric substitution instead of inventing a provenance story.
- A correction prompt can expose a distinct weakness: recognizing that an old value is wrong is not the same as retrieving the authoritative replacement.
- Golden rules should explicitly prohibit averaging, interpolation, unit conversion, and plausible-value reconstruction when the answer is directly printed.
- Preserve the exact user-run result privately and wait for the terminal platform judgment before calling the candidate a benchmark success.
