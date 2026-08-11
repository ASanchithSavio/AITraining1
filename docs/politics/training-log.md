# Politics training log

## 2026-08-03 - first answer-first Politics rebuild

### Prior evidence used

- The strongest local Politics examples produced meaningful wrong answers through a fragile identity or sequence handoff in completed official records.
- Their useful mechanisms were exact historical scope, spelling or tenure bridges, and plausible alternatives inside the correct record.
- The new design must preserve those causal properties without copying a debate-quotation or delimitation-adjacency architecture.

### Research decisions

1. Chose completed campaign-finance filings as a new native Politics source family.
2. Used an official result-certification date as a version boundary rather than a decorative clue.
3. Verified the full sequence of organization statements on both sides of that boundary.
4. Compared the relevant historical form pages visually and textually.
5. Selected a bank name that is added in the post-boundary amendment while a strong biographical association points toward the retained pre-boundary bank.

### Rejections

- Rejected a contested-election committee-report path because search extraction exposed nearly every distinctive count that could serve as an answer.
- Rejected current committee metadata because the overview page and snippets expose it directly.

### Current status

One 84-word candidate passed ground-truth, chronology, atomicity, source-ecosystem, originality, visual-verification, and shortcut checks. Its exact prompt, answer, source links, file numbers, images, and audit remain in ignored local notes. It was not tested or submitted by the agent.

The difficulty hypothesis was a historical version-selection error: the solver had to locate the last organization statement before a state result certification and the first amendment after it, then identify one newly added field value. The later manual result invalidated that hypothesis because the target eventually resolved the version boundary and answered correctly.

### Manual-test result

The user first reported that a fresh target-model session had spent about 25 minutes researching without a final answer. The platform's terminal check arrived several minutes later and rejected the task because the target had answered correctly. The candidate is therefore retired as solved, not promoted as a model failure.

This outcome establishes a stronger timing rule: even roughly half an hour of research is not success. Elapsed time can measure retrieval cost, but only the final answer or terminal platform judgment determines whether a prompt stumped the target.

## 2026-08-03 - additional answer-first mining

Several Politics branches were rejected before drafting a test candidate:

- A historical convention-ballot sequence failed the shortcut audit because an exact query surfaced the delegation and likely sequence.
- A modern roll-call delta collapsed after one participant's own official statement exposed the relevant vote change.
- A historical veto comparison produced a valid set of vote switchers, but the proposed biographical discriminator independently named the intended person. The roll-call comparison therefore became decorative.
- A preferential-election transfer path was not promoted because the accessible result pages did not preserve the complete intermediate distribution needed for a fair, reproducible terminal selection.

The reusable lesson is that a difficult comparison cannot be rescued by a clue that independently identifies its answer. For a future Politics candidate, the person or record should emerge only from the intersection of independently sourced sets, and at least two meaningful decisions should remain after the central event is known.

## 2026-08-05 - roll-call intersection to directory candidate retired

### Manual-test result

The user ran a frozen Politics candidate with the required target model. The model returned the verified answer correctly in 1 minute 32 seconds and accurately described every decisive stage. The candidate is retired as a model success and prompt-design failure; no wrong-answer failure is claimed, and elapsed time does not alter the result.

### Cause

The candidate began with a small bounded set of election winners and used two public roll calls as an identity intersection. That looked multi-source, but after the member was identified the chain collapsed into a minimum over two county rows, a one-to-one county/city mapping, and direct transcription of an office field from a fixed directory. The several sources improved verification without sustaining ambiguity: each remaining hop had one obvious output, and the neighbouring office entries ceased to be live alternatives as soon as the county was known.

### Permanent change

- Retire the complete architecture, not merely its entities or wording.
- Do not return a superficial variant that swaps in different districts, votes, years, jurisdictions, directories, or address fields.
- Do not count an easy geographic crosswalk as a meaningful post-identification decision when it selects a unique directory row.
- Future Politics candidates must leave at least two plausible, source-backed answers alive after identity resolution and resolve them through a new mechanism such as a controlling amendment, correction, sequence, footnote, or genuinely consequential version boundary.
- Compare the final two operations of every new candidate against ignored retirement records before it can be delivered for testing.

## 2026-08-11 - one-page seating-roster candidate retired

### Manual result

The user-run target model identified the intended guest and returned the correct table number in 1 minute 6 seconds. It also distinguished the guest from the two other surname matches. The candidate is retired as solved.

### Why the candidate was weak

- The exact dinner date, honored guest, repository, surname, and target occupation reduced retrieval to one known one-page seating list.
- The biographical clue independently identified the publisher, while the prompt itself classified the other surname matches as the publisher's wife and another named guest.
- After identifying the publisher, the only remaining action was copying the table heading above one clearly printed name.
- The multiple surname entries appeared to create a bounded-identity problem, but their roles were already resolved in the question.
- The clue chain increased prose length without creating a post-identification scope, chronology, or document-version decision.

### Reusable correction

Reject `named event and date -> one-page roster -> explicitly classified surname match` candidates. For a roster task to be difficult, the target identity should emerge from an intersection that is not independently stated in the prompt, and the roster should feed a further evidence decision rather than serve as the terminal transcription page.
