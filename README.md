# Credit Default Prediction and Policy-Oriented Threshold Analysis

This repository contains a data analysis and predictive modeling project focused on **credit default risk**, completed as part of the **Data Bootcamp (Finance)** course at **NYU Stern**.

The project emphasizes not only predictive performance, but also how model outputs translate into **credit decision policies** through threshold tuning and cost-sensitive evaluation.

---

## Project Overview

The objective of this project is to predict whether a borrower will default on a credit obligation and to analyze how different modeling and threshold-selection strategies affect financial outcomes.

Key themes:
- Comparison of interpretable and high-performance machine learning models
- Precision–recall trade-offs in credit decisions
- Translation of predicted probabilities into decision thresholds
- Cost asymmetry between false positives and false negatives

Rather than prescribing a single “best” model or threshold, the analysis highlights how **institutional preferences and risk appetite** shape optimal credit policies.

---

## Dataset

- **Source:** UCI Machine Learning Repository — *Default of Credit Card Clients (Taiwan)*
- **Observations:** 30,000  
- **Features:** 23  
- **Target:** Binary default indicator (1 = default, 0 = non-default)  
- **Default rate:** 22.12%

The dataset represents a realistic retail credit portfolio with moderate class imbalance.

---

## Repository Structure

├── final.ipynb
├── Credit_Risk_Writeup.pdf
├── Credit_Risk_Presentation.pdf
└── README.md
---

## File Descriptions

### `final.ipynb`
Jupyter notebook containing:
- Data exploration
- Model training (Logistic Regression, Random Forest, HistGradientBoosting)
- Performance evaluation
- Threshold tuning (recall-focused, F1-optimized, cost-sensitive)
- Model interpretation and feature importance

### `Credit_Risk_Writeup.pdf`
Formal written report structured as:
- Introduction  
- Data Description  
- Models and Methods  
- Results and Interpretation  
- Conclusion and Next Steps  

### `Credit_Risk_Presentation.pdf`
Short presentation summarizing:
- Modeling approach
- Key findings
- Policy implications for credit decision-making

---

## Methods Summary

### Models Evaluated
- Logistic Regression (interpretable baseline)
- Random Forest
- HistGradientBoosting

### Evaluation Techniques
- ROC–AUC
- Precision, recall, and F1-score
- Confusion matrices

### Threshold Tuning
- Recall-targeted thresholds
- Maximum F1-score thresholds
- Cost-sensitive decision rules

Interpretability is emphasized for logistic regression, while tree-based models are assessed primarily on predictive and economic performance.

---

## Key Findings

- Tree-based models outperform logistic regression in ROC–AUC and F1-score.
- Threshold choice materially affects portfolio outcomes.
- Recall-focused thresholds reduce missed defaults but increase false positives.
- Cost-sensitive thresholds illustrate how risk aversion drives decision policy.
- Logistic regression remains valuable for transparency and governance despite lower predictive accuracy.

---

## Technologies Used

- Python  
- pandas, numpy  
- scikit-learn  
- matplotlib  
- Jupyter Notebook / Google Colab  

---

## Notes

This project is intended as an **academic demonstration** of credit risk modeling concepts and policy trade-offs.  
Results and thresholds should be interpreted in the context of institutional objectives, regulatory requirements, and business constraints.
