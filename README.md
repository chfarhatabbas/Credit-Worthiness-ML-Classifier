# Credit-Worthiness-ML-Classifier
MS Mathematics Thesis: Comparing ML Classifiers and Resampling Techniques on Imbalanced Credit Datasets.
# Prediction of Bank Credit Worthiness Using Machine Learning

An empirical evaluation of classification algorithms and data-balancing techniques optimized for credit risk assessment. This repository hosts the computational architecture developed during my Master of Science (M.Sc.) in Mathematics thesis at Sir Syed CASE Institute of Technology.

## 📊 Automated Data Pipeline
To ensure complete reproducibility and eliminate dependencies on localized files or private cloud storage paths, this project features an automated data ingestion architecture:
* **Data Source:** UCI Machine Learning Repository ("Default of Credit Card Clients" Dataset | ID: 350)
* **Instance Count:** 30,000 applications containing 23 quantitative and qualitative features.
* **Ingestion Method:** Automated API streaming utilizing the official `ucimlrepo` library.
* **Data Alignment:** The pipeline automatically processes the dual-header array, maps structural feature tags back to their original descriptive labels, and mathematically reconstructs indexing dimensions entirely in-memory.

## 🛠️ Methodologies Implemented
1. **Resampling & Data Balancing:** Synthetic Minority Over-sampling Technique (SMOTE), Random Under-Sampling (RUS), Random Over-Sampling (ROS).
2. **Machine Learning Classifiers:** Extra Trees (ET) Classifier, Decision Tree (DT) Classifier, and Logistic Regression (LR).
3. **Statistical Performance Criteria:** Evaluation modeled across Accuracy, Precision, Recall/Sensitivity, Specificity, and F1-score.

## 📈 Key Research Findings
Through comprehensive benchmarking across multiple configurations, the experimental results established that pairing an **Extra Trees (ET) Classifier with Random Over-Sampling (ROS)** yielded optimal predictive performance, stability, and robustness for managing credit default risk.

## 📂 Project Structure
* `/src`: Self-contained code files for automated data fetching, preprocessing, sampling execution, and model evaluation.
* `/docs`: Project documentation, including the thesis title page,  abstract, table of contents, list of figures, list of tables and abbreviations.
