# Week 2 — Know Your Data / First Impression

## Objective

The objective of Week 2 is to understand the structure, characteristics and quality of the Credit Card Fraud Detection dataset before performing data preprocessing.

## Dataset

The dataset used for this project is the Credit Card Fraud Detection dataset obtained from Kaggle.

## Dataset Dimensions

The dataset contains 284,807 records and 31 columns.

## Target Variable

The target variable is `Class`.

- `Class = 0` → Legitimate transaction
- `Class = 1` → Fraudulent transaction

## Data Understanding

The following operations were performed:

- Displayed the first few records using `head()`
- Checked the dimensions using `shape`
- Examined column names
- Checked data types
- Generated summary statistics using `describe()`
- Checked for missing values
- Examined the target-class distribution

## First Impression

The dataset contains numerical transaction-related features and a binary target variable.

The target classes are highly imbalanced. Legitimate transactions form the vast majority of the dataset, while fraudulent transactions represent a very small proportion.

## Week 2 Outcome

The structure and basic characteristics of the dataset were understood. The dataset was then prepared for the cleaning and preprocessing activities planned for Week 3.
