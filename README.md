# Arima-and-STR-stock_prediction
Description: i wanted to see the prediction of the stock of amazon using different models and observe the result, seeing which is more accurate 

skillset used: 
- Data cleaning of each dataset
- performing EDA (time series for volume in regards to amazon : month, weekday , day of the week)
- correlation between the 2 datasets
- splitting the dataset to train and test
- Decomposition of dataset (STR)
- Timeseries model:
  Auto Regressive Integrated Moving Average (ARIMA), Pure Forecast, TensorFlow neural network : Relu with Bootstrapping 

Datasets are found on kaggle
https://www.kaggle.com/datasets/borismarjanovic/price-volume-data-for-all-us-stocks-etfs
https://www.kaggle.com/datasets/varpit94/apple-stock-data-updated-till-22jun2021 (Apple stock data)

Libraries used: 
- Pandas
- numpy
- matplotlib
- seaborn
- sklearn.model_selection
- from statsmodels.tsa.seasonal import seasonal_decompose
- statsmodels.tsa.arima.model
- statsmodels.api
- tensorflow
- sklearn.preprocessing 
