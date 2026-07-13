# Credit Worthiness Prediction Using Machine Learning

A machine learning framework for predicting bank credit worthiness using supervised classification algorithms and class imbalance handling techniques.

---

## Project Overview

This repository contains the implementation of a machine learning framework developed for predicting bank credit worthiness. The project was completed as part of the Master of Science (MS) in Mathematics at Sir Syed CASE Institute of Technology, Islamabad, Pakistan.

The objective of this research is to investigate the effectiveness of supervised machine learning algorithms for credit risk assessment. The proposed framework applies data preprocessing, and class imbalance handling techniques before training and evaluating multiple classification models.

Three supervised machine learning algorithms are implemented and compared:

- Logistic Regression
- Decision Tree Classifier
- Extra Trees Classifier

To address the class imbalance problem commonly encountered in credit datasets, the following sampling techniques are investigated:

- Random Under-Sampling
- Random Over-Sampling
- Synthetic Minority Over-sampling Technique (SMOTE)

The models are evaluated using multiple performance metrics, including Accuracy, Precision, Recall, F1-score, Sensitivity, and Specificity. Among the evaluated approaches, the Extra Trees Classifier combined with Random Over-Sampling achieved the best predictive performance on the selected dataset.

---

## Research Objectives

The primary objective of this research is to investigate the application of supervised machine learning techniques for predicting bank credit worthiness and supporting credit risk assessment.

The specific objectives of this study are:

- Develop a machine learning framework for credit worthiness prediction.
- Perform data preprocessing and exploratory data analysis.
- Address class imbalance using multiple sampling techniques.
- Train and compare multiple supervised classification algorithms.
- Evaluate model performance using standard classification metrics.
- Identify the most effective machine learning model for the selected dataset.
- Provide a reproducible implementation for future research and comparative studies.

---

## Repository Structure

```text
Credit-Worthiness-ML-Classifier
│
├── README.md
├── LICENSE
├── .gitignore
├── requirements.txt
│
├── notebooks/
│   └── Credit_Worthiness_Analysis.ipynb
│
├── data/
│
├── results/
│   ├── figures/
│   ├── tables/
│   └── confusion_matrices/
│
├── docs/
│
└── images/
```

### Folder Description

| Folder | Description |
|----------|-------------|
| `notebooks/` | Jupyter Notebook containing the complete machine learning workflow. |
| `data/` | Dataset information and related documentation. |
| `results/` | Experimental results, figures, tables, and evaluation outputs. |
| `docs/` | Additional project documentation. |
| `images/` | Images used in the project documentation and README. |

---

## Dataset

This project uses the **Statlog (German Credit Data)** dataset obtained from the **UCI Machine Learning Repository**.

### Dataset Characteristics

- Source: UCI Machine Learning Repository
- Domain: Credit Risk Assessment
- Task: Binary Classification
- Samples: 30,000
- Features: 24 predictive attributes
- Target Variable: Credit Worthiness (Good / Bad Credit Risk)

The dataset contains demographic, financial, and credit-related attributes that are commonly used for evaluating the credit worthiness of loan applicants.

> **Note:** The dataset is publicly available from the UCI Machine Learning Repository. Please refer to the original source for licensing information and the latest version.

---

## Methodology

The machine learning workflow implemented in this project consists of the following stages:

1. Data acquisition from the UCI Machine Learning Repository.
2. Data preprocessing and cleaning.
3. Exploratory Data Analysis (EDA).
4. Feature encoding and transformation.
5. Class imbalance handling using different sampling techniques.
6. Model training using supervised machine learning algorithms.
7. Performance evaluation using multiple classification metrics.
8. Comparative analysis to identify the best-performing model.

---

## Machine Learning Models

The following supervised classification algorithms are implemented and evaluated in this study:

- Logistic Regression
- Decision Tree Classifier
- Extra Trees Classifier

Each model is trained using identical preprocessing procedures to ensure a fair comparison of predictive performance.
