# Project Motivation
To see the impact of proxmitiy to a the subway or suvway line has an impact on rental prices in Manhttan and Brooklyn. Our goal was to see if the opening and closing of subway line would impact the price of apartment rentals in the area. 

Used a combination of location and price data, to build model to predict whether apartments in Manhattan and Brooklyn will be above or below their neighborhood median rental price.


# Data and Data Processing
* Created a dataset using the following sources: 
  - subway entrances, stations and lines: NYC open data 
  - median rental prices: Zillow 
  - apartment sales: NYC department of  finance 
  - boundry analysis: Google API 
  
* Used the rental prices inforamtion from Zillow in Manhattan and Brooklyn to conert past sale prices of NYC apartments into rental prices. 
* Each apartment and  subway entrace/station had latitutde and longitude informaiton. Using the Google MAP API we were able to map the distance between each subway entrance to the apartments to measure the impact of proxmitity and the change in rent price. 
* Added in feature improatance of how many subways entrances were within .5 miles, .4 miles, .3 miles, .2 miles and .1 miles to each indiviudal apartment to see impact of proximity. 





