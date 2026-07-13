# Dataset Card

## Overview

| Field | Value |
|-------|-------|
| Name | ml-complex-qa-queries |
| Size | 4,716 synthetic queries |
| Format | JSONL (`query_id`, `query`, `query_date`) |
| Language | English |
| License | CC BY 4.0 |

## Description

A synthetic query set generated for post-training rubric-based alignment models in open-domain question-answering research. The queries span 8 prompting strategies covering complexity, ambiguity, time-sensitivity, and multi-intent patterns.

## Intended Use

- Reproducibility of training setups described in "From Preferences to Principles: Rubric-Based Alignment for Grounded Knowledge Answers"
- Research on rubric-based alignment for grounded knowledge answers

## Out of Scope

- Product evaluation, ranking, or benchmarking
- Representative user studies or user behavior analysis
- Supervised fine-tuning (no answers, passages, or preference labels are included)

## Generation Methodology

Queries were generated using 8 distinct synthetic prompting strategies:

1. General open-ended
2. Ambiguity-heavy
3. Time-sensitive
4. Fragment-style
5. Underspecified
6. Implicit time-sensitive
7. Location-dependent
8. Multi-intent

## Disclaimer

This release contains synthetic training queries generated through broad open-domain query synthesis prompts for research reproducibility purposes only. References to Apple products, competing consumer brands, or comparative product-style queries emerged naturally as part of the synthetic generation process and are not intended as product evaluations, rankings, benchmarking, or representative user studies.

- The queries are fully synthetic.
- Not derived from user logs or proprietary data.
- This artifact is intended for reproducibility of the research methodology rather than evaluation of consumer products or assistants.
