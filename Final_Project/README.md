# Loan Eligibility Assessment — STAT 507 Final Project

Author: Hanyang Liu  
Course: University of Michigan — STAT 507 Data Science & Analytics in Python  
Project Type: Machine Learning Classification Pipeline Report

## Overview

This project develops a complete machine learning pipeline for predicting loan eligibility using demographic and financial attributes from the Kaggle loan dataset.  
Three machine learning models are implemented: Logistic Regression, Decision Tree, and Random Forest with hyperparameter tuning.  
The workflow includes preprocessing, visualization, model training, evaluation, and the generation of prediction outputs.  
All results in the final report can be reproduced using the notebooks provided in this project.

## Repository Contents

The repository includes:

1. A data folder containing training data, test data, and prediction outputs.
2. A Graphs folder containing all figures used in the report, including categorical distributions, confusion matrices, model comparison plots, and the project workflow diagram.
3. A notebooks folder containing: The main pipeline notebook for end-to-end processing and model training; A supplementary notebook for additional visualization.

## Environment Requirements

Recommended Python environment:

python >= 3.9  
pandas  
numpy  
matplotlib  
scikit-learn  

## How to Run the Project

### Main Pipeline

Open and run the notebook:

notebooks/Final_Project_pipeline.ipynb

This notebook performs data loading, preprocessing, encoding, model training, hyperparameter tuning, evaluation, and prediction generation.  
Prediction results are written to the file:

data/loan-test-predictions.csv

All figures used in the final report are saved into the Graphs folder automatically.

### Additional Visualization

Open and run the notebook:

notebooks/Additional_visualization.ipynb

This notebook generates supplementary plots for variables such as Married, Dependents, Education, and Gender.  
Generated images are saved in the Graphs folder.

## Key Model Results

Logistic Regression  
Accuracy: 0.6992  
Recall (Class 1): 0.03  
F1-score (Class 1): 0.05  

Decision Tree  
Accuracy: 0.7398  
Recall (Class 1): 0.53  
F1-score (Class 1): 0.56  

Random Forest  
Accuracy: 0.8130  
Recall (Class 1): 0.47  
F1-score (Class 1): 0.61  

Class 1 corresponds to the minority "Not Approved" category.  
Random Forest demonstrates the strongest balanced performance.

## Output Files

loan-test-predictions.csv  
Contains predicted approval labels and probability estimates for each applicant.  
Generated automatically by the main pipeline notebook.

## Reproducibility Notes

To reproduce results:

1. Open notebooks/Final_Project_pipeline.ipynb  
2. Restart the kernel  
3. Run all cells in sequential order  
4. Ensure the folder structure is unchanged  
5. The notebook will save figures and output files automatically  

Relative paths are used for compatibility across machines and GitHub.

## References

All references follow IEEE format and appear in the final project report.

## Final Remarks

This repository includes all required components for the STAT 507 Final Project, including a documented machine learning pipeline, reproducible computations, visualization artifacts, and prediction outputs.
