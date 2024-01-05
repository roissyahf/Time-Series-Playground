## Predicting Total Ticket Sales with Deep Learning

This repository documents my experiments in forecasting total sales using simple RNN and LSTM networks, using the daily cinema ticket sales dataset.

### Approach

1. Windowing dataset, so it match with format needed for time series task.
2. Splitting dataset into train and test sets.
3. Reshaping `X_train` and `X_test`.
4. Training and Evaluating simple RNN networks.
5. Training and Evaluating LSTM networks.
6. Comparing and analyzing the performance of the two models using MSE as the main evaluation metric.

### Results

* Simple RNN networks has MSE score in the train set: 0.016, in the test set: 0.019
* LSTM networks has MSE score in the train set: 0.015, in the test set: 0.020

These models are still bad considering the $R^2$ score for both model is still weak (0.48 for simple RNN, and 0.52 for LSTM). 

### Future Work

Tuning the hyperparameter for both model, or experiment with different architectures.

