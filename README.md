Project Description:

This Google Colab project performs a comprehensive analysis of international trade transactions, examining both imports and exports. The core dataset comprises 15,000 transactions, each described by 16 variables, including details such as Transaction ID, Country, Product, Import/Export status, Quantity, Value, Date, Category, Port, Customs Code, Weight, Shipping Method, Supplier, Customer, Invoice Number, and Payment Terms.

Key Analytical Steps:

1.  Data Preprocessing:
    *   Missing Data Verification: Ensures the integrity of the dataset by confirming the absence of missing values.
    *   Categorical Encoding: Converts categorical variables into a numerical format for machine learning compatibility.
    *   Non-Categorical Scaling: Standardizes non-categorical variables (Quantity, Value, Weight) to a common scale.

2.  Descriptive Statistics:
    *   Categorical Analysis: Explores the distributions and proportions of key categorical variables (Import/Export, Category, Shipping Method, Payment Terms).
    *   Non-Categorical Analysis: Calculates measures of central tendency (mean, median, mode) and dispersion (range, standard deviation, skewness, kurtosis) for numerical variables (Quantity, Value, Weight).
    *   Correlation Analysis: Examines relationships among both categorical and non-categorical variables using appropriate correlation coefficients.

3.  Inferential Statistics:
    *   Categorical Variable Relationships: Employs Chi-squared tests to investigate associations between categorical variables.
    *   Normality Testing: Determines the normality of non-categorical variables using tests like Shapiro-Wilk.
    *   Correlation Significance: Analyzes the strength and significance of correlations between non-categorical variables.

4.  Unsupervised Learning:
    *   Clustering: Uses K-Means and Agglomerative clustering to group similar transactions.
    *   Cluster Evaluation: Evaluates cluster quality using Silhouette and Davies-Bouldin scores.

5.  Supervised Learning:
    *   Classification Models: Builds Decision Tree and Logistic Regression models to classify transactions.
    *   Performance Metrics: Assesses model performance using accuracy, precision, recall, and F1-score.

6. Ensemble Learning:
    * Classification Models: Uses Random Forest, Gradient Boosting, and AdaBoost to classify transactions.
    * Performance Metrics: Assesses model performance using accuracy, precision, recall, and F1-score.

Overall Project Goal:

The primary goal is to derive actionable insights from international trade data. This involves understanding trade patterns, identifying relationships between different trade factors, and developing predictive models to classify transactions effectively. The project uses a diverse set of methods, including data preprocessing, descriptive and inferential statistics, unsupervised learning (clustering), supervised learning (classification), and even ensemble methods to achieve these objectives.
