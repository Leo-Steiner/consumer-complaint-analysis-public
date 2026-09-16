# Consumer Complaint Analysis

Topic modelling and text analysis on the CFPB consumer complaint database using LDA and NMF.

## Overview

This project analyses consumer complaints submitted to the Consumer Financial Protection Bureau (CFPB). It cleans and vectorises the complaint narratives, applies Latent Dirichlet Allocation (LDA) and Non-negative Matrix Factorization (NMF) to identify recurring topics, and compares the two models on coherence, diversity and interpretability.

## Key results

| Model | Topics | Coherence | Top terms |
|---|---|---|---|
| LDA | 2 | 0.58 | payment, loan, account, pay, bank |
| NMF | 2 | 0.52 | account, bank, call, get, loan |

- Topic 1: credit / report / account (41.98 %)
- Topic 2: payment / loan / account (58.02 %)
- Best model by coherence: LDA (0.58 vs 0.52)
- Best model by diversity: LDA

## Repository structure

- `src/` — Jupyter notebook with the full analysis pipeline
- `results/` — model evaluation, topic terms, visualisations
- `data/` — raw and processed data (kept locally)
- `docs/` — documentation
- `tests/` — test scripts

## How to run

1. Install the dependencies:

       pip install -r requirements.txt

2. Open the notebook:

       jupyter notebook src/consumer-complaint-analysis.ipynb

## Dependencies

See `requirements.txt`.

## Licence

MIT
