# Politics prompt review gates

Use these gates in addition to the general method. Exact candidates and source URLs remain in ignored local notes.

## 1. Completed-event gate

- Prefer completed elections, historical tenures, closed hearings, dated debates, archived filings, and final boundary orders.
- Reject current officeholders, live campaign claims, pending litigation, current polling, and facts that can change with the news cycle.
- If a later correction or amendment matters, state the date or version boundary that selects it.

## 2. Identity and chronology gate

- Every spelling variant, predecessor-successor link, constituency, office, and date must be supported directly.
- A date should control the next lookup rather than decorate the prompt.
- Distinguish election day, certification, swearing-in, filing receipt, publication, and effective dates; they are not interchangeable.

## 3. Versioned-record gate

- Verify the complete sequence of filings, amendments, reports, or orders around the chosen boundary.
- Inspect both the selected record and the nearest earlier or later record.
- Store the exact changed field and a plausible value from the wrong version.
- Reject the candidate if the current overview exposes the historical answer or if the version boundary is ambiguous.

## 4. Source-architecture gate

- Use at least three independent political publication ecosystems.
- Each source must contribute an identity, date, jurisdiction, version, or scope value consumed by the next hop.
- Do not count several confirmation pages for one politician as independent difficulty.
- Avoid copying the identity-to-debate or election-to-delimitation structure of prior successful examples.

## 5. Terminal-answer gate

- Ask for one name, number, date, place, office, label, or short printed phrase.
- Do not require vote-total arithmetic, partisan interpretation, legal judgment, or policy evaluation.
- Visually inspect forms, roll calls, tables, and scans; confirm selectable text or reliable OCR also supports the answer.

## 6. Shortcut and wrong-answer gate

- Search the exact candidate, document type, date, and proposed answer together.
- Check current profiles, later amendments, mirrors, data exports, snippets, and third-party summaries.
- A plausible wrong answer should be valid in a nearby version or scope, not an unrelated famous fact.
- Reject simple metadata lookups and terminal values already reproduced in snippets.

## 7. Retired-architecture gate

- Reject the sequence `small officeholder set -> roll-call intersection -> minimum/maximum over a few geographic rows -> directory or address-field transcription`.
- Changing the politicians, jurisdiction, legislation, election year, directory edition, or requested contact field is a surface variation, not a new architecture.
- Treat a geographic crosswalk as decorative when it merely maps the already selected jurisdiction to one obvious office row.
- Reject a candidate when the resolved identity and jurisdiction leave a single directly printed field in an explicitly named terminal directory, even if every upstream source is technically necessary.
- A successor to this pattern must retain at least two live, source-backed terminal alternatives after identity resolution and use a genuinely different mechanism, such as a controlling correction, disputed version boundary, sequence reconciliation, or consequential footnote.
- Compare every proposed Politics candidate's source-family sequence and final two selection operations with the ignored retirement records before delivery. A near-match is not returned for testing.

## 8. Empirical gate

- A candidate that passes these checks is only ready for a manual test; it is not proven difficult.
- If the target model retrieves the correct historical versions and answers correctly, retire the candidate rather than adding decorative political clues.
- Record a correct result as a model success and prompt-design failure; elapsed time never changes that classification.
