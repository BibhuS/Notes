# Multi-Linear Regression

**Note:** Please remember the below list of words in your mind before getting into the course   
	1. IV = Independent Variable (or) Predictor variable   
	2. DV = Dependent Variable (or) Response variable   
	3. SLR = Simple Linear Regression   
	4. MLR = Multi-Linear Regression (or) Multiple Linear Regression   

#### 1. Introduction
- Hello, Welcome to second part of Regression Models. I hope you might have an clear understanding of SLR and how to implement it in python. Lets move on to the next topic in Regression models. Today we are going to discuss about Multi-Linear Regression(MLR).
- We move from the SLR model with one predictor(Independent Variable) to the multiple linear regression model with two or more predictors(Independent Variable's).
- One good news here is that everything you learned about the SLR extends with minor modification in MLR. The key difference's between SLR and MLR are listed below
	- **Relationship:** SLR follows **One-to-One** Relationship between IV to DV, where-else MLR follows **Many-to-One** Relationship between IV's to DV.
- Lets see the concept of MLR using the following example [[Dataset.csv]](). In the dataset we have 3 IV's {Miles Traveled(<b>X<sub>1</sub></b>), NoOfDeliveries(<b>X<sub>2</sub></b>) and GasPrice(<b>X<sub>3</sub></b>)} and one DV {TravelTime(<b>Y</b>)}