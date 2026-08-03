# Finance prompt review gates

Use these gates with the general method. Exact entities, filing values, record identifiers, URLs, and manual test outcomes remain in ignored local notes.

## Domain and answer

- Keep the task native to corporate, banking, securities, accounting, regulatory, or transaction research.
- Ask for one directly reported value, name, code, date, or short phrase from a stable filing or regulatory record.
- Fix the reporting entity, legal entity level, report type, period, units, and field coordinate whenever any of them can change the answer.
- Reject valuation opinions, market forecasts, live prices, and answers that require calculating an unprinted figure.

## Entity hierarchy

- Distinguish a parent holding company from every subsidiary bank, savings association, trust company, broker-dealer, and successor institution.
- Use charter location, regulator identifiers, or transaction language to select the legal entity; a shared brand name is not enough.
- Audit renamed institutions and historical names at the requested report date.
- A plausible wrong answer should come from a real sibling, successor, predecessor, or similarly named reporting entity.

## Event and reporting period

- Prove the effective closing time or legal event date from an authoritative transaction record.
- Select the last or first report strictly on the requested side of that event; do not substitute an announcement, approval, certification, or later accounting date.
- Inspect the adjacent reporting periods and record their values as date-scope distractors.
- State whether the report is quarterly, annual, amended, or restated when that status controls the value.

## Form coordinate and terminal data

- Verify schedule, item, column, unit, and regulatory mnemonic independently from the reported value.
- Treat adjacent amount and account-count columns as different fields even when a data API gives them similar short names.
- Use the official form or data dictionary to prove the field meaning and the regulator's institution-level data to prove the value.
- The final answer must be printed in the selected record; code may locate or validate the row but must not derive the answer.

## Source graph and shortcut audit

- Prefer independent sources for transaction identity, effective date, form semantics, and terminal data.
- Every source must eliminate a real alternative. Reject a source that only repeats a fact already sufficient to reach the same record.
- Search the entity name, regulator identifier, report date, field mnemonic, friendly field label, and proposed answer in likely combinations.
- Reject a candidate if an indexed ranking page or snippet directly joins the intended entity, period, and answer.
- A friendly field label can be a shortcut. When appropriate, ask by an official schedule coordinate whose meaning is independently verifiable.

## Language and empirical gates

- Repeat `holding company`, `subsidiary bank`, `savings association`, `report`, and `field` when a pronoun or modifier could attach to more than one entity.
- Separate exclusion instructions from the target selection sentence.
- Passing preflight makes a candidate ready for one user-run target-model test; elapsed time is irrelevant, and a correct final answer retires the candidate.
