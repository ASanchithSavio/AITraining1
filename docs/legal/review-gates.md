# Legal prompt review gates

Use these gates in addition to the general method. They are designed for completed legal records, not requests for legal advice or statements of current law.

## Domain and stability

- The source graph remains native to Legal: judgments, parliamentary legal records, commission reports, statutes, regulations, orders, or administrative adjudications.
- The question asks what a dated record says, not what the law currently requires.
- Every case, sitting, report, order, and correction is identified by a fixed date or stable identifier.
- The final answer is a directly printed name, title, term, section, or table entry rather than a legal conclusion.

## Record identity

- An upstream judgment or order supplies a real key used to locate the later report or proceeding.
- A separate official index, laying record, docket, or publication page confirms the exact document and version.
- Similar case names, report numbers, annexures, and amended versions have been checked and eliminated.
- The prompt does not disclose a distinctive terminal phrase that collapses the chain into one search.

## Corrections and errata

- Both the original document and the correction are opened.
- The correction's page, annexure, serial number, and column number all match the prompt.
- The direction of change is explicit: the value in the **for** column is the old text and the value in the **read** column is the replacement.
- Adjacent correction rows and nearby entries in the original table are recorded as distractors.
- If a corrected cell contains more than one entity type, the wording asks for a type that selects exactly one of them.
- A merely typographical or apparently erroneous correction is rejected unless the prompt clearly asks for text exactly as printed and the result remains fair.
- Reject a one-page errata or corrigendum task when the prompt names the correction and gives its exact row and column. Image-only access does not repair this collapse.

## Source quality

- At least three necessary records are available through stable, direct URLs.
- The source ecosystems are independent where practical, such as a court, legislature, and issuing commission.
- Long PDFs have exact physical and printed page references.
- Image-only evidence is used only when the direct official image is sharp, bounded, and manually reproducible; its lack of selectable text is logged as a review risk.
- Search snippets are used for discovery only and do not substitute for the controlling document.

## Answer and difficulty

- The answer is atomic and its requested type is explicit.
- The strongest wrong answers come from the original version, an adjacent errata row, or a different entity type in the correct cell.
- Difficulty depends on record identity, version selection, and exact table scope rather than current-law knowledge.
- A target-model run counts as a failure only after it returns a meaningfully wrong final answer or explicitly terminates without one.
- After the controlling record is identified, require at least two meaningful selection or handoff decisions before the answer can be transcribed. Opening a named correction and reading a supplied coordinate is only one lookup.
- Do not use an answer-type instruction as the only discriminator when a terminal cell contains just one phrase of that type.
- Each upstream judgment, laying record, docket, or index must affect the terminal version or scope. A chain that only establishes the title of a directly linked report is evidentially sound but may still be easy.
- Retire a candidate answered correctly in a clean target-model run when the remaining path was deterministic; do not add extra upstream clues or cosmetic obscurity.
