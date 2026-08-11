# Art training log

## 2026-08-03 - artist, provenance, and cross-page pigment table

### Prior evidence used

- The strongest Science result reached the correct database record but selected a nearby row. That mechanism is more diagnostic than merely hiding an obscure fact.
- The repaired Science wording also showed that exact noun repetition is necessary when several records, studies, and fields appear in one prompt.
- The Art search therefore targeted a stable catalogue with near-identical neighbouring objects and a layout-dependent terminal lookup.

### Research decisions

1. Used an official museum teaching packet to identify an artist through training and technique, without naming the artist in the prompt.
2. Used a second museum's provenance record to select one oil-on-panel study from the identified artist's works.
3. Used a fixed 2003 conservation survey from a third museum to obtain one directly printed pigment name.
4. Verified the biographical page and both decisive technical-table pages visually.
5. Confirmed that the pigment table begins with artwork titles and early pigment columns on one page, then continues with later columns on the next page without repeating the artwork titles.
6. Confirmed that two adjacent studies have titles differing by one word and different entries in the requested pigment column. The neighbouring entry is therefore a plausible, source-grounded wrong answer.
7. Ran shortcut searches using the provenance names, date, object title, catalogue context, and pigment terminology. Search results did not directly align the selected object with the terminal value.
8. Rewrote the 119-word candidate without `it` or `its`; every clause explicitly names the artist, target study, provenance, or technical survey.

### Current status

One Art candidate passed the domain, atomicity, stability, source-independence, object-identity, provenance, visual-verification, cross-page alignment, shortcut, and grammatical-attachment gates. The exact prompt, gold answer, URLs, title, object identifier, row positions, and neighbouring wrong answer remain in ignored local notes.

The difficulty hypothesis is not obscurity alone. A solver must identify the artist, use provenance to select the exact study, preserve that study's row position across a page break, and avoid taking the black-pigment value from the almost identically titled adjacent study.

No target-model test or platform submission was performed by the agent. The candidate is ready for one fresh user-run GPT-5.5 extended-thinking test, but it is not claimed to be empirically difficult until the final answer is known.

### Reusable lessons

- Museum technical bulletins can create strong Art tasks when layout, object identity, and conservation vocabulary all matter.
- A page break is legitimate difficulty only when the row order can be verified unambiguously from the printed table.
- Near-identical titles create a useful wrong-answer mechanism, but object number and provenance must make the intended work unique.
- Search snippets that expose row labels and values as separate lists do not establish the answer; alignment must be checked in the source.
- Do not disclose the target title, catalogue number, table row, page number, or pigment family in a prompt when upstream clues are meant to select them.

## 2026-08-03 - user-run target solved the candidate

### Outcome

The user reported that the required extended-thinking target model returned the verified pigment name correctly. The candidate is retired. Research time and the presence of a plausible neighbouring-row answer do not count as a failure when the final answer is correct.

### Why the difficulty mechanism was insufficient

- Once the provenance chain selected the object, the terminal task reduced to preserving one row across a page break.
- The model kept the row alignment despite the nearly identical adjacent title.
- Artist identification and provenance increased retrieval cost, but they did not leave enough independent decisions after the technical bulletin was found.
- The nearby pigment was a credible distractor, yet the source layout made the correct row recoverable without resolving another schema, edition, or record-scope distinction.

### Reusable correction

Do not promote a cross-page table candidate merely because the row labels disappear on the continuation page. Require at least one additional post-identification decision—such as an edition crosswalk, object-status change, revised catalogue field, or independently selected analytical method—that controls the terminal cell. Retire every candidate answered correctly by the target model, regardless of elapsed time.

## 2026-08-11 - exact-accession pigment-row candidate retired

### Manual result

The user-run target model returned the verified pigment in 45 seconds. It found the combined accession-range row, separated the pigment abbreviation from the analytical-method letters, and expanded the abbreviation correctly. The candidate is retired as solved.

### Why the candidate was weak

- The exact accession range was supplied in the prompt, functioning as a terminal row identifier rather than an upstream clue.
- The artist, source family, combined-row behavior, and requested `Other` column were also stated explicitly.
- Once the study was opened, the solver needed only one row lookup and one abbreviation-key lookup within the same appendix.
- The winter-scroll and blue-pigment facts became decorative after the accession range had already fixed the row.
- Method letters following the pigment abbreviation looked confusable, but the appendix legend resolved them directly.

### Reusable correction

Do not expose a museum accession number when that number is searchable inside the terminal technical table. An accession clue is useful only when it must first be derived from a separate catalogue record and when another substantive choice remains after the accession is known. Reject `exact accession -> named column -> local legend` designs before testing.
