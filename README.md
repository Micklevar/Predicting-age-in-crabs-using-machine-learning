Markdown

# 🦀 Crab Age Prediction: A Professional Machine Learning Approach

## 📌 Project Overview
This repository documents a supervised machine learning project focused on predicting the age of crabs based on physical and morphological characteristics. Beyond a simple regression task, this project prioritizes **statistical rigor** and **clean data engineering** to ensure the final model is robust and generalizable.

The project follows the full Machine Learning lifecycle, with a deep focus on Exploratory Data Analysis (EDA) and evidence-based decision-making.

## 🔬 Engineering Highlights (Current Progress)

### 1. Robust Exploratory Data Analysis (EDA) & Cleaning
* **Data Integrity:** Performed a comprehensive audit of the dataset, confirming 0% missing values across all 3,893 initial samples.
* **Iterative Outlier Management (Tukey's Method):** Implemented a programmatic filtering process using the **Interquartile Range (IQR)**.
    * *Strategic Decision:* Outliers in independent features were removed to reduce noise. However, outliers in the target variable (**Age**, 6.60%) were **preserved** to maintain natural biological variance and prevent predictive bias.
* **Visual Diagnostics:** Developed comparative "Before vs. After" reporting using side-by-side boxplots to validate the impact of data cleaning on physical feature distributions.

### 2. Technical Decision Making
* **Target Integrity:** Justified the retention of extreme age values to allow the model to learn from rare but biologically valid specimens, which is crucial for real-world accuracy.
* **Skewness Analysis:** Identified a **positive skew (right-skewed)** across all weight-related features. This guided the selection of robust scaling techniques to mitigate the influence of long tails on the model's loss function.



## 🚀 Evolution & Roadmap

The project is currently in active development following this phase-based roadmap:

- [x] **Phase 1: Robust EDA & Data Cleaning** (Standardization and outlier mitigation).
- [ ] **Phase 2: Feature Engineering & Correlation Analysis** (Identifying multicollinearity and key predictors).
- [ ] **Phase 3: Model Benchmarking** (Comparative analysis between Linear, Polynomial, and Random Forest models).
- [ ] **Phase 4: Optimization & Pipelines** (Implementing Scikit-learn Pipelines to prevent Data Leakage).

## 📊 Evaluation Metrics
Performance will be assessed using a multi-metric approach for a balanced evaluation:
* **MAE (Mean Absolute Error):** Primary metric due to its robustness against residual outliers in the target.
* **RMSE (Root Mean Squared Error):** To penalize significant prediction deviations.
* **R² Score:** To quantify the variance explained by the final model.

---
**Author:** [Alejandro Santos]  
**Stack:** Python, Pandas, Seaborn, Matplotlib, Scikit-learn.
