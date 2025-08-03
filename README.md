#Customer Churn Prediction

This project aims to analyze and predict customer churn behavior based on transactional and behavioral data. The goal is to identify key factors that drive churn and build a predictive model to help businesses retain customers.

---

##Dataset

The dataset used in this project contains various attributes related to customer activity, product subscriptions, power consumption, contract details, and churn status.

- **Rows**: Each row represents an individual customer
- **Target Variable**: `churn` (1 = churned, 0 = retained)
- **Features** include:
  - Customer demographics
  - Power and gas usage metrics
  - Subscription margins
  - Time-related metrics (tenure, contract updates, etc.)

---

##Project Pipeline

### 1.Exploratory Data Analysis (EDA)
- Checked for missing values and outliers
- Visualized churn distribution
- Analyzed correlations between features
- Category-wise churn trends
- Distribution and boxplots for numerical variables

### 2.Feature Engineering
- Created tenure-based features
- Encoded categorical columns
- Normalized numerical variables
- Engineered churn-driving segments
- Prepared final train/test sets

### 3.Modeling & Evaluation
- Applied Random Forest Classifier
- Used metrics: Accuracy, Precision, Recall, F1-Score
- Identified key churn predictors (margin, contract time)
- Visualized model performance

---

## Tech Stack & Libraries

- Python
- pandas, numpy
- matplotlib, seaborn(for visualization)
- scikit-learn

---
## Key Findings
Most churned users had low subscription margins and short tenure.

“Churn risk” increased significantly when customers had < 4 months tenure.

Random Forest Classifier performed well with interpretable results.

Business stakeholders can use margin & contract length to flag high-risk users.
