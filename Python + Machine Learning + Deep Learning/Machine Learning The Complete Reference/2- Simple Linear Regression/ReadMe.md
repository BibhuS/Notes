# Simple Linear Regression

### 1 - Introduction
- Simple linear regression is a statistical method that allows us to summarize and study relationships(trend) between two continuous (quantitative) variables.
- We are going to learn the concept and basic procedures of simple linear regression.
- We will also learn two measures that describe the strength of the linear association that we find in data.

###### 1.1 - Things to Remember:    
  SLR -> Simple Linear Regression    
  MLR -> Multi Linear Regression    
  [Formula to find Mean](https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/Formulas/Mean.JPG?raw=true)    
  [Formula to find Median](https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/Formulas/Median.JPG?raw=true)

### 2 - What is Simple Linear Regression?
- As we seen earlier in introduction SLR is known as the following,
	- Simple linear regression is a statistical method that allows us to summarize and study relationships(trend) between two continuous (quantitative) variables.
	- One variable, denoted **X**, is regarded as the **predictor**, **explanatory**, or **independent variable**.
	- The other variable, denoted **y**, is regarded as the **response**, **outcome**, or **dependent variable**.
- SLR gets its adjective "simple," because it concerns the study of only one predictor variable.
- A simple key difference between SLR and MLR, is MLR gets its adjective "multiple," because it concerns the study of  two or more predictor variables.


### 2.1 - Types of Relationships:
- There are two types of relationships available one is  **deterministic (or functional) relationships** and second one is **statistical relationships**, simple linear regression will deals with second one.
	
###### 2.1.1 - Deterministic (or Functional) Relationships:
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
  - **Hooke's Law:** Y = α + βX, where Y = amount of stretch in a spring, and X = applied weight.
  - **Ohm's Law:** I = V/r, where V = voltage applied, r = resistance, and I = current.
  - **Boyle's Law:** For a constant temperature, P = α/V, where P = pressure, α = constant for each gas, and V = volume of gas.

###### 2.1.2 - Statistical Relationships:
- In statistical relationship, the relationship between the variables is not perfect.
- The below example illustrate the relationship between response variable y is the mortality due to skin cancer (number of deaths per 10 million people) and the predictor variable x is the latitude (degrees North) at the center of each of 49 states in the U.S. [(dataset.txt)](https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-%20Simple%20Linear%20Regression/Dataset/SkinCancer.csv)    
  <p align="center">
  	<img width="502" height="333" src="https://newonlinecourses.science.psu.edu/stat501/sites/onlinecourses.science.psu.edu.stat501/files/01simple/scatterplot_skin_cancer/index.png">
  </p>
- The above plot appears to be a negative linear relationship between latitude and mortality due to skin cancer, but the relationship is not perfect.
- Indeed, the plot exhibits some "trend," but it also exhibits some "scatter." Therefore, it is a statistical relationship, not a deterministic one.
- Based on the above observation if you lived in the higher latitudes of the northern U.S., the less exposed you'd be to the harmful rays of the sun, and therefore, the less risk you'd have of death due to skin cancer.
- Some other examples of statistical relationships might include:
	- Relationship between **Height and weight**, we all knows for each person height increases, you'd expect weight to increase, but not perfectly.
	- Relationship between **Speed and Mileage**, as driving speed increases, you'd expect gas mileage to decrease, but not perfectly.

### 3 - What is Best-Fitting Line ?
- In Definition, Line of best fit refers to a line through a scatter plot of data points that best expresses the relationship between those points.
- A straight line will result from a simple linear regression analysis of two or more independent variables.
- Since we are interested in summarizing the trend between two quantitative variables, we have to Find the Best-Fitting line for our equation.
- Equation for Best-Fit Line:
<p align="center">
	<b>y&#770;<sub>i</sub> = <i>b</i><sub>0</sub> + <i>b</i><sub>1</sub><i>x</i></b><br>
</p> 
- <b>y<sub>i</sub></b> - observed response for experimental unit <i>i</i>    
- <b>x<sub>i</sub></b> - predictor value for experimental unit <i>i</i>    
- <b>y&#770;<sub>i</sub></b> - predicted response (or fitted value) for experimental unit <i>i</i>    
- <b><i>b</i><sub>0</sub></b> - Intercept point, where <b>y<sub>i</sub></b> meets <b>x</b>    
<p align="center">
  	<img width="502" height="333" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20+%20Machine%20Learning%20+%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-%20Simple%20Linear%20Regression/References/Best%20Fit%20Line%20-%20trend%20between%20Height%20and%20Weight.jpg?raw=true">
</p>
- For Example:    
  	- lets find the **y&#770;<sub>i</sub>** for the first data point in the list indicates that student 1 is 63 inches tall and weighs 127 pounds. that means **x<sub>i</sub> = 63** and **y<sub>i</sub> = 127**. then the **y&#770;<sub>i</sub> = 120.1**(by applying **w = -266.53 + 6.1376 h** formula).
	- in the above Example the Predicted value is not accurate it has some difference on it which is known as **"prediction error"** (or **"residual error"**). In fact, the size of its prediction error is 127-120.1 or 6.9 pounds.
	- Find **y&#770;<sub>i</sub>** for the remaining values in below chat.
	<p align="center">
  	<img width="502" height="333" src="https://newonlinecourses.science.psu.edu/stat501/sites/onlinecourses.science.psu.edu.stat501/files/01simple/heightweight/index.jpg">
    </p>
	- As you can see, the size of the prediction error purely depends on the data point.
	- If we didn't know the weight of student 5, the equation of the line would predict his or her weight to be -266.53 + 6.1376(69) or 157 pounds.
	- The size of the prediction error here is 162-157, or 5 pounds.
- Keep in mind the thumb rule A line that fits the data "best" will be one for which the n prediction errors are as small as possible in some overall sense.
- One way to achieve this goal is to invoke the "least squares criterion," which says to "minimize the sum of the squared prediction errors." 


##### Quick Review:    
- Simple Linear Regression is really a comparison of 2 models    
	- when Independent Variable does not Exists
	- use the Best-Fitting Line to determine Relationship(trend) between 2 Variables

##### Reference URL:    
  [To Understand Concepts Behind SLR - Site](https://newonlinecourses.science.psu.edu/stat501/node/250/)    
  [To Understand Concepts Behind SLR - Video](https://www.youtube.com/playlist?list=PLIeGtxpvyG-LoKUpV0fSY8BGKIMIdmfCi)