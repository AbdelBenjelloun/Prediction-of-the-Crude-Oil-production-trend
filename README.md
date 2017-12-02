# Prediction of the Crude Oil production trend

Task : The challenge consists on predicting the Crude Oil production’s trend based on the previous year CrudeOil data.
More precisely given a set of historical data collected by “The Joint Organisations Data Initiative(JODI)” 
we would like to know if the production will grow or not.

Data : The dataset contains 123 features : 'closing stocks', 'exports/imports', 'refinery intake', 'West texas Intermediate Price', 'sum closing', 
'sum exports' and 'sum imports' for 12 months for a selected country (76 in total). 

The countries name are integers and the selected months are given however we do not know to which year they belong to. 

The size of training data is 10159 while the size of test data is 2000. 

In addition we observe that we have a balanced number of data point per month (~836 per month) and per country (~134 per country).

In our study, we deal with the missing values, and visualize the dataset (per month, and country). 

We perform several classification algorithms (Random Trees, K-NN, Extra-Trees, Gradient Boosting, XGBoost, SVM : rbf, linear and sigmoid). 

We got the best performance using XGBoost, we finetunne the parameters of XGBoost as a post-processing step.
