# House prices prediction
This is a comprehensive machine learning project that predicts house prices using multiple regression model. The project follows a complete data science workflow from exploration to model evalution

# Project Objective
Predict SalesPrices using various features in the [HousePricePrediction.xlsx](https://github.com/user-attachments/files/27623032/HousePricePrediction.xlsx)


# Project Workflow
# Phase 1: Data Exploration (EDA)
<img width="1200" height="600" alt="Correlation_heatmap" src="https://github.com/user-attachments/assets/284bd00f-e430-4382-b23e-23e670ac977f" />
Correlation heatmap shows relationships between numerical features. 

# Phase 2: Data cleaning
The dataset was cleaned removing all null values

# Phase 3: Feature Encoding
Because a machine model will be used, the categorical data needed to be converted to binary(0/1), so that the machine learrning model will understand and learn patterns in the data. 
OneHotEncoder was used on the concertion.

# Phase 4: Train_Test_split and model training
The dataset was split in a ratio of 1:4 for training where 1 = test data and 4 = train data. 
Three different machine learning models was train to know which has the least mean absolute percentage error.
Model 1: Sipport Vector Machines (SVM)
Results: Train MAPE: 0.1808 (18.08%)
          Test MAPE:  0.1871 (18.71%)

Model 2: Random Forest Regression
Results: Train MAPE: 0.0743 (7.43%)
         Test MAPE:  0.1887 (18.87%)

Model 3: Linear Regression
Results: Train MAPE: 0.1883 (18.83%)
         Test MAPE:  0.1874 (18.74%)

# Model Selection
Support Vector Machine
# Resosons
1. Lowest test MAPE (18.71%)
2. Minimal overfitting (train vs test gap < 1%)
3. Best generalization to unseen data

# Conclusion
The SVM model achieved a test MAPE of 18.71%, meaning predictions deviate by 18.7% on avarage.
