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

### Manual result and disposition

The user-run target model returned the verified gold answer. The candidate is retired as a prompt-design failure. The agent did not query the target model and did not submit a platform form.

The failure was a post-identification collapse. A dated regulatory action exposed one application, a binary result selected one of two sibling trials, and a public crosswalk supplied the terminal review's exact protocol identifier. Once that identifier was carried into the indexed review, the prompt itself named the treatment arm, row, statistic, and endpoint. The last step was transcription rather than a durable scope problem.

The exact prompt, answer, identifiers, URLs, page coordinate, and user-run response remain in ignored local notes.

### Reusable lessons

- A trial nickname is not a safe join key when regulatory reviews use sponsor protocol identifiers.
- The sign of a published comparative result can select one of two sibling trials without disclosing the protocol code.
- A dense regulatory table can support several fair confusers when study, treatment arm, statistic, and range endpoint must all remain in scope.
- Historical withdrawal notices are useful identity anchors, but they contribute difficulty only when later sources still require independent trial and table decisions.
- Keep historical record lookup separate from present-day treatment guidance.
- Four necessary sources do not make a hard prompt when each source reduces the task to a single deterministic join.
- A terminal table with many adjacent numbers is weak when the prompt names every coordinate and the preceding source gives the table's exact searchable identifier.
- Reject `identity anchor -> binary selector -> explicit crosswalk -> named cell` designs before testing, even when the route is long and every confuser is source-grounded.

## 2026-08-11 - same-document distribution-to-case-table candidate retired

### Manual result

The user-run target model returned the verified total in 39 seconds. The response selected the intended filling lot, read the paralytic and non-paralytic subtotals correctly, rejected the manufacturer-order subtotal, and gave the correct final value. The candidate is retired as solved.

### Why the candidate was weak

- The prompt disclosed the report month, subject, manufacturer order, and the selected lot's complete four-jurisdiction distribution signature.
- The distribution signature uniquely identified one filling lot in Table 6; the answer then required carrying that printed lot number into Table 5 of the same 20-page report.
- The prompt explicitly warned against the manufacturer-order subtotal, revealing the principal row-scope trap before the solver encountered it.
- No independent source handoff, version boundary, terminology crosswalk, or unresolved scope decision remained after the report was found.
- The adjacent values were visually clear. They created a possible transcription error, not a durable reasoning failure.

### Reusable correction

Reject `unique row signature -> copied identifier -> nearby total in the same document` candidates. A second table counts as a real hop only when it introduces a new semantic or version decision; carrying an exact lot number between adjacent tables is ordinary lookup. Do not describe the intended wrong subtotal in the prompt unless that distinction must be inferred from independent evidence.
