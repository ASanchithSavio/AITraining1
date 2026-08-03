# Travel failure patterns

## Observed classes

| Pattern | Why it fails | Repair |
|---|---|---|
| Famous-property funnel | Several clues collapse immediately to a well-known destination, after which the final timetable or station fact is directly indexed. | Start from the obscure final record, then build backward through less-indexed handoffs. |
| Precision calculation | The answer depends on subtracting values read from a scan. OCR and rounding create multiple plausible decimals, and arithmetic may be disallowed. | Ask for one value exactly as printed in a clearly scoped cell. |
| Live visit-cost question | Admission, shuttles, activities, parking, and optional items vary over time and by visitor choice. “Visit fully” and “highly rated” are subjective. | Use a dated official tariff only if the benchmark permits time-bound answers; otherwise choose a stable fact. |
| Ambiguous superlative | Phrases such as “biggest dam” or “constructed without cement” can identify different places depending on the category used. | State a source-backed category and add a discriminator that leaves one entity. |
| Wall-to-wall source map | Naming the exact document for every hop converts research into a scripted lookup and can expose the final page. | Attribute only what is necessary; pose one question and let the solver discover the route. |
| Source-count illusion | Three links all establish the same place, while the answer comes from one unrelated link. | Draw a source graph and require a distinct output from every node. |
| URL-count illusion | Several pages are cited, but they come from only one or two web hosts. | Count independent hostnames during preflight and replace redundant same-host pages with necessary sources from separate ecosystems. |
| Famous-example fingerprint | A chain copies the skeleton, edge case, or source network of a published reference task. | Re-mine the terminal fact and construct an original graph; cosmetic entity swaps are not new architecture. |
| One-off stochastic miss | A candidate fails once but the model reliably solves the same chain in other fresh runs or automated evaluation. | Treat difficulty as a repeatability target; replace the reliably solved hop rather than adding filler. |
| Model-correct “failure” | A complicated prompt feels hard, but the target model returns the verified answer. | Discard it. Complexity without an incorrect final answer is not a failure. |
| Wrong gold answer | The selected row/year/entity was never independently verified, so the model appears wrong while it is correct. | Verify primary-source row alignment before testing. |

## Additional patterns confirmed by manual testing

| Pattern | Why it fails | Repair |
|---|---|---|
| Compliance-hardness conflation | A prompt passes the word, domain, source-host, and atomic-answer checks, so it is promoted without evidence that the target model will struggle. | Treat validity, architecture, and difficulty as separate gates; passing the first two does not predict the third. |
| Short-list ordering | The final operation is merely selecting the next higher or lower value, or the adjacent entry, from a small clean list. | Move the terminal answer into a longer contextual record with a scoped subgroup, duplicate, spelling bridge, or row-alignment trap. |
| Transparent distractor | A nearby name, opposite-direction stop, or category mismatch looks tempting but is eliminated immediately by explicit numbers or labels. | Use a distractor that survives earlier constraints and is ruled out only by careful reading of terminal context. |
| Snippet-exposed terminal fact | Search snippets or one obvious query reveal the relevant row and its neighbour. | Run a shortcut audit and replace the terminal source with a poorly indexed but readable record. |
| URLs embedded in the prompt | Direct links remove source discovery and hand the target model the intended lookup sequence. | Keep verification sources in their separate fields; write a self-contained question without URLs. |
| Wrong-publication near match | Historical sources about the same route can give different instructions, spellings, or values, so an undated clue permits multiple defensible answers. | Name the exact edition or publication needed for uniqueness and verify that a competing source supplies only a distractor. |

## Why earlier successful designs were different

The useful pattern was answer-first construction:

1. Select a stable, obscure, directly printed answer.
2. Confirm the exact row or passage.
3. Work backward through several authoritative sources.
4. Use sequence, scope, or spelling handoffs that can produce a plausible wrong answer.
5. Keep the requested output atomic.

The failed Travel designs generally began with a popular place and tried to add difficulty afterward. That produces longer prompts, not harder retrieval. Multiple pages from the same official destination site do not repair the architecture.

A stronger Travel design can use publication confusion fairly: the prompt identifies one dated edition, while another searchable historical guide contains a plausible but incorrect near match. The challenge then becomes accurate source selection and contextual reading rather than arithmetic or ambiguity.
