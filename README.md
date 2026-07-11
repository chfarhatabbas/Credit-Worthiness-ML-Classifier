# Credit-Worthiness-ML-Classifier
MS Mathematics Thesis: Comparing ML Classifiers and Resampling Techniques on Imbalanced Credit Datasets.
# Prediction of Bank Credit Worthiness Using Machine Learning

An empirical evaluation of classification algorithms and data-balancing techniques optimized for credit risk assessment. This repository hosts the computational architecture developed during my Master of Science (M.Sc.) in Mathematics thesis at Sir Syed CASE Institute of Technology.

## 📊 Dataset Setup
* **Data Source:** UCI Machine Learning Repository ("Default of Credit Card Clients" Dataset)
* **Instance Count:** 30,000 applications containing 23 quantitative and qualitative features.
* * **Accessing the Data:** To run the scripts in the `/src` folder, please download the raw data from one of the official public links:
  👉 [Option 1: Official UCI Repository Portal](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)  
  👉 [Option 2: Verified Kaggle Mirror Repository](https://www.kaggle.com/datasets/uciml/default-of-credit-card-clients-dataset)
## 🛠️ Methodologies Implemented
1. **Resampling & Data Balancing:** Synthetic Minority Over-sampling Technique (SMOTE), Random Under-Sampling (RUS), Random Over-Sampling (ROS).
2. **Machine Learning Classifiers:** Extra Trees (ET) Classifier, Decision Tree (DT) Classifier, and Logistic Regression (LR).
3. **Statistical Performance Criteria:** Evaluation modeled across Accuracy, Precision, Recall/Sensitivity, Specificity, and F1-score.

## 📈 Key Research Findings
Through comprehensive benchmarking, the experimental results established that pairing an **Extra Trees (ET) Classifier with Random Over-Sampling (ROS)** yielded optimal predictive performance and robustness for managing credit default risk.

## 📂 Project Structure
* `/src`: Code files for data preprocessing, sampling execution, and model evaluation.
* `/docs`: Project abstract, list of figures, abbreviations, and table of contents.
