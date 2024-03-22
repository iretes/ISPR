# ISPR

## Midterm 1

### Assignment 2

Consider the following dataset: https://www.kaggle.com/datasets/imsparsh/single-chestmounted-accelerometer

It contains accelerometer timeseries for 15 participants performing 7 different physical activities.

For this assignement focus on a single activity (of your choice) and consider the 15 participants (timeseries) you have. Your goal is to see if there are similarities and differences in the behaviour of the accelerometers of these 15 participants. In other words, you need to see how they cluster. To achieve this goal,  you can use one of the techniques we have seen during the lecture, e.g.:
- Fit an autoregressive (ARMA) model for each participant and then compare them based on the values of their ARMA coefficients (alpha and beta values)
- Transform the timeseries in the Fourier domain and compare them on their power spectrum
- ... any other thing that makes sense ...
You don't need to do the actual clustering with a clustering algorithm, as soon as you can discuss similarities and differences of the "profiles" you have constructed.

Hint: If you opt for the autoregressive analysis, you can use the autoregressive model of your choice (AR, ARMA, ...). In Python, use the ARIMA class of the statsmodels library (e.g. set order=(3,0,0) for an AR of order 3); in Matlab you can use the ar function to fit the model and the forecast function to test.