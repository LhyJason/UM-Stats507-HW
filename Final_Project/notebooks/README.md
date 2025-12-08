Loan Eligibility Assessment — STAT 507 Final Project

Author: Hanyang Liu
Course: UMich STAT 507 — Data Science & Analytics in Python
Project Type: IEEE-style Final Project (Machine Learning Pipeline)

Overview

This project builds a complete machine learning system to predict loan eligibility using demographic and financial attributes from the Kaggle loan dataset.
Three classification models were implemented and compared:

Logistic Regression

Decision Tree

Random Forest (with GridSearchCV tuning)

The workflow includes preprocessing, visualization, model training, evaluation, and test-set prediction.
All results shown in the final report are fully reproducible using the notebooks in this directory.

Project Structure
Final_Project/
│
├── data/
│     ├── loan-train.csv                 # Training dataset
│     ├── loan-test.csv                  # Test dataset
│     └── loan-test-predictions.csv      # Prediction output file
│
├── Graphs/
│     ├── categorical_distributions.png
│     ├── confusion_matrix_rf.png
│     ├── Dependents.png
│     ├── Education.png
│     ├── Flow_graph.png
│     ├── Gender.png
│     ├── Married.png
│     ├── model_performance_comparison.png
│     └── rf_tuning_curve.png
│
├── notebooks/
│     ├── Final Project.ipynb            # Main end-to-end ML workflow
│     └── Additional codes for visualization.ipynb
│
└── README.md                            # (This file)

Environment Requirements
python >= 3.9
pandas
numpy
matplotlib
scikit-learn


How to Run the Project
1. Run the main pipeline

Open:

notebooks/Final Project.ipynb


This notebook performs:

Data loading & preprocessing

Encoding categorical variables

Training Logistic Regression / Decision Tree / Random Forest

Random Forest hyperparameter tuning

Evaluation & visualization

Prediction generation on loan-test.csv

Saving results to:

data/loan-test-predictions.csv


All figures used in the final report are saved into:

Graphs/

2. Supplementary Visualization

Open:

notebooks/Additional codes for visualization.ipynb


This notebook includes additional plots for:

Married

Dependents

Education

Gender

Stored in:

Graphs/

Key Results
Model	Accuracy	Recall (Class 1)	F1-score (Class 1)
Logistic Regression	0.6992	0.03	0.05
Decision Tree	0.7398	0.53	0.56
Random Forest	0.8130	0.47	0.61

Random Forest provides the strongest and most balanced predictive performance.

Output File

loan-test-predictions.csv contains:

predicted approval labels (Y/N)

probability estimates for both classes

This file is generated automatically by the main notebook.

Reproducibility Notes

To fully reproduce results:

Open notebooks/Final Project.ipynb

Restart Kernel

Run all cells

Ensure directory structure remains unchanged
