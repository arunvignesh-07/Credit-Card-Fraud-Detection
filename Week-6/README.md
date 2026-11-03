# Week 6 – Feature Engineering

**Project:** Credit Card Fraud Detection  
**Course:** Data Science and Visualization (DSV)  
**Contributor:** Arunvignesh R S

## Overview

Week 6 focuses on feature engineering techniques to prepare the credit card transaction dataset for further analysis and machine learning. The main objective is to transform existing features, create new features, and apply scaling techniques to improve data representation.

## Objectives

- Understand the dataset structure and feature distributions.
- Analyze skewness in the transaction Amount feature.
- Apply log transformation to reduce skewness.
- Create new features using transaction amount categories.
- Perform one-hot encoding.
- Split the dataset into training and testing sets.
- Apply normalization and standardization.
- Compare the transformed feature values visually.

## Work Completed

### 1. Dataset Inspection
Loaded the credit card dataset and examined its dimensions, data types, statistical summary, missing values, and duplicate records.

### 2. Skewness Analysis and Log Transformation
Analyzed the distribution of the Amount feature and identified its skewness. Applied log transformation to create a new feature called `Amount_log`.

### 3. Feature Creation and Encoding
Created a new categorical feature named `Amount_Category` based on transaction amounts.

Applied One-Hot Encoding to convert categorical values into numerical representations.

### 4. Train-Test Split
Separated the input features and target variable (`Class`).

Performed an 80:20 stratified train-test split to maintain the original class distribution in both datasets.

### 5. Feature Scaling

Applied two important scaling techniques:

**Min-Max Normalization**
- Transforms values into a fixed range, generally 0 to 1.
- Helps bring features into a common scale.

**Standardization (StandardScaler)**
- Transforms features based on their mean and standard deviation.
- Produces values with approximately zero mean and unit variance.

The scaler was fitted using training data and then applied to testing data to prevent data leakage.

### 6. Visualization
Compared original, normalized, and standardized feature values using visualizations to understand the differences between the scaling techniques.

## Tools and Libraries

- Python
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## Files

| File Name | Description |
|---|---|
| `week_6.ipynb` | Feature engineering notebook |
| `creditcard.csv` | Original dataset |
| `creditcard_week6.csv` | Processed dataset |

## How to Run

1. Clone or download the repository.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open `week_6.ipynb` in Jupyter Notebook.
4. Ensure the dataset is available at the specified file path.
5. Execute all cells in sequence.
6. The processed dataset will be saved as `creditcard_week6.csv`.

## Outcome

Week 6 successfully applies feature engineering techniques, including log transformation, feature creation, encoding, normalization, and standardization. The resulting dataset is prepared for further feature analysis and dimensionality reduction.
