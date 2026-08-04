# Business training log

## 2026-08-03 - answer-first archival ownership chart

### Prior evidence used

- The Finance failure showed that a shared corporate name can pull a model onto the wrong legal entity.
- The retired Art candidate showed that an adjacent-row trap alone may add time without changing the final answer.
- The strongest Science result combined record selection with a separate terminal-coordinate decision.
- The Business search therefore required two independent selections before a visually aligned historical chart lookup.

### Research decisions

1. Rejected recent annual reports and ordinary plant tables whose values or product lists appeared in search snippets.
2. Mined a university collection of historical corporate reports from the answer backward rather than drafting clues first.
3. Selected a fixed statistical booklet containing a full-page organization chart with multiple subsidiaries, ownership percentages, and incorporation or acquisition dates.
4. Used an older government enforcement report to identify the chart's parent corporation without naming the parent in the candidate.
5. Used a later, independent government vessel notice to select one operating subsidiary without revealing the subsidiary in the candidate.
6. Confirmed that the terminal chart contains two neighbouring same-type companies in the same jurisdiction with different ownership percentages. The sibling percentage is a plausible, source-grounded wrong answer.
7. Rendered the enforcement page, vessel-notice page, and terminal chart. Visual inspection confirmed the names, the vessel-to-owner pairing, the chart branches, and the percentage alignment.
8. Ran exact and natural shortcut searches combining the booklet date, subsidiary, parent, chart terminology, and proposed answer. No indexed result joined the intended subsidiary to the terminal percentage.
9. Rewrote the candidate with explicit nouns. No pronoun can attach to the parent, subsidiary, vessel, notice, or neighbouring company in competing ways.

### Current status

One Business candidate passed the domain, atomicity, stability, three-host independence, source-necessity, corporate-hierarchy, same-type-confuser, visual-alignment, shortcut, and grammatical-attachment gates. The exact prompt, gold answer, URLs, document identifiers, page coordinates, and sibling value remain in ignored local notes.

The difficulty hypothesis has three stages: identify the historical parent from an enforcement description, identify the target subsidiary from a vessel record, and align that subsidiary to the correct percentage in a dense ownership chart. The neighbouring same-type company prevents a broad jurisdiction or industry match from being sufficient.

No target-model prompt was tested and no platform form was submitted by the agent. The candidate is ready for one fresh user-run GPT-5.5 extended-thinking test. It is not claimed to be empirically difficult until that test returns a final answer.

### Reusable lessons

- Old corporate charts are stronger terminal sources than generic annual-report prose when relationship lines and sibling entries control the answer.
- A later registry or government notice can legitimately select a historical subsidiary when the legal name is unchanged and the notice supplies a unique independent key.
- The parent-identification source and subsidiary-identification source should contribute different lookup keys; neither should merely repeat the other.
- OCR from organization charts often scrambles percentages and dates. The rendered chart, not extraction order, determines alignment.
- A warning to use the target row rather than the neighbouring same-type row can improve fairness without disclosing either value.
- Keep Business ownership and operations research separate from Finance tasks built around accounting fields, reporting periods, or monetary values.

## 2026-08-04 - first user-run target failure

### Outcome

The user reported a wrong percentage from the required extended-thinking target model. Rechecking the three source handoffs and the rendered organization chart confirmed the stored gold answer. The returned percentage is printed on the correct chart, but it belongs to the target subsidiary's immediate parent rather than to the subsidiary selected by the independent vessel record.

### First established divergence

The target reached the correct corporate branch but stopped one level too high in the hierarchy. This is a parent-versus-subsidiary scope error, not an arithmetic, date, publication-version, or unrelated-entity error. Without a reasoning trace, the evidence does not show whether the connector line was misread, the parent's percentage was incorrectly inherited, or the final subsidiary-selection clue was dropped.

### Reusable lessons

- Compare every returned chart value against the target box, immediate parent, sibling boxes, and nearby dates before assigning a failure label.
- A wrong value printed beside the immediate parent is strong evidence of hierarchy-scope failure.
- An independent selector for a child company remains useful only if the terminal lookup carries that exact legal name all the way to the child box.
- Dense organization charts can create a legitimate failure mechanism when parent and child percentages are both plausible and visually close.
- Diagnose only the first error proved by the final answer. Do not invent an exact internal search path without the model's trace.

## 2026-08-04 - division-versus-main-list replacement architecture

### Why a new architecture was required

Another domain's multi-source candidate was answered correctly because its last identifier led to an indexed document and the prompt named the remaining table coordinate. That result reinforced a stricter Business rule: finding the terminal report must not reduce the task to one search-and-copy action.

Several historical corporate reports were screened and rejected. Ordinary financial tables, production summaries, and restated annual figures either became direct row lookups or exposed the entity-value pair in search snippets.

### Construction decisions

1. Selected a historical retail annual report whose store directory repeats the same geographic labels under two different organizational scopes.
2. Confirmed that the target borough has one count in the corporation's main network and a different count in a separately headed division. Both values are genuine same-field answers rather than unrelated nearby numbers.
3. Used one historical opinion to identify the annual-report publisher and a different opinion to identify the target division.
4. Used an independent library catalogue record to select the geographic row without naming the borough directly in the candidate.
5. Required the terminal lookup to preserve both organizational scope and geographic scope after the annual report is found.
6. Rendered the report's business-description page and both store-list pages. Visual inspection confirmed the division relationship, headings, hierarchy, duplicate borough label, and two different counts.
7. Ran shortcut searches joining the two historical marks, publisher, division, report year, geographic clue, and candidate value. No indexed result exposed the terminal division-borough pair.
8. Repeated explicit nouns in the prompt so the publisher, chain, borough, report, division section, and preceding list each have one grammatical role.

### Current status

One replacement Business candidate passed the domain, answer-first, source-necessity, post-document-decision, same-field-confuser, visual-verification, shortcut, source-format, and grammatical-attachment gates. Exact names, marks, answer, URLs, page coordinates, and distractor values remain in ignored local notes.

The agent did not query the target model and did not submit a platform form. The candidate is ready for one fresh user-run extended-thinking test. A correct terminal answer will retire it regardless of elapsed time.

### Reusable lessons

- Duplicate labels become useful only when they sit under different, independently selected organizational headings.
- A division-versus-main-network error is stronger than an arbitrary adjacent-row trap because the wrong value preserves the requested field and geography while losing entity scope.
- Use separate clues for publisher, sub-entity, and row. If one clue reveals two of those coordinates, the terminal lookup may collapse.
- After finding the terminal document, require at least two remaining decisions: which organizational section and which row within that section.
- Record totals at every hierarchy level before testing; a returned city, state, division, or corporate total can then be diagnosed precisely.
- A prompt may warn against the wrong organizational section without printing either value or turning the question into a browsing checklist.

## 2026-08-04 - source-format and locator preflight

### Audit outcome

The candidate's complete evidence path was rechecked after an earlier Finance submission had been returned for machine-readable sources. The Business path contains three human-readable PDFs and one HTML catalogue record. It contains no JSON or YAML. The three decisive PDF pages were rendered and visually inspected again.

One archive's original-asset URL has no filename extension. The URL shape alone is not the file format: the catalogue identifies the download as a PDF, the downloaded asset validates as a multi-page PDF, and the cited terminal page renders correctly. The catalogue page and original asset remain one source ecosystem even though both URLs are useful in the trajectory.

The locator audit also added the physical PDF page beside the printed page for each long government publication. This makes the proof reproducible in a browser PDF viewer without changing the prompt, answer, or reasoning chain.

### Reusable lessons

- Classify a source from its actual response and rendered content, not from whether its URL ends in `.pdf`.
- When an archive serves an extensionless original asset, cite the human-readable catalogue record as format metadata and cite the original PDF as the evidence document.
- Count the catalogue and original asset as one publication ecosystem, not two independent sources.
- State both physical and printed page numbers whenever pagination differs.
- Run the no-JSON/no-YAML check across the whole submitted path, including intermediate sources.

## 2026-08-04 - directory candidate answered correctly and retired

### Outcome

The user-run extended-thinking target model returned the verified terminal answer. No agent-run model test or platform submission occurred. The candidate is retired rather than rewritten.

### Why the architecture failed

The external legal and geographic joins identified the report publisher, target division, and target place without much resistance. The terminal report did contain the same place label under two organizational headings, but the prompt explicitly named the correct separately headed section and warned against the preceding list. That wording performed the only important scope decision for the solver. After document discovery, the task reduced to transcribing one clearly labelled row.

### Reusable lessons

- A real duplicate row is not automatically a strong confuser. The solver must still have to determine which heading governs the requested entity.
- Reject a directory prompt when an exclusion sentence names the correct subsection so precisely that only one row remains.
- Do not mistake a long source chain for terminal difficulty; audit the decisions remaining after the last document opens.
- When a prompt is answered correctly, retire the mechanism if the weakness is structural. Adding more upstream clues or indirect wording does not restore a missing terminal decision.
- A future organizational-scope design should make independent evidence select the subsection without spelling out its label in the question.

## 2026-08-04 - answer-first fire-insurance protection note

### Why this mechanism was selected

Several answer-first candidates were rejected before drafting. Historical-statistics errata exposed corrected values in indexed snippets. A corrected patent title became a direct certificate transcription after the patent was identified. A historical drug-table route lacked a stable, human-readable edition path. Each route failed either the shortcut gate or the post-document decision gate.

The retained Business mechanism begins with a visually buried operating fact in a historical fire-insurance map. A university archival record identifies a founder, a state preservation record selects the correct company property and construction event, and a federal map collection supplies the edition chronology, special index, and terminal sheet. The upstream records do not print the answer.

### Construction and verification decisions

1. Chose an industrial property with several similarly named plants so entity selection remains meaningful after the company is known.
2. Used a dated addition to select the first map edition after a real physical change instead of printing the map year in the prompt.
3. Required the volume's special index to locate the property sheet. The map is not reached through an exact answer-bearing search result.
4. Selected a terminal fire-protection note containing several figures about one water system: a normal supply tank, an emergency reservoir, and a pump rate. These are semantic confusers, not arbitrary neighbouring numbers.
5. Verified that the requested figure appears only on the map sheet and is not repeated in the preservation nomination. An upstream record does mention one wrong-component figure, which creates a plausible documented error without leaking the answer.
6. Rendered and visually inspected the decisive nomination pages, map index, full property sheet, and an original-resolution crop of the note. OCR was used only as a discovery aid and not as alignment proof.
7. Ran exact and natural searches joining the company, property, sprinkler language, equipment type, and candidate value. No result exposed the intended entity-value pair.
8. Rewrote the question with explicit nouns and only one generic reference to the terminal source type. It does not narrate a source-by-source itinerary.

### Current status

One candidate passed the Business-domain, answer-first, source-necessity, edition-selection, index-navigation, same-system-confuser, visual-verification, shortcut, source-format, process-instruction, and grammatical-attachment gates. Exact names, prompt, answer, URLs, sheet coordinate, and distractor values remain in ignored local notes.

The agent did not test the target model and did not submit a platform form. The candidate is ready for one fresh user-run extended-thinking test and is not claimed to have failed the model until a terminal response is reported.

### Reusable lessons

- Fire-insurance maps can provide strong Business terminal evidence when the requested fact concerns manufacturing operations rather than geography alone.
- Prefer several figures in one operational system over a random adjacent-row trap. Tank capacity, reservoir capacity, and pump flow are close in topic but have different equipment roles.
- A dated building addition can select a map edition naturally, provided the edition sequence is independently verifiable.
- Make the map index a consumed decision: the historical record identifies the property, while the index supplies the printed sheet.
- Check every upstream narrative for the final value. If the answer is repeated before the terminal source, the map step is decorative and the candidate should be rejected.
- For image-based evidence, record both the sequence image and printed sheet, then verify the exact wording at original resolution.
- Mentioning one terminal source type is not a wall-to-wall source map. Naming every intermediate archive, publication, and lookup step in the prompt is.

## 2026-08-04 - fire-insurance candidate answered correctly and retired

### Outcome

The user-run extended-thinking target returned the independently verified terminal value after roughly half an hour. No agent-run target test or platform submission occurred. Because the final answer was correct, the candidate is retired regardless of the long runtime.

### What the result shows

The target successfully preserved all of the intended distinctions: original plant rather than later plant, first map edition after the addition, indexed property sheet, normal sprinkler supply rather than emergency storage, and capacity rather than pump rate. The visual map and same-system confusers increased research time but did not create a durable model failure.

### Reusable lessons

- A long attempt is not evidence that a candidate stumped the target. Wait for the terminal answer and compare it with the verified gold.
- Multiple post-document decisions can still be jointly solvable when every decision has explicit archival support and the terminal note labels each equipment role clearly.
- Image-only evidence and grounded confusers improve quality but do not guarantee failure against extended reasoning.
- Retire a correctly answered architecture instead of adding more upstream identity clues. Extra founder, property, or edition clues would increase length without changing the terminal mechanism.
- For the next Business candidate, change the evidence operation itself: consider a controlling amendment, cross-document nomenclature conflict, or version-dependent coordinate rather than another map-note transcription.

## 2026-08-04 - railroad annual-return candidate

### Research decision

After the fire-insurance-map mechanism was solved correctly, the replacement Business design moved to a historical common-carrier annual return. Independent corporate and operating-history sources distinguish two short lines under one parent and select the reporting year through a fixed ownership event. The terminal return then requires both a service-row choice and a freight-versus-passenger column choice.

### Verification performed

- Verified the target route and the sibling railroad from independent historical sources.
- Fixed the report year from the parent-company transaction rather than exposing the year as an instruction.
- Rendered the annual-return schedule and checked the service-row and column alignment visually.
- Recorded the road-service figure and total as same-table confusers.
- Confirmed that natural searches did not expose the carrier-year-field-value join.
- Confirmed a human-readable HTML/PDF evidence path with no calculation, JSON, YAML, or flat-file search.

### Status and lesson

The candidate is ready for one user-run target-model test. Exact entities, values, URLs, and wording remain in ignored local notes. A railroad route is useful only when it distinguishes a carrier from a real sibling; the ownership event is useful only when it selects the report year; and the terminal schedule remains substantive only when both row and column scope must be preserved.
