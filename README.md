# Netflix Customer Data - EDA Assignment

### Name: Parth Lalit  
### University Roll No.: 2315200020  

---

## Objective

To explore and analyze a Netflix customer dataset and derive actionable insights related to user behavior, subscription patterns, and churn tendencies using Exploratory Data Analysis (EDA).

---

## Dataset Overview

- Source: Kaggle
- Rows: 5000
- Columns: 14

### Features Included

- Demographics: `age`, `gender`, `region`
- Account Info: `subscription_type`, `monthly_fee`, `number_of_profiles`, `payment_method`
- User Behavior: `watch_hours`, `avg_watch_time_per_day`, `last_login_days`, `device`, `favorite_genre`
- Target Variable: `churned` (0 = No, 1 = Yes)

---

## Task 1: Data Overview

- Displayed first 5 rows of the dataset
- Checked for missing/null values (none found)
- Listed unique values in columns like gender, region, subscription_type, etc.

The dataset is clean and ready for analysis.

---

## Task 2: Univariate Analysis

### Distribution Plots for Numerical Variables
- `age`, `watch_hours`, `monthly_fee`, `churned`

### Count Plots for Categorical Variables
- `subscription_type`, `gender`, `region`, `device`, `payment_method`, `favorite_genre`

This gave an overall idea of how different features are distributed.

---

## Task 3: Bivariate Analysis

### Compared Averages of
- `watch_hours` and `monthly_fee` across:
  - `subscription_type`
  - `region`
  - `device`

### Analyzed
- `avg_watch_time_per_day` by `favorite_genre`

### Churn Rate Analysis
- Grouped churn rate by:
  - `gender`
  - `region`
  - `subscription_type`
  - `payment_method`

This step helped identify patterns in engagement and churn tendencies across different customer groups.

---

## Task 4: Correlation Analysis

- Created a heatmap of correlation between numerical variables.
- Key observations:
  - `last_login_days` showed strong positive correlation with churn.
  - `watch_hours` and `avg_watch_time_per_day` had moderate negative correlation with churn.
  - `monthly_fee` had a weak positive correlation with churn.

These helped highlight strong potential predictors of churn.

---

## Key Insights

1. Customers with lower watch hours are more likely to churn. Less active users are at higher risk of cancellation.
2. Users who haven’t logged in for many days are significantly more likely to cancel their subscriptions.
3. Premium users tend to churn less compared to Basic plan users, showing higher commitment.
4. Customers in Africa have the highest average watch hours, indicating strong user engagement in that region.
5. Mobile device users tend to churn more than those who stream on TVs or laptops.
6. Users who pay via gift cards or cryptocurrency show a higher churn rate, possibly due to temporary subscriptions or low commitment.
7. Fans of Comedy and Drama tend to watch more consistently on a daily basis, suggesting higher content loyalty.

---

## Tools and Libraries Used

- Python
- Pandas
- Seaborn
- Matplotlib
- Google Colab

---
