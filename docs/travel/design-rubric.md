# Answer-first Travel design rubric

## Step 1: Mine final facts

Search authoritative travel material for facts that are stable, specific, and poorly indexed:

- accommodation or rest-house tables;
- historic railway and visitor guides;
- protected-area visitor-facility lists;
- nomination dossiers and management plans;
- route, trail, or station tables;
- old tourism directories and gazetteer travel chapters.

Record the exact source location and two neighbouring rows before doing anything else.

## Step 2: Test the answer locally

Ask:

- Is it printed, rather than calculated?
- Can two reviewers read the same value?
- Is there a nearby row that a model could plausibly confuse with it?
- Is the answer too famous or exposed in search snippets?
- Is the source readable without relying on broken OCR?

If any answer is unfavourable, choose another fact.

## Step 3: Build backward

Create a source graph, not a pile of clues:

```text
visitor clue -> destination/district
second travel source -> specific route, sanctuary, station, or lodging
archival list -> scoped row or sequence
final source -> one printed answer
```

Every arrow must narrow the candidate set. Remove any source whose output is not used by the next hop.

## Step 4: Choose a fair failure mechanism

Best mechanisms:

1. Adjacent-row selection inside a named group.
2. Two similarly named places joined by an explicit official bridge.
3. Old/new spelling variants with a source that proves identity.
4. A direction or subgroup constraint that rules out a tempting popular answer.
5. A final cell surrounded by plausible distractors.

Unsafe mechanisms:

- vague superlatives;
- subjective ratings or “complete” itineraries;
- live prices and schedules;
- arithmetic across several cells;
- illegible scans;
- a hidden assumption about whether optional activities count.

## Step 5: Write the natural question

State the clues in neutral prose and end in one question. Avoid imperative chains such as “open this report, take this number, then search that table.” Source names may be necessary for attribution, but the wording should not pre-assign every research step.

## Step 6: Preflight before testing

Validate word window, domain, source necessity, atomic answer, lack of arithmetic, grammar, source stability, and exact answer proof. Only then is a target-model test worth its cost.
