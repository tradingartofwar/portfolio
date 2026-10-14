# Evidence standards

A claim must state its object, scope, source revision, verification method, result, limitations, and review status. Evidence type and validation strength are separate dimensions.

| Evidence type | What it permits | What it does not imply |
| --- | --- | --- |
| Implemented system | Identified source code implements named behavior | Successful execution, deployment, safety, or usefulness |
| Implemented and checked | Stated checks passed at a pinned revision | Correctness beyond those checks or operational reliability |
| Observed operational result | A dated outcome with its observation method and denominator | Causality, representative performance, or generalization |
| Reproduced experimental result | A specified procedure reproduced a result within scope | Novelty, independent human validation, or external utility |
| Provisional finding / hypothesis | A testable proposition with counterevidence and failure criteria | Established mechanism or performance |
| Architectural proposal | A design and its intended behavior | Implemented enforcement or adoption |
| Personal interpretation | An explicitly attributed interpretation | An empirical finding about cognition or other people |

The source research vocabulary—KNOWN, REPRODUCED, OBSERVED, HYPOTHESIS, OPEN, DISPROVEN—retains its meaning. A portfolio summary cannot promote a source claim.

## Claim contract

For every substantive claim record:

1. A stable ID and one exact statement.
2. Source repository, immutable commit, and artifact path.
3. Evidence type and original claim status.
4. What was inspected, executed, or compared, and when.
5. Inputs, denominator, environment, and command where applicable.
6. Failures, unknowns, stops, counterchecks, and missing controls.
7. Attribution: human direction, AI contribution, and actual review.
8. Publication permission and sensitivity.
9. What evidence would justify changing the claim.

Separate a document's report of a test from a fresh test. Separate a test pass from a live service. Separate a successful return code from a verified result package. Separate algorithmic crosschecking from independent review.

## Publication rules

Use public, non-sensitive sources for public claims. Private source access is not permission to publish it. Sanitized case studies require a bounded release review; a public link is not evidence that everything in the destination is suitable to quote.

Keep client, clinical, financial, family, credential, and operational records out of this repository. Do not publish secret values, private logs, or screenshots containing sensitive details. Never change source-repository visibility as a publication shortcut.

Verify exact credential names, issuer, program type, completion status, and dates before publishing them. Self-reported experience must not silently become a verified employment history.

## Corrections

Preserve the original claim, the correcting evidence, and the new disposition in Git history. A known failure or missing artifact must not disappear through a rerun. Research decisions stay in their owning repository; this portfolio links to them and records the scope of its own checks.

AI may draft, implement, and review. AI agreement is not an independent proof certificate or substitute for human authorization.
