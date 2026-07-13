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

## Key Features

- Machine learning framework for bank credit worthiness prediction.
- Comparative evaluation of three supervised classification algorithms.
- Investigation of three class imbalance handling techniques, including SMOTE.
- Comprehensive performance assessment using multiple classification metrics.
- Reproducible implementation developed in Google Colab using Python and Scikit-learn.
- Structured research repository designed to support future journal publication and academic research.

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

This project uses the **Default of Credit Card Clients** dataset obtained from the **UCI Machine Learning Repository**.

| Attribute | Value |
|-----------|-------|
| **Dataset** | Default of Credit Card Clients |
| **Source** | UCI Machine Learning Repository |
| **Domain** | Credit Risk Assessment |
| **Task** | Binary Classification |
| **Samples** | 30,000 |
| **Predictive Features** | 24 |
| **Target Variable** | Default Payment Next Month |

The dataset contains demographic information, credit history, bill statements, payment records, and previous payment status of credit card clients. These attributes are used to predict whether a client will default on their credit card payment in the following month.

> **Note:** The dataset is publicly available from the UCI Machine Learning Repository. Please refer to the original dataset source for licensing information and download instructions.

---

# Methodology

The proposed machine learning framework follows a systematic workflow for predicting bank credit worthiness. The complete methodology consists of data acquisition, preprocessing, exploratory analysis, class imbalance handling, model development, performance evaluation, and comparative analysis.

## Workflow

The overall workflow of the proposed framework is illustrated below:

```
Dataset Acquisition
        │
        ▼
Data Preprocessing
        │
        ▼
Exploratory Data Analysis (EDA)
        │
        ▼
Handling Class Imbalance
        │
        ▼
Model Training
        │
        ▼
Model Evaluation
        │
        ▼
Performance Comparison
        │
        ▼
Best Performing Model
```

## Methodology Steps

### 1. Dataset Acquisition

The dataset was obtained directly from the UCI Machine Learning Repository using the `ucimlrepo` Python package, ensuring reproducibility and easy access to the latest version of the dataset.

### 2. Data Preprocessing

The raw dataset was prepared for machine learning by performing the necessary preprocessing operations. These included inspecting the dataset structure, handling categorical and numerical variables, checking for missing values, and preparing the feature matrix and target variable for model development.

### 3. Exploratory Data Analysis (EDA)

Exploratory Data Analysis was conducted to better understand the characteristics of the dataset. Various visualizations and statistical summaries were used to examine feature distributions, identify potential patterns, and analyze relationships between variables.

### 4. Handling Class Imbalance

Since credit risk datasets often contain imbalanced class distributions, three different sampling techniques were investigated:

- Random Under-Sampling
- Random Over-Sampling
- Synthetic Minority Over-sampling Technique (SMOTE)

The impact of each sampling strategy on model performance was evaluated and compared.

### 5. Model Development

Three supervised machine learning algorithms were trained and evaluated:

| Model | Description |
|--------|-------------|
| Logistic Regression | Linear classification model used as the baseline. |
| Decision Tree | Tree-based classification algorithm capable of learning non-linear decision boundaries. |
| Extra Trees Classifier | Ensemble learning algorithm based on multiple randomized decision trees. |

Each model was trained using the same preprocessing pipeline to ensure a fair comparison of predictive performance.

### 6. Model Evaluation

The predictive performance of each model was evaluated using several classification metrics:

- Accuracy
- Precision
- Recall
- F1-score
- Sensitivity
- Specificity

Confusion matrices and classification reports were also used to analyze model performance.

### 7. Comparative Analysis

The performance of all machine learning models was compared under different class imbalance handling techniques to determine the most effective approach for predicting bank credit worthiness.

The experimental results showed that the **Extra Trees Classifier combined with Random Over-Sampling** achieved the best overall predictive performance on the selected dataset.


---

# Machine Learning Models

Three supervised machine learning classification algorithms were implemented and evaluated in this study. These algorithms were selected to compare different learning strategies for predicting credit default while maintaining a consistent experimental framework.

| Model | Category | Description |
|--------|----------|-------------|
| Logistic Regression | Linear Model | A statistical classification algorithm used as the baseline model for binary classification. |
| Decision Tree Classifier | Tree-Based Model | A non-linear model that learns decision rules from the training data and provides interpretable predictions. |
| Extra Trees Classifier | Ensemble Learning | An ensemble algorithm that constructs multiple randomized decision trees and combines their predictions to improve classification performance and reduce overfitting. |

All models were trained using the same preprocessing pipeline and evaluated under identical experimental conditions to ensure a fair and unbiased comparison.

---

# Handling Class Imbalance

Class imbalance is a common challenge in credit risk prediction because the number of non-default clients is usually much larger than the number of default clients. Training machine learning models on imbalanced data may result in biased predictions toward the majority class.

To investigate the effect of class imbalance on predictive performance, three different sampling techniques were applied before model training.

| Sampling Technique | Description |
|--------------------|-------------|
| Random Under-Sampling | Reduces the size of the majority class to obtain a balanced training dataset. |
| Random Over-Sampling | Increases the minority class by randomly duplicating existing minority samples. |
| SMOTE (Synthetic Minority Over-sampling Technique) | Generates synthetic minority class samples instead of duplicating existing observations. |

Each sampling technique was independently combined with every machine learning model, allowing a comprehensive comparison of classification performance under different class distributions.

---

# Performance Evaluation

The predictive performance of each machine learning model was assessed using multiple evaluation metrics commonly employed in binary classification problems.

| Evaluation Metric | Purpose |
|-------------------|---------|
| Accuracy | Measures the overall proportion of correctly classified instances. |
| Precision | Evaluates the proportion of correctly predicted positive instances among all predicted positives. |
| Recall (Sensitivity) | Measures the ability of the model to correctly identify positive cases. |
| F1-score | Provides the harmonic mean of Precision and Recall, offering a balanced performance measure. |
| Specificity | Measures the ability of the model to correctly identify negative cases. |

In addition to these quantitative metrics, confusion matrices and classification reports were used to provide a more detailed assessment of model performance.

---

# Experimental Results

The performance of all classification models was compared under different class imbalance handling techniques.

Among all evaluated combinations, the **Extra Trees Classifier combined with Random Over-Sampling** achieved the highest predictive performance on the selected dataset.

The experimental results demonstrate that appropriate handling of class imbalance significantly improves classification performance and that ensemble learning methods can provide more reliable predictions for credit risk assessment.

Detailed performance tables, confusion matrices, and comparative analyses will be included in the `results/` directory as the repository continues to evolve.
---

# Technologies Used

The project was developed using the following tools and technologies:

| Category | Technologies |
|----------|--------------|
| Programming Environment | Google Colab |
| Programming Language | Python |
| Machine Learning | Scikit-learn |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn, Plotly |
| Statistical Analysis | SciPy |
| Dataset Source | UCI Machine Learning Repository |
| Version Control | Git, GitHub |

---

# Installation

Clone the repository:

```bash
git clone https://github.com/chfarhatabbas/Credit-Worthiness-ML-Classifier.git
```

Navigate to the project directory:

```bash
cd Credit-Worthiness-ML-Classifier
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

---

# Usage

1. Clone the repository.
2. Install the required Python libraries.
3. Open the Jupyter Notebook located in the `notebooks/` directory using Google Colab or Jupyter Notebook.
4. Execute the notebook sequentially to reproduce the complete machine learning workflow, including data preprocessing, model training, evaluation, and comparative analysis.

---

# Future Work

This repository will continue to be extended as part of ongoing research in machine learning for credit risk assessment. Planned improvements include:

- Evaluation of additional machine learning algorithms, including Random Forest, Support Vector Machine (SVM), K-Nearest Neighbors (KNN), XGBoost, LightGBM, CatBoost, and Artificial Neural Networks.
- Hyperparameter optimization using systematic search techniques.
- Feature selection and dimensionality reduction.
- Cross-validation for improved model generalization.
- Explainable Artificial Intelligence (XAI) techniques such as SHAP and LIME.
- Comparative evaluation using additional benchmark datasets.
- Publication of the extended research in a peer-reviewed journal.

---

# Citation

If you use this repository in your research, please cite the associated thesis:

**Farhat Abbas**

*Prediction of Bank Credit Worthiness Using Machine Learning Algorithms*

Master of Science in Mathematics

Sir Syed CASE Institute of Technology, Islamabad, Pakistan

2023

---

# License

This project is distributed under the MIT License.

See the `LICENSE` file for more information.

---

# Contact

**Farhat Abbas**

GitHub: https://github.com/chfarhatabbas

For questions, suggestions, or research collaborations, please feel free to open an issue in this repository.
