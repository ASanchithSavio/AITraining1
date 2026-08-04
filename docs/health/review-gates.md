# Health & Medicine prompt review gates

Use these gates with the general method. Exact drug names, application numbers, trial names, protocol identifiers, values, URLs, and manual outcomes remain in ignored local notes.

## Domain and safety

- Keep the task about historical medical evidence, public-health reporting, clinical-trial records, regulatory review, drug labeling, or medical-device documentation.
- Ask for a fixed factual record, not diagnosis, treatment advice, present-day safety guidance, or a recommendation for an individual.
- Prefer completed trials, dated regulatory actions, original approval packages, and frozen surveillance reports.
- If a product was later withdrawn or superseded, make the historical date and document version explicit.

## Answer-first regulatory design

- Select the terminal table cell before writing clues. Record the study, treatment arm, population, row label, statistic, unit, and every adjacent value.
- Prefer original regulatory reviews with several sibling trials, treatment arms, and summary statistics in the same table.
- Do not use medical obscurity as the only difficulty mechanism. Require at least two meaningful selections after the drug or device is identified.
- Ask for a directly printed value or phrase. Do not require clinical interpretation, risk comparison, or arithmetic.

## Trial identity and protocol mapping

- Distinguish trial nickname, registry number, sponsor protocol identifier, application number, treatment arm, and analysis population.
- Use an explicit human-readable source when a published trial name must be mapped to a regulatory protocol code.
- Do not assume similarly named trials are interchangeable. Record the feature that uniquely selects one sibling trial.
- Carry the selected protocol identifier unchanged into the terminal regulatory table.

## Table scope and confusers

- Verify whether a table groups columns first by study and then by treatment arm, or first by treatment and then by study.
- Distinguish the application drug from the active comparator or placebo.
- Distinguish mean, median, range, confidence interval, count, and percentage.
- When asking for a range endpoint, state upper or lower explicitly and verify that no footnote changes the unit or population.
- Record same-row confusers from the comparator and sibling trial before release.

## Source and language preflight

- Use necessary sources from distinct publication ecosystems, such as a regulatory notice, published results, a registry or coverage evidence table, and an original review.
- Cite only human-readable HTML or PDF in the submitted path; do not cite JSON or YAML.
- Render the terminal PDF page and inspect column spans, headers, footnotes, and alignment.
- Repeat `selected trial`, `protocol identifier`, `application drug`, and the requested statistic when a pronoun or modifier could attach to multiple entities.
- Run shortcut searches combining the drug class, trial nickname, protocol code, terminal row, and proposed answer.

## Promotion gate

- A candidate that passes these checks is ready for one fresh user-run target-model test; it is not yet an empirical model failure.
- Before promotion, perform a post-identification collapse check: assume the product and protocol identifier are already known, then count the substantive decisions still required in the terminal record.
- Reject a candidate when an indexed protocol identifier plus wording that names the arm, row, statistic, and endpoint leaves only direct transcription.
- Do not count source quantity, binary sibling selection, adjacent numeric values, or absence from search snippets as substitutes for terminal scope difficulty.
- A correct final answer retires the tested architecture regardless of elapsed time.
- A wrong answer counts only after the historical source chain, protocol mapping, table column, statistic, and gold value are reverified.
