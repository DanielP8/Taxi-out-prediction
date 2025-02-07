# Taxi-out-prediction
Context:
This data was scraped under a Academic Paper under Review by IEEE transportation

Content:
Using data from JFK airport from Nov 2019-Dec-2020, predict 'taxi-out' time of a flight using multiple linear regression with sci-kit learn. 'Taxi-out' time is how long a plane spends moving between it's gate and the runway before takeoff. Taxi-out time can impact the cost of the flight.

# Framing the problem
1. 'Taxi-out' is our labelled target variable, the one we are trying to predict. All the rest are input variables, or features, used to predict taxi-out time.
2. I will use multiple linear regression to minimise our cost function and then calculate R^2 (as well as MSE, MAE and RMSE), which measures how well our input variables measure the variance in our target variable, taxi-out time. 
3. I will then use L1 and L2 regularization to assess if different levels of alpha improve our performance metrics.
4. I will finish by using cross-validation to repeat these tests with 10-fold cross-validation to see if our first performance metrics are accurate. A low standard deviation between different folds means our R^2 is consistent across folds, and therefore the mean of our fold R^2 should be accurate.
5. I will also use RMSE and MAE to compare the performance of our models, measuring the variance in our predictions.
6. I will use GridSearchCV to find the optimal alpha value for L1 and L2 regularization.
