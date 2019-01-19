# Simple Linear Regression

### Introduction
- Simple linear regression is a statistical method that allows us to summarize and study relationships(trend) between two continuous (quantitative) variables.
- We are going to learn the concept and basic procedures of simple linear regression.
- We will also learn two measures that describe the strength of the linear association that we find in data.

###### Notes:    
  SLR -> Simple Linear Regression    
  MLR -> Multi Linear Regression    
  [Formula to find Mean](https://github.com/ManikandanJeyabal/Workplace/blob/master/DataScience/Formulas/Mean.JPG?raw=true)    
  [Formula to find Median](https://github.com/ManikandanJeyabal/Workplace/blob/master/DataScience/Formulas/Median.JPG?raw=true)

### What is Simple Linear Regression?
- As we seen earlier in introduction SLR is known as the following,
	- Simple linear regression is a statistical method that allows us to summarize and study relationships(trend) between two continuous (quantitative) variables.
	- One variable, denoted **X**, is regarded as the **predictor**, **explanatory**, or **independent variable**.
	- The other variable, denoted **y**, is regarded as the **response**, **outcome**, or **dependent variable**.
- SLR gets its adjective "simple," because it concerns the study of only one predictor variable.
- A simple key difference between SLR and MLR, is MLR gets its adjective "multiple," because it concerns the study of  two or more predictor variables.


### Types of Relationships:
- There are two types of relationships available one is  **deterministic (or functional) relationships** and second one is **statistical relationships**, simple linear regression will deals with second one.
	
###### Deterministic (or Functional) Relationships:
- one of the simple example to define deterministic relationship is the relationship between Celsius and Fahrenheit.
- Please find the below data points to understand the relationship.
- In deterministic relationships, the equation exactly describes the relationship between the two variables.

<p align="center">
  <img width="500" height="333" src="https://newonlinecourses.science.psu.edu/stat501/sites/onlinecourses.science.psu.edu.stat501/files/01simple/temps/index.jpg">
</p>
	

- Note that the observed (x, y) data points fall directly on a line. As you may remember, the relationship between degrees Fahrenheit and degrees Celsius is known to be:

<p align="center">
	<b>Fahr = 9/5 Cels + 32</b><br>
</p>

-  If you know the temperature in degrees Celsius, you can use this equation to determine the temperature in degrees Fahrenheit exactly.
- For each of these deterministic relationships, the equation exactly describes the relationship between the two variables.
- Some other examples of deterministic relationships:    
  - Circumference = π × diameter

###### Statistical Relationships:
- In statistical relationship, the relationship between the variables is not perfect.
- The below example illustrate the relationship between response variable y is the mortality due to skin cancer (number of deaths per 10 million people) and the predictor variable x is the latitude (degrees North) at the center of each of 49 states in the U.S. [(dataset.txt)](https://newonlinecourses.science.psu.edu/stat501/sites/onlinecourses.science.psu.edu.stat501/files/data/skincancer/index.txt)    
  <p align="center">
  	<img width="502" height="333" src="https://newonlinecourses.science.psu.edu/stat501/sites/onlinecourses.science.psu.edu.stat501/files/01simple/scatterplot_skin_cancer/index.png">
  </p>
- The above plot appears to be a negative linear relationship between latitude and mortality due to skin cancer, but the relationship is not perfect.
- Indeed, the plot exhibits some "trend," but it also exhibits some "scatter." Therefore, it is a statistical relationship, not a deterministic one.
- Based on the above observation if you lived in the higher latitudes of the northern U.S., the less exposed you'd be to the harmful rays of the sun, and therefore, the less risk you'd have of death due to skin cancer.
- Some other examples of statistical relationships might include:
	- **Relationship between Height and weight**, we all knows for each person height increases, you'd expect weight to increase, but not perfectly.
	- **Relationship between Speed and Mileage**, as driving speed increases, you'd expect gas mileage to decrease, but not perfectly.

##### Reference URL:    
  [https://newonlinecourses.science.psu.edu/stat501/node/250/](https://newonlinecourses.science.psu.edu/stat501/node/250/)    
  [https://www.youtube.com/playlist?list=PLIeGtxpvyG-LoKUpV0fSY8BGKIMIdmfCi](https://www.youtube.com/playlist?list=PLIeGtxpvyG-LoKUpV0fSY8BGKIMIdmfCi)