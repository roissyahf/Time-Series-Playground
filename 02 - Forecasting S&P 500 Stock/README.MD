## Forecasting S&P 500 Stock with Deep Learning

This repository documents my experiments in forecasting the daily closing prices of a major stock index using simple RNN, LSTM, and Conv1D networks.

### Approach

1. Exploratory data analysis (EDA) to better understand the data characteristics and trends.
2. Windowing dataset, so it match with format needed for time series task.
2. Splitting dataset into train, validation, and test sets.
3. Reshaping `X_train`, `X_valid`, and `X_test`.
4. Training and Evaluating simple RNN networks.
5. Training and Evaluating LSTM networks.
6. Training and Evaluating the combination of Conv1D, MaxPooling1D, LSTM networks.
7. Comparing and analyzing the performance of the three models using $R^2$ as the main evaluation metric.

### Results

Simple RNN perform better than LSTM and Conv1D, because $R^2$ Score in train, validation, and test sets fall in 0.93-0.99. *Why do we use $R^2$ as the main evaluation metric? because when using data where the target variable has been scaled (as is common with time series data), a normalized metric like R-Squared may be more helpful since it is not affected by the scale of the data.*

### Future Work

Optimize the networks, solve `ValueError` when visualizing the result.