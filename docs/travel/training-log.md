# Travel training log

## 2026-08-02 — Baseline reconstruction

### Evidence reviewed

- the local workspace and its prior research artifacts;
- a saved collection of strong and weak multi-source prompts;
- existing Travel target-model sessions;
- automated-review feedback from related prompt work;
- locally saved instruction screenshots.

Platform-specific wording, copied submissions, account data, and exact prompt candidates were retained only in ignored local notes.

### Findings

1. The strongest prior designs began with the final obscure fact and worked backward.
2. The Travel attempts began with a destination and tried to manufacture difficulty through extra clues, a calculation, or a visit budget.
3. A heritage-rail timetable answer was fully indexed and therefore easy despite using several sources.
4. An elevation-profile candidate had a fragile decimal answer, too few genuinely distinct sources, and an arithmetic dependency.
5. Dam-cost candidates were short, volatile, subjective, and non-atomic; adding another adjective improved entity identification but did not repair answer ambiguity.
6. Automated review also rejects scripted named-source lookup chains, arithmetic, ambiguous pronouns, incorrect gold answers, and malformed research trajectories.

### Method change

- Adopted answer-first construction.
- Added deterministic review gates before target-model testing.
- Separated prompt validity from model difficulty.
- Added a public/private documentation boundary to protect confidentiality and originality.
- Created two Travel candidate architectures; exact candidates remain local and untested.

### Next feedback loop

When the user tests a candidate in the required target model, record:

- exact prompt version;
- model and reasoning mode;
- final answer and whether it is meaningfully wrong;
- sources the model used or missed;
- automated-review messages;
- whether the cause was model retrieval, prompt ambiguity, or incorrect ground truth;
- the smallest design change supported by that evidence.

## 2026-08-03 — live rule and all-domain audit

### What changed

- Read the complete prompt/review workflow and the domain-strategy material for every listed domain in a signed-in, read-only session.
- Confirmed that source independence is stricter than raw URL count: repeated pages from the same host can fail the architecture gate.
- Confirmed that valid hardness comes from in-domain chaining, exact scope, contextual table reading, confusable names, or bounded enumeration—not arithmetic or ambiguity.
- Added a cross-domain method, domain strategy map, rejection taxonomy, and evidence-driven training loop under `docs/general/`.
- Retired the two local untested Travel candidates because their several URLs resolve to only two hostnames. No model test was run.

### Travel consequence

The next Travel candidate must be mined across at least three genuinely independent publication ecosystems from the start. Adding another page from the same district or agency site is not a repair. Prefer stable brochures, heritage or nomination dossiers, historical guidebooks, management plans, transport publications, and infrastructure records with directly readable text.

### Confidentiality

Exact platform language, account context, candidate prompts, URLs, reviewer-specific material, and private screenshots remain outside version control. Public files contain only generalized methods.

## 2026-08-03 — first manual batch failed the difficulty gate

### Test signal

The user manually tested four new Travel candidates with the required extended-reasoning target model. The model returned every verified answer correctly, each within roughly one to two minutes. The entire batch was retired; no platform submission was made.

### Why the batch was easy

1. The designs began with recognizable destinations and routes, then added source links and ordering constraints forward.
2. Terminal facts appeared on short, indexed HTML lists or clear tables rather than buried contextual records.
3. Two prompts reduced to choosing the next entry from a short list; two reduced to sorting or filtering mileposts.
4. The prompts exposed nearly the complete lookup path, lowering discovery cost.
5. Nearby names and opposite-direction entries looked like distractors to a human but were trivial once the model read the supplied numbers and categories.
6. Passing word-count, atomic-answer, domain, and independent-host checks was incorrectly treated as evidence of target-model difficulty.

### Process correction

- Add a shortcut audit before describing any candidate as ready.
- Reject a candidate if snippets or one obvious query expose the terminal row.
- Reject simple ordering or category filtering over a short list as the sole failure mechanism.
- Require a poorly indexed final record whose answer depends on contextual reading inside a precisely scoped subgroup.
- Keep validity, source architecture, and empirical difficulty as separate promotion decisions.

## 2026-08-03 — archival rebuild after the failed batch

### Research correction

- Removed verification URLs from the prompt body. Sources are supplied separately during verification; embedding them in the question gives the target model a scripted retrieval path.
- Mined terminal facts in a dated historical travel handbook and visually checked the printed pages rather than trusting OCR or search snippets.
- Built backward through three independent publication ecosystems: a national or international travel record, a regional tourism source, and the archival terminal source.
- Added edition and historical-spelling constraints only where they disambiguate the cited record.
- Searched for shortcut queries and competing historical publications before promotion. A useful trap is a plausible answer from the wrong edition or publication, not a nearby number that simple sorting eliminates.

### Current status

Three new Travel candidates passed deterministic preflight and remain untested. Exact prompts, answers, URLs, page references, and audits are kept only in ignored local notes. No target-model query or platform submission was made by the agent.

## 2026-08-03 - archival batch also failed the difficulty gate

### Manual result

The user manually tested all three archival-handbook candidates in the required extended-reasoning target model. Every answer was correct, so the complete batch was retired. One response omitted an adjective but fully satisfied the prompt's request for a building type; evaluation must follow the requested semantic granularity rather than a longer stored phrase.

### Why the apparent obscurity did not help

1. Every terminal fact came from the same famous historical handbook.
2. Each prompt named the year, edition, and record type, turning the last hop into a targeted lookup.
3. Historical spelling and imperfect OCR slowed retrieval but did not create a hard selection problem.
4. The nearby passages were not credible alternatives once the exact record was found.
5. A batch can therefore fail through source-family repetition even when each individual prompt uses several independent websites.

### Research correction

- Retire an architecture after repeated correct answers instead of making cosmetic clue changes.
- Audit alternate copies and extracted search snippets, not just the preferred source URL.
- Prefer image-dominant primary records whose answer depends on a map edge, schedule column, or final table cell.
- Visually verify every relevant row, column, label, and header before storing a gold answer.
- Preserve a strong wrong-cell candidate, such as a current distance beside a historical fare, while keeping the requested output unambiguous.

### Current status

A replacement set using three different visual-selection mechanisms has been verified and retained only in ignored local notes. Its prompts, answers, URLs, and page coordinates are not committed. The set remains untested by the target model, and no platform form was submitted.
