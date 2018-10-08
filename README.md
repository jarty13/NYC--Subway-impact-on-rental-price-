# Project Motivation
To see the impact of proxmitiy to a subway line has on rental prices in Manhttan and Brooklyn. Our goal was to see if the opening and closing of subway line would impact the price of apartment rentals in the area. 

Used a combination of location and price data, to build model to predict whether apartments in Manhattan and Brooklyn will be above or below their neighborhood median rental price.


# Data Processing
* Created a dataset using the following sources: 
  - Subway entrances, stations and lines: NYC open data 
  - Median rental prices: Zillow 
  - Apartment sales: NYC Department of Finance 
  - Boundry analysis: Google API 
  
* Used the rental prices inforamtion from Zillow in Manhattan and Brooklyn to conert past sale prices of NYC apartments into rental prices. 
* Each apartment and  subway entrace/station had latitutde and longitude informaiton. Using the Google MAP API we were able to map the distance between each subway entrance to the apartments to measure the impact of proxmitity and the change in rent price. 
* Added in feature improatance of how many subways entrances were within .5 miles, .4 miles, .3 miles, .2 miles and .1 miles to each indiviudal apartment to see impact of proximity. 

# Data Exploration of Maping with GeoPandas

<img src="https://github.com/jarty13/NYC--Subway-impact-on-rental-price-/blob/master/data/Aparmtent%20sales%20.png" width="450" height="550">

<img src="https://github.com/jarty13/NYC--Subway-impact-on-rental-price-/blob/master/data/Subway%20%20map.png" width="450" height="550">


# Models Built: 
- To predicting if an apartment will be priced above or below the median rental price based on proximity to subway. 

- Ran a grid search on each classifier to find the best hyperparatmers. Each Classifer was than fit to the training set using the following Classifiers:
  * Logistic Regression 
  * Random Forest 
  * Gradient Boosting 
  * Ada Boost 

# Results: 
Gradient Boosting had the best results resulting in an accuracy of 71% and AUC of %76
<img src="https://github.com/jarty13/NYC--Subway-impact-on-rental-price-/blob/master/data/Gradient%20Boosting%20Classifier.png" width="450" height="550">

# Next Steps: 
Due to time constraints, we were unable to get into the poriton to look at the impact of opening and closing of subway lines on rental prices in Manhattan and NYC. This is something that we are looking into conitnuing for this project. 
