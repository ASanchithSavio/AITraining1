# Business prompt review gates

Use these gates with the general method. Exact company names, subsidiary names, answers, URLs, and manual test outcomes remain in ignored local notes.

## Domain and answer

- Keep the task native to corporate history, operations, ownership, distribution, manufacturing, acquisitions, or organization structure.
- Ask for one directly printed name, percentage, year, facility function, product, or other atomic historical fact.
- Prefer completed historical events and fixed publications. Reject current ownership, live rankings, market prices, forecasts, and derived financial arithmetic.
- Treat Business and Finance as separate domains: an ownership or operating-structure task is Business even when the source is a corporate report.

## Answer-first archival design

- Mine the terminal fact before writing any clues. Record the exact publication date, page, chart branch, row, and neighbouring entries.
- Prefer old booklets, directories, enforcement reports, and organization charts whose decisive fact is readable but poorly indexed.
- Use obscurity only as the discovery layer. The terminal fact must remain plainly visible once the correct document and entry are selected.
- Reject a candidate if identifying the company collapses the task into a single obvious lookup with no later decision.

## Reverse source graph

- Build backward from the terminal entry. One source can identify the issuing corporation, a second independent source can select a subsidiary or facility, and the archival document can supply the answer.
- Every source must contribute a lookup key consumed by the next step. Remove biographical or historical clues that merely reconfirm an entity already selected.
- Count independent hosts, not URLs. Where three sources are required, use three genuinely separate publication ecosystems.
- Keep at least two meaningful decisions after the broad industry or famous brand is recognized.

## Corporate hierarchy and chart alignment

- Distinguish parent, controlled company, subsidiary, division, plant, and successor. A shared brand or place name is not an identity bridge.
- Prefer a same-type confuser: two subsidiaries, facilities, products, or percentages printed close together in the same dated record.
- Visually inspect relationship lines, indentation, braces, legends, percentages, and dates. OCR order is not proof of chart alignment.
- Record the neighbouring entry and its value before testing; a useful wrong answer must belong to a real confusable entry.

## Version, scope, and shortcut checks

- Fix the exact month and year of the booklet, not merely the company name. Historical ownership is not current ownership.
- State whether the requested value comes from a chart, table, note, or prose when the same publication reports rounded and unrounded variants.
- Search combinations of the issuer, target entry, document date, terminal label, and proposed answer. Reject any candidate whose intended entity-value pair is exposed by a snippet.
- Confirm that each source is directly accessible and that a solver can reach the archival document without a private database or login.

## Language and empirical gates

- Repeat `booklet publisher`, `target company`, `chart`, and `percentage` when a pronoun could attach to more than one entity.
- Keep source clues in one natural question; do not turn the prompt into a browsing checklist.
- Passing preflight makes a candidate ready for one user-run target-model test. A correct final answer retires the candidate regardless of elapsed time.
