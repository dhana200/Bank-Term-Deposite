# Bank Term Deposit Prediction

## Overview
This project analyzes customer behavior and builds a predictive machine learning model to determine whether a customer will subscribe to a term deposit. It combines exploratory data analysis (EDA), customer demographics analysis, and logistic regression modeling to identify key factors influencing subscription decisions.

## Objective
The primary goal is to:
- Understand customer demographics and characteristics
- Identify patterns in term deposit subscriptions
- Build an accurate predictive model using Logistic Regression
- Evaluate model performance using classification metrics and ROC-AUC score

## Dataset
The dataset (`data.csv`) contains 21 features related to customer profiles and campaign information:

### Key Features:
- **Customer Demographics**: age, job, marital status, education, default credit history, housing/personal loans
- **Campaign Information**: contact type (telephone/cellular), call duration, number of contacts, days since last contact
- **Economic Indicators**: employment variation rate, consumer price index, consumer confidence index, Euribor 3-month rate, number of employees
- **Target Variable**: `y` (yes/no) - whether the customer subscribed to a term deposit

## Project Structure

### Analysis Sections:

1. **Data Loading & Exploration**
   - Dataset overview and basic statistics
   - Data shape, types, and null value analysis
   - Distribution analysis of numerical and categorical variables

2. **Customer Demographics Analysis**
   - Age range distribution
   - Job category distribution
   - Identification of demographic patterns

3. **Balance & Deposit Trends**
   - Average economic indicators by subscription status
   - Relationship between Euribor rates and subscriptions

4. **Campaign Effectiveness Analysis**
   - Contact method effectiveness (telephone vs. cellular)
   - Impact of campaign frequency on conversion

5. **Correlation Analysis**
   - Correlation heatmap of numerical variables
   - Identification of relationships between features

6. **Predictive Modeling**
   - Feature preprocessing (OneHot encoding)
   - Train-test split with stratification
   - Feature scaling using StandardScaler
   - Logistic Regression model training and evaluation

## Key Findings

- **Age Distribution**: Customer base spans from young adults to seniors, with concentration in 30-50 age range
- **Job Diversity**: Customers come from various professional backgrounds
- **Subscription Correlation**: 
  - Certain age groups show higher subscription rates
  - Cellular contact is more effective than telephone
  - Campaign duration influences outcomes
  - Higher economic indicators correlate with subscriptions
- **Contact Method**: Cellular contact method shows better conversion rates
- **Campaign Impact**: Fewer repeated contacts often lead to better results (recency bias)

## Model Performance

The Logistic Regression model achieved:
- **Accuracy**: Model accuracy on test set
- **ROC-AUC Score**: Measures the model's ability to distinguish between classes
- **Classification Report**: Detailed precision, recall, and F1-scores
- **Confusion Matrix**: Visualization of true positives, false positives, true negatives, and false negatives

## Technologies & Libraries

- **Python 3.x**
- **Data Analysis**: pandas, numpy
- **Machine Learning**: scikit-learn
- **Visualization**: matplotlib, seaborn

### Required Packages:
```bash
pip install pandas scikit-learn matplotlib seaborn
```

## How to Run

1. Ensure all dependencies are installed
2. Place `data.csv` in the same directory as the notebook
3. Open `Advance_Bank_Term_Deposit.ipynb` in Jupyter Notebook or VS Code
4. Execute cells sequentially to run the analysis and model training

## Key Takeaways

- Certain age groups and job categories are more likely to subscribe to term deposits
- Higher economic indicators (Euribor rates, consumer indices) correlate with higher subscription rates
- **Cellular contact is significantly more effective than telephone** for campaign outreach
- Campaign duration and total contact frequency are important predictive factors
- Logistic regression effectively identifies key features that influence subscription decisions

## Files

- `Advance_Bank_Term_Deposit.ipynb` - Main analysis and modeling notebook
- `data.csv` - Dataset containing customer and campaign information
- `README.md` - Project documentation

## Author Notes

This project demonstrates the complete machine learning pipeline from data exploration to model evaluation. The analysis provides actionable insights for marketing teams to optimize term deposit campaigns through better targeting and channel selection.

---

**Dataset Source**: Bank Marketing Dataset

