# When a successful run cannot be certified

**Evidence:** read-only artifact integrity check and documented stop.  
**Experiment:** EXP-002, bounded local-time interpretation.  
**Disposition:** STOPPED / UNASSESSABLE; H1 and H2 remain open.

## The consequential distinction

A process can return success while its retained evidence fails the experiment's acceptance rule. EXP-002 preserves that distinction rather than treating the runner's summary as authoritative.

The [source report](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-002-results-2026-10-06.md) records a successful runner return and primary grades of 12 adequate queries for each arm. But full canonical replay was also required. The saved replay contains only 13 of 24 required records and disagrees with the runner's recorded SHA-256.

The October 14 portfolio audit independently recomputed the saved file's hash and counted its records. It confirmed the documented discrepancy. “Independently” here means a fresh computation in this audit, not independent human review.

## What follows—and what does not

- The saved replay is incomplete relative to the frozen contract.
- The original success assertion remains part of the record, without endorsement.
- The result cannot certify H1 cross-domain conformance under the frozen acceptance rule.
- The primary tie does not establish method advantage or a fully reproduced comparative null.
- Cause and timing of the artifact discrepancy remain unknown.

No EXP-002 decoder, runner, repair, or replacement replay was executed during this audit.

## Governance relevance

This is an inspectable example of an evidence requirement changing the reported result. It is relevant to research governance as a decision artifact: the acceptance rule, discrepancy, disposition, and conditions for renewed work remain visible. It is not proof of enterprise governance experience or of successful external transfer.

## Sources

- [Execution and stop report](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-002-results-2026-10-06.md)
- [Integrity-stop record](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-002-integrity-stop-2026-10-06.json)
- [Saved replay](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp002-run01/REPLAY.json)
- [Original artifact hashes](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp002-run01/ARTIFACT_HASHES.json)
- [Fresh verification details](../evidence/VERIFICATION_2026-10-14.md)
