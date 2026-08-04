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

## 2026-08-04 - reviewer return for large-file navigation

### Review outcome

A submitted Science trajectory was returned even though the reviewer agreed that its final answer held. The reviewer challenged two nonterminal distractor descriptions and, more importantly, rejected instructions that told a solver to search multi-megabyte text exports. The terminal answer cannot depend on Ctrl+F through a massive flat file.

### Evidence audit and repair

The official export was downloaded again before editing. That audit did not support the reviewer's proposed replacement identifiers. Because the disputed distractors were not needed to prove the answer, the repair does not argue over them or substitute unverified numbers; it removes them from the submitted trajectory.

The USGS release provides the same tables as official Excel workbooks. The replacement path uses header filters in the location workbook to isolate one record, then filters the analysis workbook by that record key and the scientifically selected mineral. The final filter leaves one row, from which the mapped identifier is read directly. The prompt, gold answer, primary-paper logic, and schema mapping do not change.

### Reusable lessons

- A source can be authoritative yet operationally unsuitable. Multi-megabyte text exports need a navigable official alternative for reviewer reproduction.
- Do not use Ctrl+F as the terminal-answer method in a large flat file. Prefer an official spreadsheet or database interface with named-column filters.
- State every filter field, operator, and value. `Filter the record-key column to X, then the mineral column to Y` is reproducible; `search the file` is not.
- Distinguish database field values from spreadsheet row numbers. Never describe an identifier as a visible row number.
- Do not automatically adopt a reviewer's proposed correction when the cited primary source contradicts it. Re-audit first, then remove unnecessary contested details if they do not contribute to the proof.
- Keep the golden trajectory minimal. Every extra distractor citation creates another factual claim that can fail review without helping establish the answer.

## 2026-08-04 - wall-to-wall source-mapping rejection

### Platform result

A scientifically valid candidate with a verified wrong target answer failed the process-instruction check. Nearly every clue was attributed to a named source in the order the solver was expected to use it. Although the prompt was phrased as a question, it narrated the research route from identity page to historical compilation to terminal database.

### Wording repair

The answer and complete verification package were frozen. The revised prompt states the location, relative position, age, stratigraphy, sample, and correction details as factual clues without naming the intermediate sources. Only the terminal database remains named because the requested value is explicitly a field in that database.

The revision does not add search verbs, URLs, page numbers, source order, sample identifiers, record identifiers, field names, or either competing value. The solver must independently discover the identity source and historical analysis before reconciling the terminal row and schema field.

### Reusable lessons

- A multi-source prompt should require source discovery, not label every clue with its source.
- Repeated constructions such as `the page states`, `the report identifies`, and `the database records` can turn a question into a disguised lookup script.
- Name a source only when the source itself is part of the requested coordinate, such as a value in a specified fixed database.
- Convert intermediate source attributions into standalone factual clues while preserving every uniqueness constraint.
- When a process check fails but the evidence graph remains sound, freeze the answer and golden package. Repair only the prompt wording.
- Re-run grammar and source-necessity audits after removing attribution; source hiding must not create ambiguous pronouns or decorative sources.

## 2026-08-04 - proactive terminal-table accessibility repair

### Audit result

The large-flat-file lesson from a returned Science submission was applied to another candidate before review. Its scientific proof and answer were unchanged, but both database-table citations still used text exports and the terminal step asked the reviewer to find a row in the final text file.

### Repair

Both text files were replaced by official workbooks from the same agency release. The location workbook now has two named-column filters that leave one record. The analysis workbook has record-key, laboratory-sample, and mineral filters that leave one terminal row. The correction comment, mapped field, and answer are then read from that row without Ctrl+F.

### Reusable lessons

- Apply reviewer lessons across every active candidate, not only the submission that received the comment.
- A smaller text export can still fail the terminal-source rule; file size is not the only issue when Ctrl+F locates the answer.
- Preserve the source ecosystem and evidence by switching formats within the same official release rather than changing the scientific chain.
- Reconfirm that each specified filter sequence leaves exactly one row before replacing the submitted sources.
- Keep raw text exports locally for audit if useful, but omit them from the trajectory and verification-source list.

## 2026-08-04 - heading-versus-detail identifier reconciliation

### Research decision

A new answer-first design begins with an internal nomenclature conflict in a fixed engineering report. A summary heading attaches one measurement identifier to an anomaly, while the detailed discussion assigns a different identifier to the described channel. An independent telemetry dictionary establishes that the heading's identifier belongs to a related tank measurement and that the detailed identifier belongs to the actual interface measurement.

The corrected identifier is then carried into a historical visual format matrix. The wrong and right identifiers occupy adjacent cells in the same subformat column, creating a grounded confuser: a solver that trusts the heading can reach the correct terminal table and still return the neighbouring coordinate.

### Verification performed

- Rendered both report passages and confirmed that the pressure offsets and mission timestamp describe the same anomaly.
- Rendered the independent telemetry dictionary and verified the distinct channel titles for both identifiers.
- Rendered the terminal matrix and checked the identifier, subformat column, and word/bit row visually.
- Audited the surrounding terminal pages so that a continuation-caption defect could not change the selected cell.
- Ran combined exact searches using both identifiers, the anomaly timestamp, the terminal format name, and likely coordinate vocabulary. No terminal coordinate was exposed.
- Confirmed that the terminal source is a fixed human-readable PDF table and requires neither a machine endpoint nor a large-file text search.

### Reusable lessons

- An internal source inconsistency can create valid difficulty only when the prompt explicitly states which passage controls and an independent source resolves the nomenclature.
- Do not silently correct a historical heading. Preserve both printed identifiers in the audit and prove why one is a bounded confuser.
- Adjacent cells are useful only when the row choice follows from a substantive semantic distinction, such as tank pressure versus interface pressure.
- Reconcile the identifier before opening the terminal matrix; visual row-column reading cannot repair a wrong entity carried into the table.
- Audit continuation captions and surrounding pages whenever a terminal table crosses page boundaries. A caption defect must be documented and shown not to affect the answer.
- Keep the prompt factual and compact. The solver should discover the report and dictionary rather than receive a source-by-source itinerary.

### Current status

The candidate passed provenance, nomenclature, visual-alignment, adjacent-confuser, direct-answer, accessibility, grammatical-attachment, process-language, and shortcut gates. No agent-run target-model test or platform submission occurred. Exact wording, identifiers, coordinates, URLs, and test status remain in ignored local notes.
