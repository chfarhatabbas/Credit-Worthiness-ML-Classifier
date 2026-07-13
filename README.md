# Credit Worthiness Prediction Using Machine Learning

A machine learning framework for predicting bank credit worthiness using supervised classification algorithms and class imbalance handling techniques.

---

## Project Overview

This repository contains the implementation of a machine learning framework developed for predicting bank credit worthiness. The project was completed as part of the Master of Science (MS) in Mathematics at Sir Syed CASE Institute of Technology, Islamabad, Pakistan.

The objective of this research is to investigate the effectiveness of supervised machine learning algorithms for credit risk assessment. The proposed framework applies data preprocessing, feature engineering, and class imbalance handling techniques before training and evaluating multiple classification models.

Three supervised machine learning algorithms are implemented and compared:

- Logistic Regression
- Decision Tree Classifier
- Extra Trees Classifier

To address the class imbalance problem commonly encountered in credit datasets, the following sampling techniques are investigated:

- Random Under-Sampling
- Random Over-Sampling
- Synthetic Minority Over-sampling Technique (SMOTE)

The models are evaluated using multiple performance metrics, including Accuracy, Precision, Recall, F1-score, Sensitivity, and Specificity. Among the evaluated approaches, the Extra Trees Classifier combined with Random Over-Sampling achieved the best predictive performance on the selected dataset.
