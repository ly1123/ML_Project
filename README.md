# DS 1003 Machine Learning Project -- Build up Recommender System

In this project, we aims to implement recommendation systems that help Santander Bank to provide product recommendations based on their 1.5 years customers purchase historical records. We choose simple recommender, user-based recommender, random forest and XGBoost to make these recommendations.


# Dataset

https://www.kaggle.com/c/santander-product-recommendation

This dataset provides the monthly records of customer behavior data with 1.5 years period range from 1/28/2015 to 5/28/2016 including 24 demographic features such as ’Age’, ’Sex’, ’Customer code’ and 24 product features which are the names of the products like ’Guarantees’, ’Saving Account’ and ’Credit Card’ etc. We have a list of demographic information and the products owned for each individual in the period of the one and half years.

# Code

The code of this project are divided into 3 parts: Data Processing, User-based collaborative filtering, Multi-classification

### Data Processing:

- Data Processing .ipynb contains codes that clean and replace missing values for each column. We replace missing numerical - values with mean and for specical column such as income, we replace the missing value with mean income group by cities. For most categorical values we transfer their unique values to number categories. 

- Data Filter 2nd Ver.ipynb contains the data preparation code for next step analysis, including date filter and product sum group by customer id. 

### User-based collaborative filtering:

- User based Recommender.ipynb contains codes of data processing, popularity recommender and user-based similarity recommender.The evaluation functions including MAP (mean average precision) and hit rate are also included in this python notebook. 

### Multi-classification:

- Modeling_RF.ipynb	contains code using Random Forest as the classification model. 
- Modeling_xgboost.ipynb contains code of advanced customer filter and XGBoost model. A modified MAP and hit rate is also included. 

# Acknowledgement

This project was supported and advised by Bonnie Ray, who is the Vice President of Pegged Software and previous director of Cognitive Algorithms at IBM Research. We would like to express our thanks to her who provided insight and advice that greatly assisted this project.
