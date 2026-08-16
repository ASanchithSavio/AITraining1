# Geography training log

## 2026-08-04 - planned-city landmark to historical census scope candidate

The candidate starts from a fixed housing-census cell rather than from a famous place. An independent museum record identifies a lumberman through his former mansion, and a historic-register nomination links that founder to a planned city and a named company hotel. The hotel name then selects a full precinct row in the Census.

The terminal page also contains a city-total row and a later line for the portion of the city inside the same precinct. Those are grounded geographic-scope confusers, not arbitrary nearby numbers. High-resolution crops were used to verify the row label and mortgage-status columns. Natural searches did not expose the terminal value.

Exact wording, place names, values, URLs, and page coordinates remain in ignored local notes. The candidate is ready for one fresh user-run target-model test.

## 2026-08-05 - ground-truth correction and retirement

The user-run target returned the value actually printed in the selected historical precinct row. A fresh original-resolution audit showed that the stored gold had one digit transcribed incorrectly. The result is therefore a correct model answer and a failed ground-truth preflight, not a model failure.

The earlier verification relied too heavily on a tight numerical crop. The corrected audit retained the multi-level mortgage-status header, complete row label, adjacent mortgaged count, and the neighboring city and in-precinct rows. Future Geography candidates using dense census scans require two independent visual reads at original resolution before testing.

The candidate is retired. Exact values and place names remain only in ignored local notes.

## 2026-08-11 - taluk headquarters versus temple-village row

### Manual result

The user-run target identified the correct historic district and taluk but returned the female population printed for the taluk headquarters on an earlier census page. The prompt asked for a different village in the same taluk. The official village table gives a different female value in that village's row.

The returned number is therefore not a random hallucination. It is a real value under the same year and sex column, but at the wrong administrative row. The candidate is retained as a meaningful failure.

### First established divergence

The heritage clues establish the temple village and its taluk. The response named that village correctly, so the identity chain succeeded. The first provable error is the terminal census scope: the model substituted the row for the similarly named taluk headquarters for the row of the selected village.

### Reusable lessons

- Historical village tables can sustain a fair confuser when the taluk headquarters and target settlement appear in the same administrative section and share a name stem.
- Record the returned wrong value's exact row, year, and sex column. This proves a scope substitution without speculating about the model's internal search.
- Preserve the full hierarchy through the final lookup: district, taluk, hobli, village, census year, and sex column.
- Do not infer that correct entity prose proves correct table alignment. Recheck the row label beside the returned number.
- A long scan becomes useful difficulty when an independently established subdistrict and village must both remain in scope; page length alone is not difficulty.

## 2026-08-16 - reviewer repair for the village-row failure

The underlying wrong-place substitution remained source-grounded, but the first submitted failure annotation did not explain the contradiction tightly enough. It discussed page order and the model's presumed browsing path instead of stating that the returned population belongs to the taluk headquarters excluded by the question, while the temple village's row prints the gold value. The reviewer therefore rejected the annotation as unsupported and out of scope.

A separate automated check also rejected awkward wording that described the historical census with a machine-like time phrase. The natural repair uses an ordinary dated census description and explicit settlement names. Because that wording changes the prompt, the previous response cannot be attached to the revision; a fresh target run and matching link are required.

### Reusable lessons

- In a place-scope failure reason, name the requested settlement, name the real settlement that owns the returned value, and state the gold value. Leave page navigation to the trajectory.
- Do not claim that the model read a nearby row unless the returned value is actually printed in that row.
- Make an excluded same-name place part of the question's factual scope if the diagnosis depends on that exclusion.
- Prefer normal dated prose such as `the 1901 census` over compressed expressions intended to sound historical.
- Treat an `expected failure reason` written before testing as private only; replace it with the actual observed outcome after the run.
