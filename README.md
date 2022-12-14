# 02_LA_CarPricePrediction

## Project Description

The client company, which distributes automobiles, is developing an application for lead generation at the moment. The objective of data science project is to build a machine learning model for defining a car price in order to put a correct price to the app.

## Project Design

- Data quality evaluation, data pre-processing.
- As a quality metric we use RMSE.
- For modeling we use the Python library lightGBM for _gradient boosting_.
- For gradient boosting we use built-in Python library LightGBM.

### Features in the data

•	_DateCrawled_ — date of downloading the profile from the database

•	_VehicleType_ — vehicle body type

•	_RegistrationYear_ — year of vehicle registration

•	_Gearbox_ — type of gearbox

•	_Power_ — power (hp)

•	_Model_ — car model

•	_Kilometer_ — mileage (km)

•	_RegistrationMonth_ — month of vehicle registration

•	_FuelType_ — type of fuel

•	_Brand_ — car brand

•	_NotRepaired_ — Was the car under repair? Yes / No

•	_DateCreated_ — date of creation of the questionnaire

•	_NumberOfPictures_ — the number of photos of the car

•	_PostalCode_ — postal code of the owner of the questionnaire (user)

•	_LastSeen_ — date of last user activity

### Target 
Target is price (in euro)

## Project Outcomes
- The best advised model is Gradient Boosting lgb.Dataset()
- RMSE for validation data is 2248, while for test data is 2259, which are both less than agreed threshold 2500.
- Execution time 453 ms, which is the quickest model amonth all.
- CatBoostRegressor is also a good model (RMSE for validation data is the best comparing with DT, RF). But the exetution time for training is around 1 hour, which prevent to admit this as the best solution for business.

### Code: https://github.com/ybezginova2016/02_LA_CarPricePrediction/blob/main/car_price_main.ipynb
