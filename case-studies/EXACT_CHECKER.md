# Exact checking without losing equality cases

**Evidence:** implementation inspected; 25 existing tests passed during the October 14, 2026 audit.  
**Scope:** bounded rational-input computations. No general conjecture proof.

## Problem

For runners on a circle, the question is whether every other runner is sufficiently far from a chosen runner at some time. A sampled animation can miss isolated equality points—the entire feasible set can have zero interval width.

## Implementation

The [Python checker](https://github.com/tradingartofwar/the-lonely-runner-conjecture/blob/c8a287f52ef0066d2ba6247094bdeba023825081/lonely_runner/checker.py) uses exact rational arithmetic and two separately structured calculations:

- Method A intersects closed allowed-time intervals, preserving singleton points.
- Method B partitions distance curves into affine pieces and evaluates corners and crossings to find a maximum.

The methods share input validation and rational arithmetic. Their agreement is a useful internal crosscheck, not independent authorship or formal proof review. Input normalization preserves the original runner count and a map back to original time. Work limits raise explicit errors rather than returning false mathematical counterexamples.

## Fresh verification

The audit ran the repository's existing suite:

```bash
python -m unittest discover -s tests -v
```

**Result: 25 tests passed.** Coverage includes equality points, rational and signed inputs, normalization, invalid inputs, resource-limit handling, CLI output, and a bounded comparison over 162 speed sets. The test domain is not the full conjecture domain.

The repository also contains an offline demonstration. This audit did not render it or certify its browser layout.

## How this work led to Representation Science

The wider Lonely Runner investigation repeatedly exposed distinctions that compressed representations had lost. Its [founding records](../research/REPRESENTATION_SCIENCE.md#how-lonely-runner-led-here) include isolated equality points carrying the entire existence answer and separate feasible ranges failing to preserve joint compatibility. Those episodes led to Representation Science as an independent inquiry. This checker is one concrete implementation of the same discipline: preserve the structure needed for the question being asked.

## Why it belongs in this portfolio

The engineering example is precise: preserve a distinction that changes the answer, use an alternative algorithm to check the implementation, and distinguish inability to compute from evidence of impossibility. Its relevance to AI evaluation is methodological; no claim about frontier model performance follows from these tests.

## Sources

- [Checker source](https://github.com/tradingartofwar/the-lonely-runner-conjecture/blob/c8a287f52ef0066d2ba6247094bdeba023825081/lonely_runner/checker.py)
- [Regression suite](https://github.com/tradingartofwar/the-lonely-runner-conjecture/blob/c8a287f52ef0066d2ba6247094bdeba023825081/tests/test_checker.py)
- [Original validation account and limits](https://github.com/tradingartofwar/the-lonely-runner-conjecture/blob/c8a287f52ef0066d2ba6247094bdeba023825081/notes/CHECKER_VALIDATION.md)
- [Fresh verification record](../evidence/VERIFICATION_2026-10-14.md)

Newer mathematical arguments elsewhere in the source repository retain their own provisional status. This case study does not certify them.
