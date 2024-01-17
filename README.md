# MLP_RNN_models
This Python script demonstrates a time series forecasting task using Multilayer Neural Network (MLP) and Recurrent Neural Network (RNN) models on the Daily Minimum Temperature dataset.

Here's a summary of the code:

Data Loading and Preprocessing:
Downloads the Daily Minimum Temperature dataset and visualizes it over a 10-year period.
Normalizes the data using Min-Max scaling.

Time Series Forecasting Preparation:
Defines a function to create input-output pairs for time series forecasting.
Sets the look-back period to 20 days.

Model Training:
Creates MLP and RNN models using Keras.
Trains both models on the entire dataset for 100 epochs.

Model Predictions and Evaluation:
Obtains predictions on the entire dataset for both models.
Inverts the scaling to obtain temperature predictions in original units.
Evaluates model performance using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).

Plotting:
Visualizes the true values against predictions for both MLP and RNN models.
Plots predictions for the next 10 years for comparison.

Dynamic Time Warping (DTW):
Extracts predictions for the last 10 years from both models.
Calculates the Dynamic Time Warping (DTW) distance between MLP and RNN predictions using the fastdtw library.

Summary and Results:
Prints and compares MAE and RMSE for both models.
Displays plots of predictions and true values.
Calculates and prints the DTW distance between MLP and RNN predictions.

The code provides a comprehensive example of time series forecasting using neural networks, evaluates model performance, and employs Dynamic Time Warping to measure the similarity between predictions from different models.
