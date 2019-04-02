# House-Prices---Ames
A model to predict  house prices with the help of various given features  by applying various regression algorithms. 
In the first step I treated the skewness of the numerical features and the target variable by taking logarithms of the features 
so that the variables have Normal Distribution. In the second step I treated the missing values, I filled the missing values in
numerical features by 0 in the appropriate places and by mean elsewhere. I then filled the missing values of categorical features
by 'None' and mode wherever appropriate. After there were no missing values left I converted all the categorical features to 
numerical features using pandas' get_dummies() funtion to get the data ready for modelling. Then I applied various regression 
techniques like ridge, lasso, lassoCV and Elastic Net and ensemble techniques like Random Forest and Gradient Boosting Regressor.
In the last step I calculated the final prediction by thaking the weighted means of the predictions of all the models. The weights
were assigned based on their porformance on the cross_val_score() metric.
