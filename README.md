# Prediction on Grocery Sales
sales predictions
* Author: Raged Aou
* coding dojo 03/05/2022

![image](https://res.cloudinary.com/mommy-nearest/image/upload/c_crop,h_800,w_1800,x_0,y_675/c_scale,f_auto,fl_lossy,q_75,w_848/pyoluqa7wayuecdihqyx)

## Project Descrption
BigMart have recopiled information that has great value to identify the sales of each outlet . Also, information about products . we are going to build a predictive model that helps sales of each product at a particular outlet.

Using this model, BigMart will try to understand the properties of products and outlets which play a key role in increasing sales.
This Project is also identefy the sales in this outlets and to predicton and improve better results

## Data source 

The data was sourced from analyticsvidhya.com
* 8523 rows 
* 12 columns. 
*  11 features  
*  1 target variable.

## The Company 

* The company has 10 outlet stores.
* The first outlet store was opened in 1985, and the most recent in 2009.
* The company offers 1559 items across a total of 16 product category types.
* The total sales for the period was $18,591,125.41.


## Here is the Data Dictionary for this dataset:
![image](https://user-images.githubusercontent.com/98135268/157154600-7027e4c5-20aa-4837-947f-0ce4630f61e1.png)


# ANALISIS
 1. Visibility in the outlets can increase the sales ?
 
 ![image](https://user-images.githubusercontent.com/98135268/157155231-f2b84e10-b334-4911-89f1-7ea4d29826ba.png)
 
 
 
 
 ## Visibility 
 Visibility is conected to sales, they are many ways to make a product more atractive, here we provide some tips:
 
 * Appeal to the five senses.
 * better Organization 
 * use resorce like technologys
 * costumers service
 
 
## HEALTHY SALES MORE


 ![download (8)](https://user-images.githubusercontent.com/98135268/199262658-f17ba8de-c703-43cb-b94e-0a38a7d3876c.png)
 
 Low Fat items may have contributed the more significantly to Total Company Sales than Regular items
 
 
 ## What about health proteins??
 

![image](https://user-images.githubusercontent.com/98135268/157155434-49b8a2e3-f4b0-481b-88c1-3abee5286182.png)

Seafood is one of the best proteins in the market, with more nutricions and less fat, that has unlimited benefits to the health of the humans

realizing that 
why this healthy products is not in the top of our chart ?
if low fat(healthy products) has more sales that regular why we dont see seafood of one of the best seller 

marketing problem?
visualization of that item ?
maybe both?



## projecting with machine learning

# Machine Learning

| MODEL | MAE | MSE | RMSE | R2 | train or test |
|-------| --- | --- | ---- | -- | ------------- |
|LINEAR REGRESSION | 848.81 | 1,303,646.20 | 1,141.77  | 0.56| TRAIN |
|LINEAR REGRESSION | 804.65 | 1,193,827.69 | 1,092.62  | 0.57| TEST |


## VS

| MODEL | MAE | MSE | RMSE | R2 | train or test |
|-------| --- | --- | ---- | -- | ------------- |
|RANDOM FOREST | 755.40  | 1,152,595.69|  1,073.59  |  0.61 | TRAIN |
|RANDOM FOREST | 728.41 | 1,096,375.02 | 1,047.08   |  0.60 | TEST |





4. baggintree in acction


| MODEL | SCORE | TRAIN OR TEST |
| ----- | ----- | ------------- |
| BAGGINTREE| 0.91 | TRAIN |
| BAGGINTREE | 0.53 | TEST |



 ## lets Understanding these 
 
 
 
 ### Mean Absolute Error(MAE)
 MAE is the arithmetic average (mean) of the absolute errors
 
 #### Advantages:

* It prevents positive (+) and negative (-) errors from canceling out.

* It has the same units of measure as the target.

### Mean Squared Error (MSE)
 
 MSE is the arithmetic average (mean) of the squared errors 
 
 #### Advantages:

* It prevents positive (+) and negative (-) errors from canceling out.

* It punishes large errors.

#### Disadvantages:

* It does not have the same units of measure as the target.


### Root-Mean Squared Error (RMSE)

RMSE is the square root of MSE, and is probably the most-useful and a better metric than MAE, MSE, and RMSE.

#### Advantages:

* It prevents positive (+) and negative (-) errors from canceling out.
* It punishes large errors.
* It has the same units of measure as the target.


### Coefficient of Determination R2

The  Coefficient of Determination R2 is the proportion (%) of the variation in the dependent variable, or target variable, that a model is able to predict, or explain, from the independent variables, or features. It is a measure of the goodness of fit of a regression model.  calculates how much better our model's predictions are vs if the mean was used instead. It should have a value between 0 and 1, however a poor model may have a negative .

#### Advantages:

It uses a consistent scale, which is used for all datasets, and thus may be used for comparison.

#### Disadvantages:

* It is difficult to interpret and very difficult to explain to non-technical audiences.
* A high  doesn’t always mean a good model and a low score doesn’t always mean a bad one.
