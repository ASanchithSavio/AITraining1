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
