# Representation Science: adequacy depends on the question

**Evidence:** implemented experiment; bounded computational reproduction.  
**Scope:** EXP-001's exposed, deterministic mathematical case.  
**Canonical source:** [results and interpretation](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-001-results-2026-10-03.md).

## Problem

A compact representation may answer one question and fail another. But failure can have several causes: omitted information, a restricted decoder, insufficient computation, or a missing certificate. Treating those causes as equivalent can produce a false claim about what the representation has lost.

EXP-001 makes these distinctions concrete by varying the requested output and permitted decoding over fixed retained payloads.

## What was built and checked

The package includes a frozen manifest, payloads, isolated query workers, a separate checker, declared resource limits, complete responses, grades, and a reproduction record. It separates native decoding, internal reconstruction, and external source recovery.

On October 14, 2026, the portfolio audit checked all 14 manifest entries, passed six synthetic contract tests, and ran the unchanged comparison in a local scratch copy. Its three output files matched the saved originals byte for byte. See [verification](../evidence/VERIFICATION_2026-10-14.md).

| Recorded operation | Result |
| --- | --- |
| 160 retained-only queries | 86 adequate, 30 inadequate under the declared decoder/support, 44 unknown |
| 43 separately triggered source-recovery queries | All 43 adequate |
| Same retained R3/R4 payloads with internal reconstruction | Both answer all five static output questions |
| Conventional full-facet and physical-envelope representations | Adequate on all five static questions |

These are heterogeneous deterministic operations, not 160 independent statistical trials. The recovery queries reuse a fixed source; they are not 43 external transfer cases.

## What changed the interpretation

The restricted two-segment and old-edge procedures miss answers that can be reconstructed from information already retained in their payloads. Increasing internal computation can therefore change adequacy without adding source information.

A second distinction concerns evidence: a native procedure can report the correct optimum value and still receive UNKNOWN because its permitted method lacks a global certificate. Matching an answer key does not supply a missing justification.

The strongest supported account is **payload + decoder + requested output + trust/recovery contract**. It is not simply “more detail requires more stored information.”

## Limits and proposed relevance

This establishes a finite operational result. It does not establish a smallest encoding, an information-theoretic lower bound, novelty, a scaling law, method superiority, general AI benefit, or independent human validation.

For AI evaluation, the proposed application is to distinguish a model or agent's answer from the evidence and recovery procedure needed to rely on it. That application still needs a dedicated task and a competent conventional baseline.

The separate local-time transfer experiment, EXP-002, remains [stopped and unassessable](../case-studies/EXPERIMENT_INTEGRITY.md). Its primary observations cannot certify successful transfer.

## Inspect the source

- [Operational contract](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-001-operational-addendum-v1.md)
- [Runner](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/run.py), [solver](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/core.py), and [checker](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/check.py)
- [Manifest](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/MANIFEST.json)
- [Complete results](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/run01/RESULTS.json) and [original reproduction record](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/run01/REPRODUCTION.json)
