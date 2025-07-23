#  Customer Churn Analysis — Telecom Industry

 Predicting telecom customer churn using machine learning and exploratory analysis  


![Churn Overview](images/customer%20churn.webp)

---

##  Dataset Overview

The dataset includes 3,333 customers with features like:

-  `state`, `area code`, `phone number`
-  `total day minutes`, `total night calls`, `customer service calls`
-  `international plan`, `voice mail plan`
-  `churn`: Target variable (1 if customer left)

---
##  Business Objective

- **Goal**: Predict which customers are likely to churn and why.
- **Impact**: Allow telecom providers to target high-risk customers and reduce revenue loss.
- **Churn Rate**: ~14.5%

---

##  Exploratory Data Analysis (EDA)

### Churn by Plan

Customers with an **international plan** are more likely to churn:

![International Plan Churn](images/churn%20by%20international%20plan.png)

---

### Customer Service Calls vs Churn

Frequent contact with customer service is a strong churn indicator:

![Service Calls vs Churn](images/churn%20by%20customer%20service%20calls.png)

---

### Feature Correlation

A heatmap shows the correlation between numerical features and churn:

![Correlation Heatmap](images/correlation%20heatmap%20of%20numerical%20features.png)

---

##  Modeling & Evaluation

### Models Trained

- Logistic Regression
- Decision Tree Classifier
- Random Forest Classifier  (Best)

### Evaluation Metrics

| Model                | Accuracy | Precision | Recall | F1 Score |
|----------------------|----------|-----------|--------|----------|
| Logistic Regression  | 85%      | 50%       | 20%    | 28%      |
| Decision Tree        | 91%      | 55%       | 40%    | 46%      |
| **Random Forest**    | **94%**  | **70%**   | **58%**| **63%**  |

### Feature Importance (Random Forest)

![Feature Importance](images/random%20forest%20confusion%20matrix.png)

---

##  Key Insights

-  International plan users are ~2.5x more likely to churn.
-  Customers with 3+ service calls show high churn probability.
-  High total day minutes is common among churned users.

---

##  Recommendations

- Offer proactive service to international plan customers.
- Improve support for customers who call frequently.
- Introduce loyalty incentives for heavy users.

---


##  Project Workflow

```text
1. Business Understanding
2. Data Understanding
3. Data Cleaning & Encoding
4. Exploratory Data Analysis (EDA)
5. Modeling (LogReg, Tree, Random Forest)
6. Evaluation & Tuning
7. Findings & Recommendations
8. Conclusion

---
Prepared by:

Newton Muhato Njeri
newtonmuhato12@gmail.com