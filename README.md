# What Drives BanglishBERT Predictions? A SHAP and LIME Analysis

## Overview
This project investigates the interpretability of **BanglishBERT** for multi-label classification of Bangla–English code-mixed social media text. It uses Explainable AI (XAI) techniques, **SHAP and LIME**, to understand which words influence predictions of four categories:

- Humorous
- Sarcastic
- Offensive
- Vulgar

## Dataset
Experiments were conducted using the **MixSarc dataset**, containing 9,087 manually annotated Bangla–English code-mixed sentences.

After preprocessing and duplicate removal, 8,305 unique sentences were used for model fine-tuning.

## Methodology
- Fine-tuning BanglishBERT for multi-label classification.
- Applying SHAP for global and cross-label feature attribution.
- Using SHAP and LIME for local explanations.
- Analyzing True Positive (TP), True Negative (TN), False Positive (FP), and False Negative (FN) predictions.
- Comparing explanation consistency using Top-5 Jaccard Similarity, Contribution-Sign Agreement, and Signed Spearman Rank Correlation.

## Key Results

| Evaluation Metric | Result |
|---|---:|
| Humorous F1-score | 0.7251 |
| Sarcastic F1-score | 0.4196 |
| Offensive F1-score | 0.1596 |
| Vulgar F1-score | 0.2874 |
| Top-5 Jaccard Similarity | 0.543 |
| Contribution-Sign Agreement | 0.944 |
| Signed Spearman Correlation | 0.681 |

The findings reveal overlapping lexical patterns between Offensive and Vulgar predictions and highlight how individual words can influence model decisions.

## Technologies
- Python
- PyTorch
- Hugging Face Transformers
- BanglishBERT
- SHAP
- LIME
- Scikit-learn
- Pandas, NumPy, Matplotlib

## Research Contributions
This work explores linguistic interpretability in low-resource, code-mixed NLP and provides insights into the strengths and limitations of post-hoc explanation methods for multilingual text classification.

## Authors
Fariha Ahmed and collaborators

