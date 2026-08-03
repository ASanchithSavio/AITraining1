# Domain selection and pivot rule

Domain choice is an empirical decision, not a judgment that one subject is inherently easy or hard. A valid domain should be paused when several genuinely different prompt architectures are repeatedly solved and another domain has stronger observed failure mechanisms.

## Evidence threshold

Evaluate a domain on four separate questions:

1. **Validity:** Can the answer be stable, atomic, and directly verified?
2. **Source depth:** Does the domain contain long, authoritative records with meaningful internal structure?
3. **Shortcut resistance:** Can the terminal fact survive search snippets, alternate copies, and direct phrase queries?
4. **Empirical difficulty:** Has the required model actually failed for the intended reason?

The fourth question outranks aesthetic impressions such as an old scan, a dense map, unfamiliar spelling, or a long prompt.

## Current Travel finding

Travel remains a valid seeded domain, but the current research program has reached a pause condition. Ten manually tested candidates were all solved across three batches:

- four candidates using indexed lists, adjacency, direction, or milepost filtering;
- three candidates ending in a dated historical handbook; and
- three candidates ending in an image-only timetable, a route-map edge, or a multi-column historical directory.

This range rules out a single bad website or a single weak wording pattern as the complete explanation. The model handled source discovery, OCR alternatives, visual inspection, map tracing, and row/column alignment. Another destination-to-record chain is therefore unlikely to improve yield merely by using a rarer place or a noisier scan.

Travel should be resumed only when the terminal mechanism is structurally new, such as a corrigendum that changes a table's meaning, a version crosswalk between independent records, or a footnote that reverses the apparent row selection. Do not resume it with another famous-place identification followed by one bounded lookup.

## Evidence-based domain order

This is a working ranking based on the local test history, not a permanent quality score.

| Priority | Domain | Positive signal | Best next mechanism | Main risk |
|---:|---|---|---|---|
| 1 | Politics | Two prior, independently reviewed examples produced meaningful wrong answers through historical official records. | Historical identity handoff into an election, delimitation, hearing, or debate record; require exact sequence, tenure, or scoped transcript reading. | Current-office drift, partisan claims, and heavily indexed federal metadata. Use completed historical events. |
| 2 | Science & Technology | A prior successful technical-table design showed that wrong-column and wrong-calibration selection can survive deep reasoning. | Cross-version report joins, appendix/table scope, test-condition selection, renamed fields, or a footnote-controlled value. | Accidental calculation, report-version ambiguity, unreadable figures, and snippets that reproduce whole tables. |
| 3 | History | Strong local evidence overlaps with Politics and technical reports, especially for rosters, proceedings, gazetteers, and dated tables. | Entity bridge followed by a bounded roster, sequence, or technical archival table. | OCR errors, namesakes, and unbounded newspaper searching. |
| 4 | Music | Catalogs, matrix ledgers, programs, and scores offer precise identifiers and edition/take distinctions. | Join a performance program to a catalog or matrix record where edition, take, arranger, or instrumentation controls the answer. | Release-version ambiguity, directly indexed catalog pages, weak source independence, lyrics, and notation-only evidence. |
| Pause | Travel | Ten correct responses across multiple source and selection mechanisms. | Resume only for a genuinely new version/corrigendum/footnote architecture. | Familiar destination funnels and bounded extraction remain easy even when the final record is visual. |

## Next-domain guardrails

### Politics

- Use historical, completed events and official records.
- Make identity, constituency, tenure, or sequence constraints necessary rather than decorative.
- Prefer state or local delimitation records, older debates, and archival proceedings over a simple federal witness lookup.
- Reject any candidate answerable from a current biography, headline, or metadata page.

### Science & Technology

- Select the terminal cell first and verify its row, column, unit, version, and footnotes visually.
- Ask for one printed value or phrase; do not require the solver to calculate it.
- Look for old/new field names, several calibration or test columns, revised appendices, and tables whose headers span pages.
- Search exact row fragments before promotion because technical tables are often extracted into snippets.

### Music

- Treat it as a controlled exploratory batch, not the first pivot.
- Fix the work, performance date, edition, issue, matrix, take, and catalog scope wherever needed for uniqueness.
- Prefer institutional archives and primary programs over fan discographies.
- Reject questions whose answer changes by release, remaster, reissue, arrangement, or regional catalog without an explicit discriminator.

## Pivot rule

Pause a domain when all of the following are true:

1. at least two distinct terminal-source families have been tested;
2. at least three distinct selection mechanisms have been tested;
3. every candidate in two consecutive batches is answered correctly; and
4. the proposed repair is only more obscurity, more clues, or a noisier scan.

After a pivot, build a small batch around one mechanism already supported by local failure evidence. Do not transfer the surface form of the failed domain into the new one.
