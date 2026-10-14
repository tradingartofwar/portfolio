# When the work changed the question

**Claims:** P-004, P-015, P-018.  
**Evidence:** a documented research-framing decision and a reproduced finite experiment.  
**Source:** Representation Science at `b8750dee72d5cc9a76d5dbee59077743cee735a9`; events recorded October 2–3, 2026, with computational reproduction in the October 14 portfolio audit.  
**Publication review:** this account uses public research records and omits personal and private operational material.

The Lonely Runner investigation produced a question beyond the conjecture: when a compact representation fails, has the solution disappeared, or has the representation stopped supporting the question being asked?

Two linked moments make the Human–AI partnership visible. The first changed what the collaboration investigated. The second changed what it could responsibly conclude.

## Opening the question

The [origin record](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/ORIGIN.md) describes repeated encounters with distinctions that changed the answer: separate feasibility versus joint compatibility, intervals versus isolated equality points, and compact summaries versus recoverable source geometry.

On October 3, AI was explicitly invited to contribute to the framing of the inquiry. Reconsidering the episodes exposed a separate research object: what representation is sufficient for a declared question as independent complexity increases? Vance created Representation Science as its own repository.

That was a consequential choice about research direction. The mathematical work retained its own home; the new program could test the broader question with its own records and experiments.

## Correcting the interpretation

EXP-001 examined compact representations of one fixed runner configuration. Consider its “old-edge” representation, R4. Its native procedure searched retained geometric edges and returned six times at which the runners achieve their greatest minimum separation. Two maximizing times were absent from that search.

The tempting inference was that those answers required information from a richer external source. The experiment tested the inference. The stored data also contained grouped vertices from which the omitted geometry could be reconstructed.

| Same R4 payload, different permitted computation | Result |
| --- | --- |
| Search the retained edges | Six maximizing times; misses `17/35` and `18/35` |
| Reconstruct the convex parent geometry from its stored vertices, then apply the declared constraint | All eight maximizing times and the complete threshold-safe set |
| Additional external source information used by the internal repair | None |

The [reconstruction record](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/records/RR-LR-005-internal-reconstruction.md) and [full report](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-001-results-2026-10-03.md) retain the correction: **missing answers from a restricted search do not establish missing information in its stored description.** Computation and the requested output belong in the adequacy contract alongside the data.

The October 14 audit reran the unchanged experiment. Three output files matched the saved results byte for byte. The [verification record](../evidence/VERIFICATION_2026-10-14.md#exp-001) gives the commands, hashes, and scope.

## Who contributed what

| Contribution | What the record supports |
| --- | --- |
| Human direction | The origin account attributes intuition, framing, correction, and direction to Vance. It records opening AI participation in framing and Vance's decision to establish the separate research repository. |
| AI contribution | The origin account attributes articulation, cross-episode comparison, formalization, and repository construction to AI. The experiment report attributes protocol, implementation, checking, and interpretation to AI under the investigator's direction. |
| Evidence that changed the account | Internal reconstruction recovered the omitted answers from unchanged payloads. The report rejected the stronger information-loss interpretation. |

These sources do not identify a particular human intervention as the cause of the internal-reconstruction correction. The case preserves the contribution detail they actually record.

## What this shows

A working partnership can make the question itself examinable, establish a separate inquiry, and retain a correction to its interpretation. This episode gives concrete form to the operating method: human direction, AI research and execution, and durable records that keep both the result and its limits available.

For agent engineering and oversight, the proposed application is diagnostic: when an answer fails, determine whether the problem lies in retained information, permitted computation, or missing justification before choosing a repair. Transfer beyond this mathematical case requires its own evaluation.

## Inspect or challenge

Begin with the [origin](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/ORIGIN.md), [bounded reconstruction record](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/records/RR-LR-005-internal-reconstruction.md), and [machine-readable verdicts](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/run01/SUMMARY.json). Use the [audit procedure](../evidence/VERIFICATION_2026-10-14.md#exp-001) to reproduce the computation.

An external source read during the internal repair, changed payloads, or a mismatch against the complete reference answers would undermine the stated correction. The result is confined to exposed, deterministic cases; it establishes neither a general recovery guarantee nor measured productivity or cognitive-load gains. The audit is AI-performed technical reproduction, not independent human validation.

[The larger development history](SYNERGISTIC_INTELLIGENCE.md) · [Research program and relational information](../research/REPRESENTATION_SCIENCE.md)
