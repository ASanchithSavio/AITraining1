# Delivery checklist

Use this checklist before returning a prompt, confirming an answer, diagnosing a model failure, or preparing a golden trajectory, golden rules, and verification sources. It is a required reload, not a substitute for the active-domain pack.

## Reload context first

1. Read the repository README and every file in its general read order.
2. Read the complete active-domain review gates and training log.
3. Read the ignored local candidate file and current-status index when they exist.
4. Locate the exact candidate version, verified gold answer, manual outcome, reviewer feedback, and latest repair.
5. Do not rely on chat memory when the repository contains a newer record.

If the ignored local notes are unavailable, say that exact candidate context is missing before reconstructing or changing anything.

## Freeze prompt and answer separately

- Treat `prompt_frozen` and `gold_frozen` as independent controls.
- When the user says the prompt and answer must remain the same, change only the trajectory, rules, source selection, or page locators.
- Do not silently polish a tested prompt. Even a grammatical edit creates a new version that needs a new preflight and test.
- A source-format repair does not invalidate a verified answer unless the replacement evidence contradicts it.
- Record every changed component and every deliberately unchanged component.

## When delivering a prompt

- Return only the requested prompt unless the user asks for supporting material.
- Use one natural, self-contained question with an atomic answer instruction.
- Re-run the active-domain gates, shortcut audit, source-necessity check, and grammatical-attachment check on the exact final wording.
- Keep URLs, internal identifiers, answer keys, and research instructions out of the prompt unless the task itself requires them.
- Do not run the target model when testing is reserved for the user.

## When confirming an answer

- Reopen the terminal source and verify the exact row, column, chart box, field, unit, and version.
- Compare the proposed answer with the recorded parent, sibling, adjacent row, neighbouring period, and similarly named entity values.
- Distinguish an equivalent formatting variant from a genuinely different answer.
- Give the verified answer directly and state uncertainty only when the source itself leaves uncertainty.

## When writing a failure reason

Use the smallest causal claim supported by evidence:

1. **Observed:** record the model's exact returned answer and the terminal result.
2. **Verified:** reconfirm the gold answer and the decisive source location.
3. **First divergence:** identify the earliest error proven by the returned value or reasoning trace.
4. **Limit:** state what cannot be inferred without the model's trace.
5. **Training change:** record the reusable architecture, wording, or review-gate lesson.

Do not infer an internal browsing path merely because a wrong answer resembles a nearby source value. Describe the proved scope, entity, row, column, or hierarchy error.

## When writing the golden package

Keep these sections separate and in this order:

1. `Golden trajectory`
2. `Golden rules`
3. `Verification sources`

If the user also asks why the tested response failed, deliver four separate sections in this order:

1. `Response failure reason`
2. `Golden trajectory`
3. `Golden rules`
4. `Verification sources`

A correct answer correction or a compact diagnosis does not satisfy a request for the complete package. Before sending, compare the response headings with every component the user requested and confirm that none was omitted.

For the trajectory:

- use `Search`, `Fetch`, `Verify`, and `Filter` only when those actions are real;
- make every search depend only on prompt facts or a fact established earlier;
- give the direct URL in every fetch step;
- include the exact section, physical PDF page, printed page, image number, row, column, or chart box;
- explain how each verified fact supplies the next lookup key or excludes a live alternative; and
- finish with a comparison of the correct target and the plausible confusers.

For the golden rules:

- write concise instructions that prevent the observed entity, hierarchy, scope, row, column, date, or unit mistake;
- repeat exact entity labels when pronouns could be ambiguous;
- state whether calculation is required; and
- state the exact required output format.

For the verification-source list:

- keep a one-to-one mapping with trajectory claims;
- use raw direct URLs when the submission form expects unrendered URLs;
- state each source's exact location, purpose, and necessary fact;
- classify the actual response as human-readable HTML or PDF before submission;
- do not cite JSON or YAML in this workflow;
- validate extensionless archive assets from catalogue metadata, file signature, and rendered content; and
- count a catalogue page and its original asset as one publication ecosystem.

## After manual or platform feedback

1. Preserve the exact prompt version and returned answer in ignored local notes.
2. Separate prompt validity, model difficulty, source format, and reviewer compliance.
3. Apply the smallest repair to the failed layer.
4. Update the active-domain private record with exact details.
5. Promote only generalized, non-confidential lessons to the public domain pack.
6. Commit and push only the public-safe files requested by the user.

Treat a missing requested section as a delivery failure even when the underlying research and diagnosis are correct. Log and repair that presentation layer separately; do not redesign the prompt or change a verified answer merely because the package was incomplete.

Elapsed research time and intermediate status are not terminal outcomes. A correct final answer retires the tested architecture; a wrong answer counts only after the prompt and gold answer survive re-verification.
