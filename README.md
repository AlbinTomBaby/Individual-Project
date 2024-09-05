# Data-Driven Player Transfer Optimization System

## Overview

The **Data-Driven Player Transfer Optimization System** is designed to help football teams optimize their player transfers by applying advanced data science techniques. The system integrates machine learning models and football analytics to provide accurate player valuations, identify undervalued talents, and maximize both financial and strategic outcomes.

## Objective

The objective of this project is to develop a data-driven framework that enables football clubs to make more objective and informed decisions regarding player transfers, enhancing both on-field performance and financial sustainability.

## Key Features

- **Machine Learning Models**: Utilizes advanced models like XGBoost, Random Forest Classifier, and a custom threshold classifier to predict whether a player should "stay at the club" or "seek better options."
- **Data Integration**: Combines various datasets, including player performance data, economic factors, and match statistics, to offer a holistic analysis.
- **Exploratory Data Analysis (EDA)**: Conducts EDA to understand data distributions, correlations, and key insights to drive transfer decisions.
- **Feature Engineering**: Leverages features such as offensive and defensive scores, pass completion percentages, and wage metrics for predictive modeling.
- **Real-Time Adaptation Potential**: Designed to integrate real-time data sources for continuous optimization.

## Methodology

1. **Dataset Collection**:
   - Data is collected from publicly available sports databases like FBref, covering features such as goals, assists, passes completed, defensive actions, and player wages.

2. **Data Preparation**:
   - Data is cleaned and preprocessed to handle missing values and inconsistencies. The relevant columns are selected and merged into a single dataset.

3. **Model Building**:
   - Three machine learning models are implemented:
     - **XGBoost Classifier**: Achieves high accuracy (99.24%) using gradient boosting.
     - **Random Forest Classifier**: Provides robust results with an accuracy of 97.71%.
     - **Custom Threshold Classifier**: A rule-based model with an accuracy of 60.31%.

4. **Model Evaluation**:
   - Models are evaluated using metrics like accuracy, confusion matrix, and classification reports. XGBoost demonstrates the highest accuracy and robustness.

5. **SHAP Analysis**:
   - SHAP values are used to interpret the XGBoost model, highlighting influential features such as age, offensive score, defensive score, and weekly wage.

## Code Usage

The provided Python code contains scripts for data loading, cleaning, model training, evaluation, and analysis.

### Prerequisites

- Python 3.x
- Required libraries: `pandas`, `numpy`, `scikit-learn`, `xgboost`, `matplotlib`, `seaborn`, `shap`

### Steps to Run the Code

1. Install the required libraries using pip:

   ```bash
   pip install pandas numpy scikit-learn xgboost matplotlib seaborn shap
