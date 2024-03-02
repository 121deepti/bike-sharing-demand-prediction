# Bike_Sharing_Demand_Prediction
Currently rental bikes are introduced in many urban cities for the enhancement of mobility comfort. The purpose of this movement is to modernize cities and encourage people to head to a green world. Let's take the examples of Paris in 2007, where "velibs" were introduced and Amsterdam, where there are more bikes than cars. The goal is to facilitate the commute in the Seoul and reduce the amount of cars and the pollution. Indeed, the development of the way to commute reduced the use of cars to go to work and visit the city.

It is important to make the rental bike available and accessible to the public, as it provides many alternatives to commuters in metropolises. There are a lot of advantages to bike rents, it is convenient because it permits people not to keep the bike all day long, whether it is at work or at school. Furthermore it is the healthiest way to travel and it has many environmental benefits.

The studied dataset contains weather information which are the features (Temperature, Humidity, Wind speed, Visibility, Dew point, Solar radiation, Snowfall, Rainfall), the target is the number of bikes rented per hour and date information. The dataset presents the company's data between December the 1st of 2017 and finishes one year later.

# How many bikes are rented per hour in function of weather conditions ?
The goal of the company Seoul Bike is providing the city with a stable supply of rental bikes. It becomes a major concern to keep user satisfied. The crucial part is the prediction of bike count rents at each hour for a stable supply of rental bikes. We can suppose that this study could be reported to the company 'Seoul Bikes'. We think it could help them knowing if yes or not they have to supply bikes stations in the city, in order to keep a good satisfaction of the customers.

You can find the dataset necessary for the analysis on following link : https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand#

# Conclusion
EDA insights:
Most number of bikes are rented in the Summer season and the lowest in the winter season.
There is no bike demand on non Functioning day.
Most number of bikes are rented in the temperature range of 15 degrees to 30 degrees.
Most number of bikes are rented when there is no snowfall or rainfall.
Majority of the bikes are rented for a humidity percentage range of 30 to 70.
The highest number of bike rentals have been done in the 18th hour, i.e 6pm, and lowest in the 4th hour, i.e 4am.
Most of the bike rentals have been made when there is high visibility.


Results from ML models:
Random Forest Regression is the best performing model with an r2 score of 0.75.
Linear Regression,Lasso Regression(L1 regularization) and Ridge Regression are performing the same with an r2 score of 0.59.
Actual vs Prediction visualisation is done for all the 4 models with cv technique.
All 4 models have been explained with the help of SHAP library.
Temperature is the most important factor according to all the models.
