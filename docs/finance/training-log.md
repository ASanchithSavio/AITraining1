# Business & Finance training log

## 2026-08-03 - acquisition, legal-entity, quarter, and Call Report coordinate

### Prior evidence used

- The strongest Science outcome combined wrong-record risk with a separate row-and-column decision.
- The retired Art candidate showed that a page break and neighbouring row alone may slow a model without producing a wrong final answer.
- The Finance search therefore targeted a transaction with sibling entities sharing a brand, a closing between quarter-ends, and a regulatory schedule containing adjacent amount and count columns.

### Research decisions

1. Rejected ordinary annual-report restatements because exact values appeared in search snippets or one filing contained the complete answer path.
2. Rejected failed-bank bid summaries whose terminal values were plainly indexed.
3. Selected a completed bank acquisition whose regulatory approval distinguishes a commercial bank, a savings association, and a fiduciary-service company with closely related names.
4. Used an independent closing filing to place the legal closing between two quarterly reporting dates.
5. Verified that the target institution, a similarly named savings association, and a later similarly named national bank have separate regulator identifiers and different historical rows.
6. Verified the decisive schedule visually: one item spans managed assets, non-managed assets, managed-account count, and non-managed-account count.
7. Verified the requested mnemonic in the Federal Reserve data dictionary and the directly reported value in the FDIC institution-level data.
8. Audited the sibling entity, the next quarter, and the three adjacent columns. Each produces a distinct, source-grounded wrong answer.
9. Removed the friendly field name after finding an indexed banking ranking page for that phrase. The final wording uses the official schedule coordinate, while the coordinate's meaning remains independently verifiable.
10. Ran exact searches combining the regulator identifier, report date, mnemonic, and proposed answer; no result joined the intended entity, period, and value.

### Current status

One 95-word Business & Finance candidate passed the domain, atomicity, stability, independent-source, legal-entity, event-date, reporting-period, field-coordinate, unit, directly-printed-answer, shortcut, and grammatical-attachment gates. The exact prompt, answer, URLs, institution identifiers, adjacent-period values, and wrong-entity values remain in ignored local notes.

The difficulty hypothesis has three independent failure points after the acquisition is recognized: choose the commercial-bank subsidiary instead of two related institutions, choose the quarter immediately before the legal closing instead of the quarter after it, and choose the managed-asset amount rather than the neighbouring non-managed amount or account counts.

No target-model prompt was tested and no platform form was submitted by the agent. The candidate is ready for one fresh user-run GPT-5.5 extended-thinking test. It is not claimed to be empirically difficult until the final target answer is known.

### Reusable lessons

- Brand-name matching is unsafe in banking research; legal entity and regulator identifier must travel together.
- Approval date and closing date serve different purposes. Only the date named by the prompt should choose the reporting period.
- Historical names must be checked at the report date, not inferred from the institution's current name.
- A form coordinate can reduce search leakage without becoming arbitrary when an authoritative data dictionary defines the coordinate.
- Amount columns and account-count columns are separate semantic types even when they sit on the same schedule row.
- Search the friendly label before finalizing. Third-party ranking pages may expose fields that look obscure inside a regulator API.
