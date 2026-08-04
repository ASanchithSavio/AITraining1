# Health & Medicine training log

## 2026-08-04 - regulatory action to trial protocol to review-table candidate

### Prior evidence used

- The strongest Business result came from preserving a child entity through a dense parent-and-sibling chart.
- The strongest Finance result came from carrying the correct legal entity, period, and form coordinate into a terminal record.
- The Science wording repair showed that a valid source graph is still unusable when pronouns or possessives have competing grammatical attachments.
- Correct responses in other domains showed that long retrieval time and visual documents do not establish difficulty by themselves.

### Research decisions

1. Selected a completed historical drug withdrawal so the product and regulatory application are fixed.
2. Used a dated publication of two sibling hemodialysis trials in which the sign of a reported between-group result uniquely selects one trial.
3. Added a separate public medical-evidence table that maps the selected trial nickname to the sponsor's regulatory protocol identifier.
4. Carried that protocol identifier into the original FDA medical review rather than relying on a shared trial nickname.
5. Selected a terminal baseline-characteristics table organized by two trials and two treatment arms per trial.
6. Chose a directly printed endpoint of a laboratory-value range. The same row contains a lower endpoint plus three other treatment-arm ranges, creating several source-grounded confusers without requiring arithmetic.
7. Rendered the terminal page and visually verified the study headers, treatment subcolumns, row label, unit, range, and footnotes.
8. Confirmed that the submitted evidence path can use human-readable HTML and PDF only. No JSON or YAML is needed.
9. Ran shortcut searches using the protocol identifier, laboratory row, range endpoint, product class, and trial nickname. No search snippet exposed the complete intended entity-value pair.
10. Rewrote the prompt with explicit nouns for the selected trial, evidence table, protocol identifier, regulatory review, and application drug.

### Current status

One Health & Medicine candidate passed the historical-stability, non-advice, atomicity, four-ecosystem source, trial-selection, protocol-mapping, treatment-arm, range-endpoint, visual-verification, source-format, shortcut, and grammatical-attachment gates.

The exact prompt, gold answer, drug, application number, trial names, protocol code, URLs, page coordinate, and confuser values remain in ignored local notes. The agent did not query the target model and did not submit a platform form. The candidate is ready for one fresh user-run test.

### Remaining empirical risk

Once the protocol identifier is known, the target may locate and align the regulatory table correctly. The source chain is valid, but only the terminal target result can establish whether the combined sibling-trial, treatment-arm, and range-endpoint decisions are difficult enough.

### Reusable lessons

- A trial nickname is not a safe join key when regulatory reviews use sponsor protocol identifiers.
- The sign of a published comparative result can select one of two sibling trials without disclosing the protocol code.
- A dense regulatory table can support several fair confusers when study, treatment arm, statistic, and range endpoint must all remain in scope.
- Historical withdrawal notices are useful identity anchors, but they contribute difficulty only when later sources still require independent trial and table decisions.
- Keep historical record lookup separate from present-day treatment guidance.
