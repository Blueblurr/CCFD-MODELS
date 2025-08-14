
#Imbalanced Classification Analysis and Oversampling Techniques

###Description:
This repository contains an exploration of handling class imbalance in classification tasks using a combination of oversampling techniques, hybrid methods, and model evaluation strategies. The goal was to determine whether synthetic data generation or class weighting improves model performance, using a Random Forest classifier as the baseline.

###Key Features & Techniques:

Oversampling Approaches: Implemented SMOTE, ADASYN, and SMOTE + ENN to generate synthetic minority class samples.

Pipeline Integration: Integrated oversampling methods within sklearn pipelines for seamless cross-validation.

Evaluation Metrics: Assessed models using PR-AUC and F1 score with Stratified K-Fold cross-validation to ensure robust evaluation on imbalanced data.

Class Weighting: Tested class_weight='balanced' in Random Forest to prioritize minority class without altering the data.

Alternative Models: Explored gradient boosting methods like XGBoost and LightGBM as potential improvements over the baseline.

Insights: Found that neither oversampling nor class weighting significantly improved performance over the baseline Random Forest on our dataset, indicating the model generalises well even with class imbalance in our specific dataset.
