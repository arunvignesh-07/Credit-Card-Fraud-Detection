# Week 7 – Feature Selection and Dimensionality Reduction using PCA

**Project:** Credit Card Fraud Detection  
**Course:** Data Science and Visualization (DSV)  
**Contributor:** Nishanth

## Overview

Week 7 focuses on analyzing relationships between features, identifying highly correlated variables, and applying Principal Component Analysis (PCA) for dimensionality reduction.

The objective is to reduce the number of dimensions while retaining as much important information from the original dataset as possible.

## Objectives

- Analyze relationships between numerical features.
- Generate a correlation matrix and heatmap.
- Identify highly correlated features.
- Apply feature standardization.
- Perform Principal Component Analysis (PCA).
- Analyze explained variance.
- Visualize the reduced dataset using two principal components.

## Work Completed

### 1. Correlation Analysis

Calculated the correlation matrix to understand relationships between numerical features.

Used a correlation heatmap to visualize positive and negative correlations between variables.

### 2. Identification of Highly Correlated Features

Used an absolute correlation threshold of **0.95** to identify highly correlated feature pairs.

This helps identify variables that may contain similar or redundant information.

### 3. Feature Standardization

Standardized the numerical input features before applying PCA.

Standardization is important because PCA is sensitive to differences in feature scales.

### 4. Principal Component Analysis (PCA)

Applied PCA to transform the standardized features into a new set of principal components.

The target variable `Class` was excluded from PCA because it represents the output label rather than an input feature.

### 5. Explained Variance Analysis

Analyzed explained variance and cumulative explained variance.

This helps understand how much of the original dataset's variation is retained by each principal component.

### 6. Two-Dimensional Visualization

Selected the first two principal components:

- `PC1` – First Principal Component
- `PC2` – Second Principal Component

Created a two-dimensional visualization to examine the distribution of legitimate and fraudulent transactions.

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
| `Week_7_Feature_Selection_PCA.ipynb` | Feature selection and PCA notebook |
| `creditcard_week7_pca.csv` | Reduced dataset containing PC1, PC2, and Class |

## How to Run

1. Clone or download the repository.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

3. Open `Week_7_Feature_Selection_PCA.ipynb` in Jupyter Notebook.
4. Ensure the required input dataset is available at the specified file path.
5. Execute all cells in sequence.
6. The reduced PCA dataset will be saved as `creditcard_week7_pca.csv`.

## Important Notes

- The `Class` column is excluded during PCA.
- PCA is an unsupervised dimensionality reduction technique.
- Standardization is performed before PCA.
- Correlation analysis helps identify relationships between features.
- The first two principal components provide a two-dimensional representation, but may not retain all the information from the original dataset.

## Outcome

Week 7 successfully performs correlation analysis, identifies highly correlated feature pairs, and applies PCA to reduce the dimensionality of the dataset.

The final reduced representation contains `PC1`, `PC2`, and `Class`, providing a simplified representation for further analysis of credit card fraud detection.
