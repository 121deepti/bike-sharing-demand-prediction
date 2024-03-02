# Bike_Sharing_Demand_Prediction
Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

# How many bikes are rented per hour in function of weather conditions ?
The goal of the company Seoul Bike is providing the city with a stable supply of rental bikes. It becomes a major concern to keep user satisfied. The crucial part is the prediction of bike count rents at each hour for a stable supply of rental bikes. We can suppose that this study could be reported to the company 'Seoul Bikes'. We think it could help them knowing if yes or not they have to supply bikes stations in the city, in order to keep a good satisfaction of the customers.

# Describing DataSet
The dataset contains weather information (Temperature, Humidity, Windspeed, Visibility, Dewpoint, Solar radiation, Snowfall, Rainfall), the number of bikes rented per hour and date information.

## Attribute Information:
Date : year-month-day
Rented_Bike_Count - Count of bikes rented at each hour
Hour - Hour of he day
Temperature-Temperature in Celsius
Humidity - %
Windspeed - m/s
Visibility - 10m
Dew point temperature - Celsius
Solar radiation - MJ/m2
Rainfall - mm
Snowfall - cm
Seasons - Winter, Spring, Summer, Autumn
Holiday - Holiday/No holiday
Functional Day - NoFunc(Non Functional Hours), Fun(Functional hours)
# Conclusion
**EDA insights**:
Most number of bikes are rented in the **Summer season** and the **lowest in the winter season**.
There is **no bike demand** on **non Functioning day**.
Most number of bikes are rented in the **temperature** range of **15 degrees to 30 degrees**.
Most number of bikes are **rented** when there is **no snowfall or rainfall**.
Majority of the bikes are rented for a **humidity percentage** range of **30 to 70**.
The **highest** number of bike rentals have been done in the **18th hour**, i.e 6pm, and **lowest** in the **4th hour**, i.e 4am.
Most of the bike rentals have been made when there is **high visibility**.

**Results from ML models:**
**Random Forest Regression** is the best performing model with an **r2 score** of **0.75**.
Linear Regression,Lasso Regression(L1 regularization) and Ridge Regression are performing the same with an r2 score of 0.59.
Actual vs Prediction visualisation is done for all the 4 models with cv technique.
All 4 models have been explained with the help of SHAP library.
**Temperature** is the most important factor according to all the models.
