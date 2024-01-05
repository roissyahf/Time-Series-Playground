## Forecasting Temperature with Deep Learning

This repository documents my experiments in forecasting the Temperature in Celcius degree using only 1 feature (with date time range in 10 minutes) using LSTM and 5 features (with date time range in one hour) using Simple RNN networks.

### Approach

1. Exploratory data analysis (EDA) to better understand the data characteristics and trends.
2. For `UnivariateTimeSeries-Forecasting_Temperature_Using_5_features.ipynb`, I conduct feature engineering to produce 4 new variables from the extracted second using sin cos transformation.
3. Windowing dataset to make time series data into the form of supervised learning data.
4. Splitting dataset into train, validation, and test sets.
5. Training and Evaluating the networks.
6. Analyzing the performance of the model using RMSE, then visualizing the results.

### Results

In this experimentation, I only used one model so there will be no model comparison. Using one feature, RMSE score in the three sets are as follow: 0.241, 0.251, 0.233. On the other hand, while using five features I obtained these RMSE score in the three sets: 0.731, 0.741, 0.686.

We might guess, forecasting temperature using only one feature is better than using five features as the network produce smaller error. But, we can't make that conclusion because they're treated differently. I didn't conduct any scaling technique in the first forecasting case, meanwhile for the second case I have to scale the variables because they're ranging in different interval. Thus, based on this facts we still can't conclude which experiment is better.


### Future Work

Read more literatures to make conclusion.