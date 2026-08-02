# Candidate architectures for Travel

Exact unsubmitted prompts, answers, and URLs are intentionally kept out of the public repository.

## 2026-08-03 architecture correction

Any instantiation of the designs below that uses several URLs but only two web hostnames is **not ready for testing**. Independent pages are not automatically independent source ecosystems. The hostname and necessity of every node must be checked before promotion.

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

Primary risk: the first two sources may be redundant and may share a hostname. Strengthen the handoff with a necessary source from a genuinely separate ecosystem before testing.

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

Primary risk: current directory order and contact details can change, and multiple directory pages may still share a hostname. Prefer a dated permanent publication and verify independent-host coverage before promotion.

## Architecture C: independent-publication chain

```text
stable visitor or heritage publication on host A
  -> identifies a bounded destination or route group
independent management, transport, or institutional publication on host B
  -> supplies a necessary historic name, component, or subgroup
permanent directory, dossier, or guide on host C
  -> requires exact row/section selection
  -> yields one printed Travel answer
```

Why it is stronger: each host contributes a different narrowing fact, the final answer stays inside Travel, and the last hop can use a fair scope or row-selection trap.

Primary risk: the first two sources may still identify the terminal page too directly. Search queries and prompt wording must not leak the final publication.

## Promotion rule

A candidate moves from backlog to “ready for user test” only after:

- the final record is visually verified;
- all source handoffs are necessary;
- the current independent-host requirement is satisfied;
- the exact wording passes deterministic review;
- volatility and originality risks are cleared;
- no external model test has been run during research-only mode.
