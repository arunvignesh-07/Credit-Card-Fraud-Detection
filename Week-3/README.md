# Week 3 — Cleaning Sprint

## Objective

The objective of Week 3 is to identify and handle data-quality issues in the Credit Card Fraud Detection dataset.

## Activities Performed

- Checked for missing values
- Identified duplicate records
- Removed duplicate records
- Detected potential outliers
- Visualized outliers using boxplots
- Applied the IQR method for outlier detection
- Compared the dataset before and after cleaning

## Missing Values

No missing values were found in the dataset.

## Duplicate Records

A total of 1,081 duplicate records were identified and removed.

Dataset size changed from:

284,807 rows → 283,726 rows

## Outlier Detection

Potential outliers in the `Amount` feature were identified using the Interquartile Range (IQR) method.

The detected outliers were not automatically removed because unusual transaction amounts may contain useful information for fraud detection.

## Week 3 Outcome

The dataset was cleaned by removing duplicate records and checking for missing values and potential outliers.

The cleaned dataset is ready for Exploratory Data Analysis in Week 4.
