# Precipitation-prediction-Rainfall

Precipitation prediction based on weather data like wet bulb temp, dry bulb temp, visibility, humidity, wind speed etc. containing 100,000 observations for location Kansas City-downtown airport. Applied univariate multiple regression splines using EARTH package in R. Data collected from NOAA. Achieved an accuracy of 86.33% and best model selected 9 out of 10 predictors

Environment: Windows, RStudio, Earth Package
R language

FEATURES
Regression splines are a flexible class of basis functions that extends over piecewise constant regression and polynomial regression.
Selected EARTH package to implement Multivariate Adaptive Regression Spline (MARS) and used cubic spline with hinge base non-parametric approach.
Stratified Cross-validation method for accurate estimates and degree 2 correlation for including interaction terms.
Minimized overfitting by cross validation method rather than forward and backward selection methods.
Performance is calculated by CVR2,CVRSS,gR2, mean absolute accuracy percentage. With huge data and complex model, calculated accuracy is relatively high.
Cross validation scheme to give appropriate test accuracy.

Input data: 
Predictors = Precipitation, Visibility, Dry bulb Temp, Wet bulb Temp, Humidity, Wind speed, Station Pressure, Sea-level Pressure, Altimeter setting, Wind Direction etc.,  
No. of observations = ~1,00,000
Datasource: https://www.ncdc.noaa.gov/cdo-web/datasets

Results:
Generalized R2 approximately equal to test R2, out of fold cross validation R2 is close to actual test R2,  max gR2, max CVR2 and selected model are close to each other.

gR2=0.294 ; 

CVR2=0.259 ; 

Standard Deviation=0.0614 ;

Mean absolute prediction accuracy = 86.33%

Residual Sum of Squares = 71.92 