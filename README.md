# Housing_Price_Estimation
House Price Prediction Using Tree-Based Models
This project demonstrates the use of tree-based models (Decision Trees and Random Forests) for predicting house prices using the House Price dataset from Kaggle. The dataset contains various features such as the size, location, and condition of houses, which are used to predict their selling prices. We train the models to predict the sales price of houses using these features, after performing exploratory data analysis (EDA) and data preprocessing.

Highlights:
Data Preprocessing: Handling missing data, feature scaling, and one-hot encoding.
Models: Decision Trees and Random Forests.
Hyperparameter Tuning: Grid Search for optimal Decision Tree parameters.
Model Evaluation: R-squared, MSE, and RMSE for model performance.
Feature Importance: Visualizing the most important features.

Data Preprocessing
The dataset contains both categorical and numerical columns. Preprocessing includes:

Imputation: Filling missing values using median for numerical columns and the most frequent value for categorical columns.
Scaling: Standardizing numerical columns.
Encoding: One-hot encoding categorical columns.

Modeling
Decision Tree
A basic Decision Tree Regressor is trained and evaluated using R-squared, MSE, and RMSE metrics. Hyperparameter tuning is performed using GridSearchCV for optimizing the max_depth and min_samples_leaf.

Random Forest
The Random Forest model is trained on the preprocessed data. It is an ensemble of decision trees and generally provides better performance by reducing overfitting. Feature importance is extracted from the model to analyze which features are most influential in predicting house prices.

Feature Importance
The Random Forest model provides feature importance scores for each feature. The top 10 most important features are visualized using a bar plot, which helps understand the impact of various features on the prediction model.

Results
Decision Tree:
R-squared: 0.82
MSE: 1248962759.19
RMSE: 35340.67

Random Forest:
R-squared: 0.83
MSE: 1152807301.30
RMSE: 33953.02

Visualizations
The project includes several visualizations:
Missing Data: A bar chart showing columns with the highest number of missing values.
Decision Tree: Visualization of the decision tree structure.
Actual vs Predicted: A scatter plot comparing actual vs predicted house prices for validation data.
Feature Importance: Bar plot showing the top 10 most important features in the Random Forest model.
