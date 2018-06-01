# corcorun_challenge
I started with EDA of the dataset and found out the following inferences
1. There are some columns which wouldn't help in the sales prediction like Ease_ment(empty), Address, Apartment Number, 
Total Units (it is sum of residential units and sommerical units)
2. There are a lot of missing values in Land Square feet and Gross Square feet, so the rows with empty values had to be removed as the price of the house would majory depend on these two factors
3. There were a lot of outliers in the Sale Price column (price being 0 and 10). So the rows having these sales price were removed as it would highly affect any machine learning algorithm. 

I have built two basic algorithms on the dataset namely linear regression and Xgboost. The reason to use inear Regression was to set a base line to check the accuracy. I have used Xgboost for Gradient Boosting. 

The parameter used for accuracy is explained variance score from sklearn to get an idea of the variance. The variance using Linear Regression was to be around 11% and using Xgboost about 13%.

