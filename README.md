# DATA SCIENCE JOB SIMULATION BCG X

I completed an 8-hour professional simulation for BCG X, where the focus was on addressing the needs of PowerCo, a leading provider of gas and electricity services for small and medium-sized businesses.

The main challenge PowerCo faces is customer churn—clients leaving in search of better offers from other energy providers. They have partnered with BCG to identify the underlying reasons why their customers are discontinuing their services.


## Use a 5-Step Methodology in Data Science to Tackle the Job:

- Business understanding and problem formulation: What is the context of this problem and why are they trying to solve it?

- Exploratory data analysis and data cleaning: What data are we working with, what is it like, and how can we improve it?

- Feature engineering: Can we enrich this dataset using our own expertise or third-party information?

- Modeling and evaluation: Can we use this dataset to make accurate predictions? If so, are they reliable?



Overview
In this professional simulation, three Jupyter notebooks were developed to showcase the results:

## 1st Notebook: BCG_explore
The client provided more than three datasets:

- Historical Customer Data: includes usage, registration date, forecasted consumption, etc.
- Historical Price Data: includes variable and fixed price information.
- Churn Indicator: whether each customer has churned or not.
- As the first step, an Exploratory Data Analysis (EDA) was conducted to understand and visualize these datasets.

## 2nd Notebook: feature_engineer
The client proposed the following idea:
“I believe that the difference between off-peak prices in December and January of the previous year could be an important feature for predicting customer churn.”

In this notebook, we applied feature engineering to create new columns aimed at improving churn prediction accuracy.

## 3er Cuaderno: model_predictions
We generate and train a prediction model using a random forest to predict customer churn.

## Python Libraries Used:

- Pandas: To read, clean and transform structured data
- Scikit-learn: We use this library to create and train models such as random forests or logistic regression.
- Numpy: For mathematical operations and array manipulation.
- Matplotlib: For data visualization.
- Seaborn: For advanced data visualization.

# Conclusions 
  The 20% discount strategy is effective, but only offer discount only to customers with more than 12 months and value customers
  with high probability of abandonment

  - Performance of a classification model

    - Overall model performance
      -  Accuracy: The model has an overall accuracy of 90%, meaning it correctly classifies 90% of the samples in the test set. However, high precision can be              misleading due to class imbalance (many more customers do not churn than churn).
    - Class 0 (customers who DO NOT abandon)
      -  Precision: 0.90, i.e. 90% of "non-churn" predictions are correct.
      -  Recall: 1.00, which means the model correctly identifies all non-churning customers.
      -  F1-Score: 0.95, indicating an excellent balance between precision and recall for this class.
    - Class 1 (customers who DO abandon)
      -  Precision: 0.71, 71% of "abandonment" predictions are correct.
      -  Recall: 0.05, indicating that the model only correctly identifies 5% of customers who actually abandon.
      -  F1-Score: 0.10, reflecting poor overall performance in this class.
    - Identified problems
      -  Class imbalance: There is a large imbalance in the data (3286 in class 0 and only 366 in class 1). This causes the model to be biased towards the majority          class (customers who do not churn).
      -  Poor recovery for class 1: The model is unable to correctly capture churning customers (recall of 0.05), which makes it little useful for predicting churn,         which is the main objective.
    - Possible solutions
      -  To improve the performance of the model in the minority class (churning customers):

Collecting more data: If possible, include more examples of customers who drop out to balance classes.

## This project demonstrates the use of data analysis, feature engineering, and machine learning techniques to enhance customer retention prediction.
