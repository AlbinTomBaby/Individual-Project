# Football Player Performance Analysis and Prediction
This project focuses on analyzing football player performance metrics and predicting their wages and performance scores. It includes data cleaning, feature engineering, exploratory data analysis (EDA), model building, and evaluation using various Python libraries.

## Table of Contents
1. [Data Sources](#data-sources)
2. [Project Structure](#project-structure)
3. [Data Preprocessing](#data-preprocessing)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Model Building](#model-building)
6. [Feature Importance](#feature-importance)
7. [Results](#results)
8. [Usage](#usage)

## Data Sources
- **Defensive Action Stats**: Contains player-specific defensive stats like blocks, interceptions, and clearances.
- **Goal and Shot Creation Stats**: Includes metrics like Shot Creating Actions (SCA) and Goal Creating Actions (GCA).
- **Passing Stats**: Provides passing accuracy percentages for each player.
- **Player Wages**: Contains data on players' weekly and annual wages.
- **Shooting Stats**: Includes shooting-related statistics such as goals, shots on target, and conversion rates.

## Project Structure

- **data/**: Folder containing the datasets used in the project.
- **notebooks/**: Jupyter notebooks used for EDA, data processing, model training, and evaluation.
- **images/**: Contains visualizations generated during the EDA and SHAP analysis.
- **src/**: Contains Python scripts for data preprocessing, model training, and evaluation.
- **results/**: Contains the final output files, including predictions and performance metrics.

## Data Preprocessing

The data preprocessing includes:

- **Data Merging**: Merging datasets based on the player names.
- **Data Cleaning**: Handling missing values and converting non-numeric values.
- **Feature Engineering**: Creating new features such as pass completion percentage and converting wages to numeric format.
- **Encoding Categorical Features**: Encoding categorical features like player position and squad.

## Exploratory Data Analysis (EDA)

- A comprehensive EDA was conducted to explore relationships between features.
- **Correlation Matrix**: Visualizes the correlation between different performance metrics.
- **Histograms**: Provide distributions of key features.
- Visuals are provided in the `images/` directory.

## Model Building

The models used in the project include:

- **Random Forest Classifier**
- **XGBoost Classifier**

The models were evaluated based on accuracy, precision, recall, and F1-score.

## Feature Importance

- **SHAP (SHapley Additive exPlanations)** was used to interpret the importance of various features in predicting player wages and performance.
- Visualizations are provided to show the average impact of each feature on the model's output.

## Results

The final predictions, along with the cleaned data, are saved in the `results/final_table_with_predictions.xlsx` file. Model performance metrics and feature importance plots are available in the repository.

## Usage

1. Run the preprocessing script to clean and merge the data.
2. Execute the notebooks in the `notebooks/` folder to perform EDA and model training.
3. Generate predictions and evaluate the model using the scripts in the `src/` folder.
