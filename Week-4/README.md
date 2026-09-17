# Week 4 — Exploratory Data Analysis (EDA)

## Objective

The objective of Week 4 is to perform Exploratory Data Analysis (EDA) on the cleaned Credit Card Fraud Detection dataset.

EDA helps us understand the distribution of transactions, identify patterns between legitimate and fraudulent transactions, and study relationships between different numerical features.

---

## Dataset

The dataset used is the **Credit Card Fraud Detection dataset** obtained from Kaggle.

### Dataset Details

- Original records: 284,807
- Original features: 31
- Target variable: `Class`
- `Class = 0` → Legitimate transaction
- `Class = 1` → Fraudulent transaction

After removing duplicate rows:

- Records: 283,726
- Features: 31
- Missing values: 0
- Duplicate rows remaining: 0

---

## EDA Performed

The following Exploratory Data Analysis techniques were performed:

### 1. Class Distribution

The distribution of legitimate and fraudulent transactions was analyzed.

The dataset is highly imbalanced, with legitimate transactions making up the vast majority of transactions.

### 2. Transaction Amount Distribution

A histogram was used to understand the distribution of the `Amount` feature.

The transaction amount distribution is right-skewed, with most transactions having relatively smaller amounts and a smaller number of transactions having large amounts.

### 3. Transaction Amount by Class

A boxplot was created to compare transaction amounts between:

- Legitimate transactions (`Class = 0`)
- Fraudulent transactions (`Class = 1`)

This helps identify differences in transaction amount patterns between the two classes.

### 4. Statistical Analysis

The mean, median, minimum, maximum, and other descriptive statistics were analyzed for the `Amount` feature.

Average transaction amount:

- Legitimate transactions: approximately **88.29**
- Fraudulent transactions: approximately **122.21**

### 5. Correlation Analysis

A correlation matrix was calculated to understand the relationship between numerical features and the target variable `Class`.

Some features showed stronger relationships with the target than others.

The features with relatively strong absolute correlations with `Class` included:

- `V17`
- `V14`
- `V12`
- `V10`
- `V16`
- `V11`

### 6. Correlation Heatmap

A heatmap was created to visualize correlations between the numerical features.

This provides an overall view of relationships within the dataset.

### 7. Feature Distribution Analysis

The distributions of selected features such as:

- `V1`
- `V2`
- `V3`
- `V4`

were visualized using histograms.

Boxplots were also used to compare these features between legitimate and fraudulent transactions.

### 8. Outlier Analysis

The Interquartile Range (IQR) method was used to identify potential outliers in the `Amount` feature.

Outliers were identified for analysis rather than automatically removed because unusual transactions may contain useful information for fraud detection.

---

## Visualizations

The Week 4 notebook contains the following visualizations:

1. Legitimate vs Fraudulent Transaction Distribution
2. Transaction Amount Histogram
3. Transaction Amount Boxplot by Class
4. Correlation Heatmap
5. `V1` Distribution
6. `V2` Distribution
7. `V3` Distribution
8. `V4` Distribution
9. `V1–V4` Boxplots by Class

---

## Key Observations

- The dataset has a severe class imbalance.
- Legitimate transactions are much more common than fraudulent transactions.
- Transaction amounts show a right-skewed distribution.
- Fraudulent and legitimate transactions show differences in their transaction amount distributions.
- Correlation analysis shows that some anonymized features have stronger relationships with the fraud target.
- Histograms and boxplots help visualize differences between transaction classes.
- Potential outliers were identified using the IQR method.
- Outliers were not blindly removed because they may contain important fraud-related information.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab
- GitHub

---

## Files

```text
Week-4/
│
├── README.md
└── Week_4_EDA_with_Outputs.ipynb
