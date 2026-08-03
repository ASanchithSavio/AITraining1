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
- Do not treat several pages on one host as independent source ecosystems.
- Keep confidential prompt wording, answer keys, task URLs, screenshots, and copied platform text out of the public repository.

## Common defects

- **Decorative source:** Removing a cited page would not change the solution.
- **Unstable discovery:** The proof depends on whichever result happened to rank first.
- **Scope jump:** A source proves a nearby fact, but not the exact date, version, district, edition, or field asked about.
- **Premature uniqueness:** The trajectory names a winner without enumerating or comparing the bounded alternatives.
- **Version blindness:** It opens one record but never proves that it is the correct record immediately before or after the boundary.
- **Verification mismatch:** A URL appears in the source list but no trajectory claim consumes it, or a trajectory claim has no supporting source.
