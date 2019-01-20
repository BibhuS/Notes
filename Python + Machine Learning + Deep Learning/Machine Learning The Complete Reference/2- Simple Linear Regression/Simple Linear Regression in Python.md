# Simple Linear Regression in Python:

#### 1 - Prerequisites:    
  - Basics of Numpy    
  - Basics of Pandas    
  - Basics of sklearn.linear_model.LinearRegression    
  - Basics of statsmodels.api.OLS    
  - Basics of matplotlib.pyplot

##### 2 - Import Libraries:
- If you want to write your own program to predict Simple Linear Regression you need to import the needed libraries first

<p align="center">
  	<img width="556" height="119" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-%20Simple%20Linear%20Regression/References/python-1.JPG?raw=true">
</p>

#### 3 - Import Dataset
- Importing our data-set is the next step, once we imported our data-set we need to Independent Variable(IV) and Dependent Variable(DV) out of data-set.
- Here we are using **Pandas** library to Import our data-set from the directory, it is recommended to keep the data-set in same directory where the python file is saved.
- We are specifying required No.of rows and columns using pandas.iloc method.
- Here in **[:, :-1]**, **:** refers to fetch all rows from our data-set and **:-1** refers to fetch all columns other than last column, since we have only one column as IV in our data-set will fetch only one ndArray as **X**
- **pandas.iloc.values** will actualy fetch and load values from data-set to variable **X and y**.

<p align="center">
  	<img width="554" height="73" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-%20Simple%20Linear%20Regression/References/python-2.JPG?raw=true">
</p>

#### 4 - Split Data into Training set and Test Set
- Once we got our IV and DV, it is recommended to Split your data in to Training set and Test Set.
- But in our case our ID and DV contains only 6 rows we are not doing this step as of now for this Example, But please find the Below code to split your IV and DV.

<p align="center">
  	<img width="677" height="60" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-%20Simple%20Linear%20Regression/References/python-10.JPG?raw=true">
</p>

#### 5 - Fit Model
- Once our data set is splited as **X and y** we can start our model fitting.

<p align="center">
  	<img width="559" height="61" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-%20Simple%20Linear%20Regression/References/python-3.JPG?raw=true">
</p>


