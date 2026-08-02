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
