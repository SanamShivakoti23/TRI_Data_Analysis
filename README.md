# TRI_Data_Analysis

# Generic Information
The analysis that conducted basically focuses on examining data from the Toxic Release Inventory (TRI) database, where we examine chemicals across different states over five years. By analyzing this dataset, we aimed to identify the chemical release and its impact on the environment and how carcinogenic it is. This analysis gives the insight into carcinogenic factors, environmental effects, regulations regarding the chemical release, industries sectors and their impacts and measures that should be taken to pursue sustainable practices for the protection of public health.

# Problem Statement
For our various basic needs, we need goods which are manufactured in industry and these basic needs have become one part of our life. But along with that various chemicals are also released in the environment due to these chemicals. If these chemicals aren’t properly managed, they will have long-term damage and harm our surroundings and health. In this report we are looking at how much chemicals are being released in each state during the time span of five years. To stay in a healthy and fresh environment is a basic aspect for every human being.

# Background of the Study
The background of the study is basically rooted in the concern of chemical releases that are happening from industries and the effects those chemicals will have in the environment and public health. The dataset is from the Toxic Release Inventory (TRI) database, which is basically managed by EPA. It provides us the data of chemical releases across the United States. Our study dives into understanding if those chemical
releases are carcinogenic or not and the effects it will have on environmental surroundings. Afterall it is very necessary to understand the environmental surrounding we are living, to understand the land, air, and water we are using. Analyze the Toxic Release Inventory (TRI) data to better understand the distribution of all those chemical releases in various states.

# Finding the right model
After data cleaning and removing the outliers, the size of dataset was (312,313 rows, 30 columns). We will look at the steps we took to find the right model to predict all the total chemical releases that is based on the dataset. Excluded features that were irrelevant to prediction like: '104. TOTAL RELEASES','47. UNIT OF MEASURE','118. PROD_RATIO_OR_ ACTIVITY','measure of unit', '4. FACILITY NAME','7. COUNTY','8. ST','20. INDUSTRY SECTOR','55. 5.5.1A - RCRA C LANDFILL','59. 5.5.3A - RCRA SURFACE IM','103. 6.2 - TOTAL TRANSFER','116. PRODUCTION WSTE (8.1-8.7)','119. 8.9 - PRODUCTION RATIO','Total_Release_air'. And seperated the target feature i.e. 'Total_Release'. Data was split (80% training, 20% testing).

# Experiment with Random Forest Regression Model
A Random Forest model with 100 estimators was created by us, it was then trained on the training data, and then used it to make predictions. Model was evaluated by using metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and R-squared (R2).

The metrices output are mentioned below:
Random Forest Regression Metrics:
MSE: 0.0008846705192794322
RMSE: 0.029743411359146956
MAE: 0.0012597728063568475
R-squared (R2): 0.9991534419462672

# Experiment with Gradient Boosting Regression Model
Gradient Boosting Regression model was used as an alternative. The Gradient Boosting Model was created with hyperparameters to train on the training data and make predictions. Model was evaluated with the same metrics of the Random Forest model. 

The merices output are mentioned below:
Gradient Boosting Regression Metrics:
MSE: 0.0108
RMSE: 0.1041
MAE: 0.0367
R-squared (R2): 0.9896

# Model Comparison
# Results
The Gradient Boosting Regression model had performed better performance while comparing it to the Random Forest model. Evaluated it based on the results of lower MSE, RMSE, MAE, and higher R-squared (R2).

# Conclusion
The Gradient Boosting Regression model was our right model, and it was the suitable model for accurate predictions for this dataset. It showed good accuracy, there wasn’t any overfitting and it dealt with outliers, and it showed good generalization capability in our dataset.
