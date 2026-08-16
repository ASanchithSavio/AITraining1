# Golden trajectory format

A golden trajectory is a reproducible proof of the answer. It should show how each source changes the search state, not merely list pages that happen to mention related facts.

## Step pattern

Use four labels when all four actions are real:

1. **Search:** Give the stable query used to locate the next authoritative record. Do not rely on a claim such as “clicked the top result,” because rankings change.
2. **Fetch:** Give the direct URL and the exact section, table, filing date, PDF page, image number, paragraph, or line that contains the evidence.
3. **Verify:** State only the fact that the cited location proves.
4. **Filter:** Explain how that fact eliminates alternatives or supplies the lookup key for the next source.

If an earlier record already provides the exact identifier or link needed for the next hop, begin with **Fetch** instead of inventing a redundant search step.

## Reusable skeleton

```text
Step 1 — Search: Search [stable query] to locate [authoritative record family].

Step 2 — Fetch: Open [direct URL]. In [exact location], find [bounded evidence].

Step 3 — Verify: This establishes [one source-backed fact].

Step 4 — Filter: This removes [plausible alternatives] or supplies [next lookup key].

[Repeat only when the next source adds a necessary fact.]

Final comparison — Compare [correctly scoped records or rows]. [Candidate A] fails because [source-backed reason]; [candidate B] uniquely satisfies every constraint.

Final answer: [atomic answer]
```

## Verification-source list

After the trajectory, list the direct sources again when the review form expects a separate verification section. Keep a one-to-one mapping between the claims in the trajectory and the sources in that list. Use raw direct URLs if the form requires unrendered URLs.

For each source, record:

- the direct URL;
- the exact location used;
- the fact it proves; and
- why that fact is necessary to the answer.

## Quality rules

- Every step must either establish a fact or narrow the candidate set.
- Prefer stable identifiers, dates, and direct URLs over search-result order.
- Distinguish a publication, filing, meeting, or certification date from the date of the underlying event.
- State PDF page numbers unambiguously; include both physical page and printed or image number when they differ.
- Compare the full relevant sequence before calling a record the “first,” “last,” “before,” or “after” version.
- Preserve the prompt's exact scope throughout the proof.
- End with the decisive comparison and one atomic answer.
- Do not pad the trajectory with repeated searches, navigation clicks, or generic confirmations.
- Treat the trajectory as a verification path, not a software tutorial. Omit menu paths, spreadsheet-filter clicks, and mechanical interface actions unless one of them is necessary to disambiguate the evidence.
- Prefer one compact Search/Fetch/Verify unit per consumed source. State the resulting identifier, row, or field directly instead of narrating every action used to reveal it.
- Do not treat several pages on one host as independent source ecosystems.
- Keep confidential prompt wording, answer keys, task URLs, screenshots, and copied platform text out of the public repository.

## Common defects

- **Decorative source:** Removing a cited page would not change the solution.
- **Unstable discovery:** The proof depends on whichever result happened to rank first.
- **Scope jump:** A source proves a nearby fact, but not the exact date, version, district, edition, or field asked about.
- **Premature uniqueness:** The trajectory names a winner without enumerating or comparing the bounded alternatives.
- **Version blindness:** It opens one record but never proves that it is the correct record immediately before or after the boundary.
- **Verification mismatch:** A URL appears in the source list but no trajectory claim consumes it, or a trajectory claim has no supporting source.

## Reproducible discovery and fixed-source gate

Apply these checks to the exact trajectory that will be submitted:

- Name the search interface when it matters: `web search`, `site search`, or `catalogue search`. A query that works in a web search engine must not be presented as though it works in an archive's internal search box.
- Quote the exact query and reproduce it in the claimed interface before delivery. Every term in the query must come from the prompt or from a fact established in an earlier step. Do not smuggle in a report number, person, institution, sample code, or answer learned later.
- If the next source is a specialist archive, show the discovery bridge. A neutral web query can locate the archive's collection page; that collection page must then explain why the archive is relevant before its internal catalogue is searched.
- A search-results page is navigation evidence, not verification evidence. Verification sources must open the direct record, document, or fixed page that contains the cited fact.
- Prefer fixed, browser-readable HTML or PDF. Reject JSON, YAML, spreadsheet downloads, live API queries, interactive filtered maps, and huge text exports that require manual filtering or `Ctrl+F` as submitted evidence.
- A parameterized URL is acceptable only when opening it in a fresh session loads one fixed answer-bearing record without asking the reviewer to construct or run a search.
- For HTML, name the section heading, metadata field, bullet, or opening words of the paragraph. For a PDF, give the physical page and printed page when they differ. For a rotated scan or a table at the bottom of a page, also give the table heading, row label, column label, and one adjacent anchor.
- Click-test every submitted URL from the final artifact in a fresh session. After replacing a source, scan the whole trajectory and source list for the obsolete URL; fixing the prose while leaving the old link in the attachment is still a failed repair.
- Count a catalogue record and its downloadable report as one source ecosystem. A metadata page does not create independent corroboration for the PDF it describes.
