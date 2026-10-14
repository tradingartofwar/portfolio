# Verification record — October 14, 2026

**Method:** GitHub connector reads at pinned revisions; exact retrieved UTF-8 text materialized into isolated local scratch copies; bounded commands below. Original repositories were not edited.  
**Reviewer:** AI assistant acting at Troy Vance Williams's direction. This is a fresh technical check, not independent human validation.  
**Python:** 3.12.14. No model API or live operational service was called.

## Source pins

| Repository | Inspected commit |
| --- | --- |
| representation-science | `b8750dee72d5cc9a76d5dbee59077743cee735a9` |
| the-lonely-runner-conjecture | `c8a287f52ef0066d2ba6247094bdeba023825081` |

This was a selective evidence audit, not an exhaustive review of every file or mathematical argument.

## Lonely Runner

From the source repository root:

```bash
python -m unittest discover -s tests -v
```

Result: **25 tests passed**, exit 0. The original suite includes a 162-speed-set crosscheck. No broader research scans, browser rendering, or proof-candidate certification were performed.

## EXP-001

All **14 entries** in the retrieved input manifest matched their SHA-256 values.

From the Representation Science root:

```bash
python experiments/exp001/test_contract.py
python experiments/exp001/run.py \
  --freeze-commit 96141bfe0b0de99c99ddfdb11e6d41187dc1eef2 \
  --output-dir /tmp/exp001-portfolio-audit
```

Use a new, nonexistent output directory. The audit used its own fresh scratch output directory.

Six contract tests passed; the full run exited 0. It produced 160 retained-only queries and 43 recovery queries. All three files below were compared as bytes against the saved `experiments/exp001/run01/` files at the inspected revision:

| File | Bytes | SHA-256 | Comparison |
| --- | ---: | --- | --- |
| RESPONSES.json | 102065 | `398c020ec4437bf66e2d3f2062e144189c26bce5a2ce34c27200853b929d1a48` | Identical |
| RESULTS.json | 222150 | `dcf52fa0598b9398d766204a77174ca5f187d2aa32ba2382489b122620eed72c` | Identical |
| SUMMARY.json | 5188 | `d7a52064e8839566592c9f9257a3947eaac4e21e495d8659a30a8d485fa42278` | Identical |

The runner checks frozen file hashes; its `--freeze-commit` argument is a supplied label, not an independent verification of publication timing. This audit verifies current payload integrity and reproducibility. The historical freeze/publication sequence remains documented by the [original record](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/exp001/run01/REPRODUCTION.json), not newly observed here.

## EXP-002: read-only integrity check

The saved `experiments/exp002-run01/REPLAY.json` parses as a list with **13 records**, versus 24 required by the [source stop report](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-002-results-2026-10-06.md).

- Observed SHA-256: `a349c256c8af574af7a2019c26bb2bc2cd8a6eaf2c75439ebdd0676d3146a43f`
- Original recorded SHA-256: `a3cc498c4dbfdea130a7f443123c5826f1cf62db2d1c90fa0dff2e4a8f4396c5`

This agrees with the [documented integrity stop](https://github.com/tradingartofwar/representation-science/blob/b8750dee72d5cc9a76d5dbee59077743cee735a9/experiments/EXP-002-integrity-stop-2026-10-06.json). This check did not rerun the experiment, recompute reference answers, repair records, or establish the cause of the discrepancy.

## Interpretation boundary

Byte-identical reproduction strengthens confidence that the specific computation is recoverable. It does not establish scientific novelty, real-world usefulness, generalization, independent authorship, or a benefit over strong conventional practice.
