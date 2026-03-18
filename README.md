🍷 Predicting Wine Quality Using Machine Learning Algorithms


Project Overview

This project explores whether measurable physicochemical properties of wine (such as acidity, alcohol content, and pH) can be used to automatically predict if a wine is of "Good" quality. By leveraging the UCI Wine Quality Dataset, I developed a binary classification model to differentiate between "Good" wines (quality score ≥ 7) and "Not Good" wines.


Why this matters: 

Automating quality assessment helps wineries maintain consistency, reduce reliance on expensive sensory panels, and identify the chemical drivers of premium wine.


Dataset

Source: UCI Wine Quality Dataset (Portugal's Vinho Verde region).

Samples: 6,497 total (1,599 Red, 4,898 White).

Features: 11 chemical attributes including alcohol, volatile acidity, sulphates, and residual sugar.

Preprocessing: Combined red and white datasets, handled class imbalance, and applied feature scaling.


Tech Stack

Language: Python

Libraries: Pandas, NumPy, Scikit-learn, XGBoost, Matplotlib, Seaborn

Environment: Jupyter Notebook / Google Colab


Machine Learning Pipeline

Exploratory Data Analysis (EDA): Identified key correlations, such as the strong positive relationship between alcohol content and quality.

Feature Engineering: Treated wine type (Red vs. White) as a categorical feature to maintain the unique characteristics of each.

Model Selection: Evaluated multiple algorithms including Logistic Regression, Decision Trees, Gradient Boosting, and XGBoost (Top Performer).

Hyperparameter Tuning: Optimized models using GridSearchCV to maximize AUC-ROC scores.


Key Results

Ensemble Advantage: Non-linear ensemble models significantly outperformed simpler models like Logistic Regression.

Generalization: The model showed high consistency between cross-validation and test performance, indicating strong generalization to unseen data.

Key Drivers: Alcohol levels and volatile acidity were identified as primary predictors of wine quality.

Repository Structure
Wine_Classification_Project_.ipynb: Full technical implementation and analysis.

Writeup_Predicting_Wine_Quality_Report.pdf: Comprehensive project write-up and findings.
