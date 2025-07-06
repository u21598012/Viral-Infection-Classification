# Viral-Infection-Classification

Project Overview
This project explores the use of Support Vector Machines (SVM) to predict viral infection status in mice based on medication administration data. The [dataset](https://www.kaggle.com/datasets/brsahan/mouse-viral-infection-study-dataset) originates from a controlled laboratory study and contains measurements of medication volumes given to each mouse, with a binary label indicating infection status (1 = Infected, 0 = Healthy).

The goal was to evaluate whether machine learning, specifically SVMs, can accurately classify infection outcomes, potentially supporting future biomedical studies focused on biomarker discovery and treatment strategies.

Tech Stack & Tools
Databricks
Distributed computing environment for scalable data analysis and model training.

Interactive notebooks for seamless code execution, visualization, and experiment tracking.

Data Preprocessing
Pandas for initial data manipulation.

Preprocessing steps included:

Lowercasing column names and replacing spaces with underscores.

Imputation of missing numerical values using mean values.

Machine Learning
scikit-learn:

Core SVM implementation for binary classification.

Train-test splitting and model evaluation.

Hyperopt:

Automated hyperparameter optimization (kernel selection, regularization, etc.).

Objective function designed to maximize AUC (Area Under the ROC Curve).

Achieved final AUC score: 1 (perfect separation on the test set).

Experiment Tracking
MLflow:

Parameter logging and metric tracking for each experiment run.

Artifact logging (models, signatures) to support reproducibility and deployment readiness.

Key Features
End-to-end binary classification workflow fully integrated in Databricks.

Automated hyperparameter search using distributed tuning.

Complete experiment management and reproducibility with MLflow.

Minimal yet robust data preprocessing pipeline tailored for biomedical data.

