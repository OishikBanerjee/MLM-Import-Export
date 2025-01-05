# Imports and Exports Data Analysis

## Project Overview

This project conducts a comprehensive analysis of international trade transactions, including both imports and exports. The goal is to derive valuable insights for business analytics, economic research, and financial modeling. The dataset, sourced from Kaggle, provides detailed information on 15,000 international trade transactions.

## Data Source

-   **Origin:** Kaggle ([imports-exports-15000](https://www.kaggle.com/datasets/chakilamvishwas/imports-exports-15000))
-   **Format:** CSV (Tabular)
-   **Dimensions:** 15,000 rows x 16 columns

## Data Description

The dataset contains detailed records of individual import and export transactions. Each row represents a single transaction with the following attributes:

-   **Transaction_ID:** A unique identifier for each transaction.
-   **Country:** The country involved in the transaction.
-   **Product:** The type of product traded.
-   **Import_Export:** Indicates whether the transaction is an import or export.
-   **Quantity:** The quantity of the product traded.
-   **Value:** The total value of the transaction in dollars.
-   **Date:** The date of the transaction (DD-MM-YYYY).
-   **Category:** The category of the traded product (e.g., Machinery, Clothing, Electronics, Furniture, Toys).
-   **Port:** The port where the transaction occurred.
-   **Customs_Code:** A unique code assigned by customs authorities.
-   **Weight:** The total weight of the traded goods in kilograms.
-   **Shipping_Method:** The shipping method used (Air, Land, or Sea).
-   **Supplier:** The supplier of the traded goods.
-   **Customer:** The customer receiving the traded goods.
-   **Invoice_Number:** A unique identifier for the invoice.
-   **Payment_Terms:** The agreed payment terms (e.g., Cash on Delivery, Prepaid, Net 30, Net 60).

### Data Variable Types

-   **Numeric:** Quantity, Value, Customs_Code, Weight, Invoice_Number
-   **Non-Numeric:** Transaction_ID, Country, Product, Import_Export, Date, Category, Port, Shipping_Method, Supplier, Customer, Payment_Terms

### Data Variable Categories

-   **Index Variables:** Transaction_ID
-   **Categorical Variables:**
    -   **Nominal:** Country, Product, Import_Export, Category, Port, Shipping_Method, Supplier, Customer, Payment_Terms
    -   **Ordinal:** None explicitly identified.
-   **Non-Categorical Variables:** Quantity, Value, Customs_Code, Weight, Invoice_Number

## Data Pre-Processing

1.  **Missing Data Handling:** No missing values were found in the dataset.
2.  **Numerical Encoding:** Categorical variables (Import_Export, Category, Shipping_Method, Payment_Terms) were encoded into numerical representations.
3.  **Scaling:** Non-categorical variables (Quantity, Value, Weight) were scaled using normalization or standardization to ensure uniformity.
4.  **Combined Dataset:** Processed categorical and non-categorical data were combined into a unified dataset.

## Analysis Techniques

### Descriptive Statistics

-   Distribution analysis of categorical and non-categorical data.
-   Correlation analysis using Spearman, Kendall, and Pearson coefficients.
-   Evaluation of data dispersion (skewness, kurtosis) and variability (coefficient of variation).
-   Calculation of confidence intervals.

### Inferential Statistics

-   Chi-squared tests to find significant relationships between categorical variables.
-   Normality tests (Shapiro-Wilk, Kolmogorov-Smirnov, Anderson-Darling, Jarque-Bera) to assess data normality.
-   Correlation analysis with t-statistics and p-values.

### Unsupervised Learning

-   K-Means and Agglomerative Clustering.
-   Silhouette and Davies-Bouldin scores for cluster validation.

### Supervised Learning

-   Decision Tree, Logistic Regression, K-Nearest Neighbors (KNN), Naive Bayes, Support Vector Machine (SVM), Stochastic Gradient Descent (SGD).
-   Performance metrics: Accuracy, precision, recall, F1-score, confusion matrix, cross-validation.

### Ensemble Learning

-   Random Forest, Gradient Boosting, AdaBoost.
-   Evaluation metrics: Accuracy, precision, recall, F1-score.

### Model Run Statistics

-   Runtime analysis.
-   Memory usage analysis.

## Key Findings

-   **Data Quality:** Excellent, with no missing data.
-   **Categorical Data:** Balanced distribution across different categories.
-   **Non-Categorical Data:** Symmetrical distribution and minimal inter-variable relationships.
-   **Inferential Statistics:**
    -   Significant relationships: (Import_Export, Shipping_Method), (Shipping_Method, Payment_Terms).
    -   Non-normal data: Quantity, Value, Weight.
    -   Strong correlations: Weight with Quantity and Value.
-   **Clustering:** K-Means (4 clusters) preferred.
-   **Supervised Learning:** SVM achieved highest accuracy (36.36%). Logistic Regression performed well too (34.56%).
-   **Ensemble Learning:** Decision Tree outperformed Random Forest. Gradient Boosting and AdaBoost had similar accuracies.
-   **Model Run Statistics:** Naive Bayes and KNN were fastest. Naive Bayes had the lowest memory usage. XGBoost had the highest memory usage.

## Managerial Insights and Recommendations

-   Use tailored strategies for categorical data.
-   Use non-parametric methods for non-normal distributions.
-   Leverage the strong correlations between weight, quantity, and value.
-   Consider Logistic Regression as a baseline model.
-   Consider SVM for high accuracy, but pay attention to class imbalance.
-   Validate models using cross-validation.
-   Choose models based on computational resources:
    -   **Speed:** Naive Bayes, KNN.
    -   **Low Memory:** Naive Bayes.
    -   **High Performance:** XGBoost (with sufficient memory).

## Libraries Used

-   pandas
-   numpy
-   scikit-learn (sklearn)
-   matplotlib
-   seaborn
-   scipy
- statsmodels

## How to Run the Code

The code is available in a Google Colab notebook. To run the code:

1.  Open the Colab notebook.
2.  Run each cell sequentially.
3.  You may need to install the necessary libraries if you run it in a new environment. Instructions for installing the libraries will be included in the Colab notebook.

## Contact

-   Oishik Banerjee
-   055028

