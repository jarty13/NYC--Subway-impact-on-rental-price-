# Project Motivation
Measuring the impact of proximity to a subway line has on rental prices in Manhattan and Brooklyn. Our goal was to see if the opening and closing of the subway line would impact the price of apartment rentals in the area.

We used a combination of location and price data, to build a model to predict whether apartments in Manhattan and Brooklyn will be above or below their neighborhood median rental price.

We Evaluated predictions using different machine learning classifiers


# Data Processing
Created a dataset using the following sources:
* Location data for station entrances and line access from MTA's API
* Apartment sales from the NYC Department of Finance
* Median neighborhood rental prices and sale-to-rent ratios from Zillow
* Apartment coordinates from GoogleMaps API
* Used the rental prices information from Zillow in Manhattan and Brooklyn to convert past sale prices of NYC apartments into rental prices.
* Each apartment and subway entrance/station had latitude and longitude information. Using the GooglMap APIs we were able to map the distance between each subway entrance to the apartments to measure the impact of proximity and the change in rent price.
* Added in feature importance of how many subways entrances were within .5 miles, .4 miles, .3 miles, .2 miles and .1 miles to each individual apartment to see the impact of proximity.

# Data Exploration of Maping with GeoPandas

<img src="https://github.com/jarty13/NYC--Subway-impact-on-rental-price-/blob/master/data/Aparmtent%20sales%20.png" width="450" height="550">

<img src="https://github.com/jarty13/NYC--Subway-impact-on-rental-price-/blob/master/data/Subway%20%20map.png" width="450" height="550">


# Classifiers: 
- To predicting if an apartment will be priced above or below the median rental price based on proximity to subway. 

- Ran a grid search on each classifier to find the best hyperparameters.The following Classifiers were then fit to the training set.
  * Logistic Regression 
  * Random Forest 
  * Gradient Boosting 
  * Ada Boost 
 

# Results: 
Gradient Boosting had the best results resulting in an accuracy of 71% and AUC of %76
<img src="https://github.com/jarty13/NYC--Subway-impact-on-rental-price-/blob/master/data/Gradient%20Boosting%20Classifier.png" width="450" height="550">

# Next Steps: 
Due to time constraints, we were unable to get into the portion to look at the impact of opening and closing of subway lines on rental prices in Manhattan and NYC. This is something that we are looking into continuing for this project. 
