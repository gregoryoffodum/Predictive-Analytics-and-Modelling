# Price Prediction and Modeling of Used Cars

The [data set](https://github.com/gregoryoffodum/Price-Prediction-and-Modeling-of-Used-Cars/blob/main/Cars%20dataset.csv) is a list of second hand cars (a snapshot of the current situation at a second hand car sales website) with their respective price, type of body mileage, engine volume, engine type, production model and information about the time when they were registered. Each row comes from a different customer who was willing to sell their car through the platform.

## Objective

This project aims to create a model to predict price of second hand cars while considering relevant variables.

## Scope

- Predictive analytics
- Machine learning

## Introduction

According to Edmunds, an online automotive review site, approximately 40 million used vehicles are sold each year. The price of a used car depends on a variety of factors, this study aims at predicting the price of a used car depending on its specifications. 

The first potential aggressor is Brand, as it is well known that a BMW is generally more expensive than, say, a Toyota. Another relevant variable is mileage, since the more a car is driven, the cheaper it should be. “As mileage increases, so does wear and tear,” said Alec Gutierrez, Director, Product Management for Cox Automotive Inc. “It goes without saying that a potential purchaser would be less inclined to pay top dollar for a 200,000-mile car versus one with 30,000 miles.”

More so, the engine volume - sports cars have larger engines and economy cars have smaller engines. Year of production also impacts the price given that the older the car, the cheaper it is; of course, with the exception of vintage vehicles. The rest of the variables considered are categorical variables which will be dealt with on a case-by-case basis. View the full project [here](https://github.com/gregoryoffodum/Predictive-Analytics-and-Modelling/blob/main/Price%20Prediction%20and%20Modeling%20of%20Used%20Cars.ipynb).

## Methodology

The [study](https://github.com/gregoryoffodum/Predictive-Analytics-and-Modelling/blob/main/Price%20Prediction%20and%20Modeling%20of%20Used%20Cars.ipynb) followed the methodology as shown:


<img width="483" alt="Methodology" src="https://user-images.githubusercontent.com/78843321/156064207-9303bcf2-697d-4d6f-a7d3-8e08907487da.PNG">

## Results

<img width="585" alt="Predictions vs  Targets and Residuals PDF" src="https://user-images.githubusercontent.com/78843321/156066150-4503abb9-0238-41f1-8681-a196f0fa96c9.PNG">



- The model is better at predicting higher prices more than lower ones. i.e  From the Residuals PDF, the mean seems to be zero, however, there is a much longer tail on the negative side. Those predictions tend to overestimate the targets from the fact that there are no such observations on the right side, and we conclude that the predictions rarely underestimate the targets.
- An explanation may be that we are missing an important factor which drives the price of a used car lower. It may be that the car was damaged in some way, a piece of information we did not initially have.
- Adjusted R-squared value = 0.74358, therefore, the model explains 74% of the variability of the data.
- Mileage is the most prominent feature in this regression. It is more than twice as important as engine volume.
- The bigger the engine volume, the higher the price and vice-versa
- The more a car is being driven, the lower the price gets.
- Audi brand being benchmark for feature engineering. On average, if a car is a BMW, it will be more expensive than an Audi. Similarly, if a car is Mitsubishi, it will be cheaper than an Audi.
- Some recommendations for more accurate models include: Use a different set of variables. Remove a bigger part of the outlier observations. Use different kinds of transformations.




