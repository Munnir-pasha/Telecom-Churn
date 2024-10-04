# Telecom Churn Case Study

## Problem Statement

### Business Problem Overview
In the telecom industry, customers can switch between service providers, leading to an average annual churn rate of 15-25%. Retaining existing customers, especially high-value ones, is more cost-effective than acquiring new ones. This project aims to predict which customers are at high risk of churn.

### Understanding and Defining Churn
There are two primary payment models:
- **Postpaid:** Customers are billed monthly/annually, and churn is easily identifiable when services are terminated.
- **Prepaid:** Customers can stop using services without notice, making churn more difficult to identify.

This project focuses on the prepaid model, particularly in the Indian and Southeast Asian markets, where churn prediction is more complex.

### Definitions of Churn
- **Revenue-based churn:** Customers who have not used any revenue-generating services.
- **Usage-based churn:** Customers with zero outgoing or incoming usage over a defined period. This is the definition used for this project.

### High-Value Churn
About 80% of telecom revenue comes from 20% of high-value customers. Reducing churn in this group can significantly impact revenue.

---

## Understanding the Business Objective and Data

The dataset contains customer information over four months (June to September), with the goal of predicting churn in the final month based on the first three months of data.

### Understanding Customer Behaviour During Churn
Customer churn happens gradually:
1. **Good Phase:** Customer is happy.
2. **Action Phase:** Customer is dissatisfied but hasn’t switched yet.
3. **Churn Phase:** Customer has stopped using the service.

The first two months are the "good" phase, the third is the "action" phase, and the fourth is the "churn" phase.

---

## Dataset and Data Dictionary

The dataset includes various customer usage metrics across months, labeled with 6 (June), 7 (July), 8 (August), and 9 (September). The data dictionary explains common abbreviations like `IC` (incoming), `OG` (outgoing), `RECH` (recharge), etc.
## Dataset

The dataset used for this project can be downloaded from the following link:

[Download the file](Data+Dictionary-+Telecom+Churn+Case+Study (2) (1).xlsx)

### Data Preparation
1. **Derive New Features:** Use domain knowledge to create features that indicate churn.
2. **Filter High-Value Customers:** Define high-value customers as those whose recharge amount in the first two months exceeds the 70th percentile.
3. **Tag Churners:** Label customers who have not made any calls or used mobile internet in the churn phase as churned.
4. **Remove Churn Phase Data:** After tagging churners, remove all churn phase data.

---

## Modelling

### Model Objectives
1. **Predict churn:** Identify high-value customers at risk of churning.
2. **Identify churn predictors:** Understand the key variables leading to churn.

### Suggested Modelling Steps:
- Preprocess data.
- Conduct exploratory analysis.
- Derive new features.
- Use **PCA** to reduce dimensionality and handle class imbalance.
- Train multiple models, tune hyperparameters, and evaluate with metrics focused on churn prediction accuracy.

### Handling Class Imbalance
Given that churn rates are low (5-10%), use techniques like oversampling/undersampling or SMOTE to handle class imbalance.

### Model Evaluation
Use evaluation metrics that prioritize identifying churners over non-churners, as the business goal is to reduce churn.

---

## Feature Importance
To identify important features, use logistic regression or tree-based models, which can reveal key indicators of churn. Ensure to handle multicollinearity in the data.

### Visualization and Insights
Once important predictors are identified, use visualizations like bar plots or summary tables to present findings clearly. This helps the business understand which factors are most predictive of churn.

---

## Recommendations
Based on the analysis, recommend strategies to prevent customer churn, such as offering competitive plans to high-risk customers or improving service quality.
