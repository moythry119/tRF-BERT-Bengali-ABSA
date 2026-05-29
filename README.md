# tRF-BERT: Aspect-Based Sentiment Analysis in Bengali

**Published in PLOS ONE, September 2024**
DOI: https://doi.org/10.1371/journal.pone.0308050

## Overview
Novel hybrid model combining BERT and Random Forest (tRF-BERT)
for Aspect-Based Sentiment Analysis in the Bengali language.
Evaluated on Cricket and Restaurant benchmark datasets.

## Key Results

| Model | Dataset | Accuracy | F1-score |
|-------|---------|----------|----------|
| tRF-BERT | Cricket | **0.89** | **0.85** |
| tRF-BERT | Restaurant | **0.92** | **0.89** |
| RoBERTa | Cricket | 0.88 | 0.84 |
| BERT | Cricket | 0.83 | 0.78 |

tRF-BERT outperforms all baselines on both datasets.

## Model Architecture
- BERT (bert-base-uncased) fine-tuned for aspect classification
- Random Forest with TF-IDF vectorization
- Combined predictions fed into ANN with ReLU + dropout
- Softmax output for multi-class classification

## Datasets
- Cricket: 2,979 Bengali cricket comments, 5 aspect categories
- Restaurant: 2,059 Bengali restaurant reviews, 5 aspect categories
- Source: Rahman et al. (2018)
- https://github.com/atik-05/Bangla_ABSA_Datasets

## Installation
