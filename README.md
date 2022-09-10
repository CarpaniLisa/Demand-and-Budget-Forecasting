# Demand-and-Budget-Forecasting
Capstone 2 Codes
Demand forecasting is crucial to inventory management. The quantity of inventory on hand is determined by demand projections. In practise, inaccurate demand forecasts may lead to significant costs, which indicates that the procedure has not been improved. Many systems invest a lot of money on their inventory to avoid "stock-outs." The problem is made more difficult by the possibility that some demands are intermittent, meaning that a user may experience times of no demand and subsequent periods of desire.

This project is about time series forecasting for demand and budget planning for the automotive supply chain. It focuses on 3 top products which is BM, HIBE and PT.The project uses 3 time series forecasting models which is ARIMA, Holt Winters and LSTM and only concentrates on US as a country.

The models are run on 3 different datasets that is for 3 different products. Each model is run for amount and quantity variable of the dataset and the best result is selected as a preferred model for the dataset.

ARIMA -
-The dataset is loaded into the pandas dataframe
-Data is visualized
-ADF is run to check the stationary
-Differenciation of 2 is added to make the data stationary
-Data is split into train and test
-ARIMA model is run on the train dataset to make predictions for test dataset
-The model with the lowest AIC is selected as the preferred model
-Predictions are made with the test dataset to compare alongside
-RMSE is figured out to check the Accuracy of the model


Holt Winters -
-The dataset is loaded into the pandas dataframe
-Data is visualized
-Seasonal Decompose is done to check how the data looks
-Data is split into train and test
-Exponential Smoothing is run on the train data
-The HW model is run on the data
-Predictions are made with the test dataset to compare alongside
-RMSE is figured out to check the Accuracy of the model


LSTM -
-The dataset is loaded into the pandas dataframe
-Data is visualized
-Seasonal Decompose is done to check how the data looks
-Data is split into train and test
-MinMaxScaler to compress data into 0 and 1
-LSTM is run with 100 neurons for 50 epochs
-The best Epoch is selected for the model to run
-RMSE is calculated to check model accuracy
