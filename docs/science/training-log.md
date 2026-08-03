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
