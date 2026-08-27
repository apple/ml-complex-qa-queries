# [From Preferences to Principles: Rubric-Based Alignment for Grounded Knowledge Answers](https://arxiv.org/abs/2608.23812)

This repository provides the synthetic training queries used for model post-training in the [paper](https://arxiv.org/abs/2608.23812) on open-domain question-answering.

## Disclaimer

This release contains synthetic training queries generated through broad open-domain query synthesis prompts for research reproducibility purposes only. References to Apple products, competing consumer brands, or comparative product-style queries emerged naturally as part of the synthetic generation process and are not intended as product evaluations, rankings, benchmarking, or representative user studies.

- The queries are fully synthetic.
- Not derived from user logs or proprietary data.
- This artifact is intended for reproducibility of the research methodology rather than evaluation of consumer products or assistants.

## Data

`data/queries.jsonl` contains 4,716 synthetic training queries. Each line is a JSON object with fields: `query_id`, `query`, `query_date`.

## Query Types

The queries were generated using 8 distinct prompting strategies to cover a range of complexity and ambiguity:

| Type | Description |
|------|-------------|
| General open-ended | Queries requiring explanation, reasoning, or multi-aspect answers (comparisons, tradeoffs, synthesis) |
| Ambiguity-heavy | Queries with entity, intent, scope, comparison, or temporal ambiguity |
| Time-sensitive | Queries depending on recent events, releases, or outcomes |
| Fragment-style | Short (1-6 word) incomplete queries reflecting real search behavior |
| Underspecified | Queries missing key constraints (budget, location, preferences) |
| Implicit time-sensitive | Queries where recency matters but is not explicitly stated |
| Location-dependent | Queries where the answer depends on location, but no location is provided |
| Multi-intent | Queries combining multiple intents in a single utterance |

## Citation

If you use this data, please cite:

```bibtex
@misc{saini2026preferencesprinciplesrubricbasedalignment,
      title={From Preferences to Principles: Rubric-Based Alignment for Grounded Knowledge Answers},
      author={Aman Saini and Priyanshu Kumar and Eric Peng and Kai Yuan and Harsh Girase and Wanming Chen},
      year={2026},
      eprint={2608.23812},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://arxiv.org/abs/2608.23812},
}
```

