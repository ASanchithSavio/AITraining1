# Candidate architectures for Travel

Exact unsubmitted prompts, answers, and URLs are intentionally kept out of the public repository.

## Architecture A: historical accommodation sequence

```text
official attraction page
  -> identifies the district
second official visitor page
  -> identifies a pilgrimage or nature destination inside it
archival travel-facility table
  -> locate the destination's precisely scoped tahsil/group
  -> resolve a duplicate or ditto row
  -> answer with the next lodging name exactly as printed
```

Why it may work: the answer is a stable table entry, the difficulty is row alignment, and every fact remains in Travel.

Primary risk: the first two sources may be judged redundant if either page independently names both the district and destination. Strengthen the handoff before testing.

## Architecture B: archival-to-current directory handoff

```text
official destination clues
  -> district and town
archival accommodation list
  -> identifies an intermediate facility via adjacency
current official lodging directory
  -> uses a repeated attribute to select a neighbouring facility
```

Why it is harder: it contains two independent row-selection operations.

Primary risk: current directory order and contact details can change. Prefer a dated archived directory or a permanent publication before promotion.

## Promotion rule

A candidate moves from backlog to “ready for user test” only after:

- the final record is visually verified;
- all source handoffs are necessary;
- the exact wording passes deterministic review;
- volatility and originality risks are cleared;
- no external model test has been run during research-only mode.
