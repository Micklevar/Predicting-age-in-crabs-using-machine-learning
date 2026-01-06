# Predicting Age in Crabs Using Machine Learning

Supervised machine learning project focused on predicting crab age from physical measurements.

![giphy](https://github.com/user-attachments/assets/4abae2c0-055e-47cd-81ac-83f9f0a49d7f)

## Description

This repository documents a **supervised machine learning project** focused on predicting the age of crabs based on their physical and morphological characteristics. The main objective of the project is to understand and apply the complete machine learning workflow, from exploratory data analysis (EDA) to model training and performance evaluation.

The project is developed as part of a **self-directed learning process**, prioritizing sound technical decision-making, result interpretation, and an understanding of the limitations of each model used.

## Version 1 (Baseline Model)

In this first version, a **linear regression model** is used as a baseline. This approach allows for validating the consistency of the dataset and establishing a reference point for comparison with more complex models.

Although the results are limited, this step provides valuable insights into the data and confirms the need for more expressive models.

## Project Evolution

The project is continuously evolving. Future versions will incorporate:

- Nonlinear regression models  
- Hyperparameter tuning  
- Additional evaluation metrics (e.g., MAE, RMSE)  

The goal is to improve predictive performance and deepen the analysis of the problem.

## Version 2 - Model Development and Evaluation

In Version 2 of the project, the focus shifts from exploratory analysis and baseline modeling to a more structured evaluation of non-linear regression approaches. Building upon the cleaned and preprocessed dataset developed in Version 1, this stage is centered on improving predictive performance and comparing different modeling strategies.

The following techniques and models were implemented:

- Polynomial Linear Regression (degrees 2 and 3) to capture non-linear relationships between physical crab features and age.

- Random Forest Regressor as a tree-based ensemble model capable of modeling complex feature interactions without assuming linearity.

- Scikit-learn pipelines to integrate data preprocessing and model training in a consistent and reproducible workflow, while avoiding data leakage.

Model performance was evaluated using multiple regression metrics:

- Mean Absolute Error (MAE) to measure average prediction error magnitude.

- Mean Squared Error (MSE) to penalize larger prediction errors.

- Coefficient of Determination (R²) to assess the explanatory power of each model.

The results show that the polynomial regression model achieved the best overall performance among the evaluated approaches, outperforming both the baseline linear regression and the Random Forest model under the current experimental conditions. These findings highlight the importance of aligning model complexity with dataset characteristics rather than assuming that more complex models will always yield superior results.
