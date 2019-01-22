# Data preprocessing
- Data pre-Processing is one of the important task in Machine/Deep Learning field.
- Pre-processing refers to the transformations applied to our data before feeding it to the algorithm.
- Data Preprocessing is a technique that is used to convert the raw data into a clean data set. In other words, whenever the data is gathered from different sources it is collected in raw format which is not feasible for the analysis.
- To achieve a best result in the applied model in Machine Learning projects the format of the data has to be in a proper manner. 
- For Example:
	- Random Forest algorithm does not support null values, therefore to execute random forest algorithm null values have to be managed from the original raw data set. This is know as Handling Missing data in data pre-processing task.
- Another aspect is that data set should be formatted in such a way that more than one Machine Learning and Deep Learning algorithms are executed in one data set, and best out of them is chosen.
- In this part I will show you the lit of techniques available in data pre-processing and how to get in handy with them. Data pre-processing has the following stages:
1. Handling Missing Data
2. Handling Categotical Data
3. Splitting Data-set into Dev/Training/Test sets
4. Feature Scaling
5. So lets dive into the module.

### 1. Handling Missing Data
- As all we know the term Missing data reffers to the data's actually not available in the expected field or available as Null or empty. if we are not addressing this issue with high prority your machine learning model will give poor prediction result.
- So we need to be equipped to handle the problem when we come across them.
- We can see multiple suggestions and ways in imternet to address this porblem, but one of the thumb rule in machine learning is Every record is importannt and we dont know some information belons to that row may be an important key factor for our prediction.
- So we are going to take one of the most common idea to handle the problem is to take a mean/Median/Most_Occured of all the values from the column and replace it with missing data.
- Imputer is a class from Scikit Learn library.Preperocessing which is going to do the task, exactly it is going to do above step.
- it has the following input parameters:
	- missing_values:
		- it has valeus like integer, string, np.nan(default) or None. 
		- Based on your usecase you can go with either of'em. at the initial phase of data pre-processing it is recommended to go with NaN.
	- strategy:
		- it is an optional field
		- By default will take mean of the column
		- If Mean --> then replace missing values using the mean along each column and it Can only be used with numeric data.
		- If Median --> then replace missing values using the median along each column. Can only be used with numeric data.
		- If most_frequent --> then replace missing using the most frequent value along each column. Can be used with strings or numeric data.
		- If constant --> then replace missing values with fill_value. Can be used with strings or numeric data.
	- Axis:
		- The axis along which to impute.
		- by default it is 0
		- If axis=0, then impute along columns.
		- If axis=1, then impute along rows.
	- it has some other input parameters like verbos and copy, based on your use case you can choose it. the abouve 2 are the most frequently used input arguments.
	
	from sklearn.preprocessing import Imputer
	imputer = Imputer(missing_values = "NaN", strategy = "mean")
	
- Once we have done the above 2 steps we can either do fit and transform separately or simply we can call fit_transform method from imputer to fill the missing values with relevent information
	
	imputer = imputer.fit(X[:,1:3])
	X[:, 1:3] = imputer.transform(X[:, 1:3])
	
	or
	
	X[:, 1:3] = imputer.fit_transform(X[:, 1:3])
	
- The code above will fit_transform the imputer object to our matrix of features X. Since we used :, it will select all rows and 1:3 will select the second and the third column 
	
### 2. Handling Categorical Data
- Categorical data is our next huddle in our pipeline to be encountered next with high priority.
- Sometimes our data is in qualitative form, that is we have texts as our data.
- Now it gets complicated for machines to understand texts and process them, rather than numbers, since the models are based on mathematical equations and calculations.
- We cannot convert all the data from text form to numeric, expect some like categorical data. therefore we have to encode the categorical data,
- examples of categorical data we may expect in our data-set are Country, Department, Gender and any key which will place Group by Aggregation operation in your problem.
- LableEncoder ans OneHotEncoder are a classes form Scikit Learn library.Preperocessing which is going to do the task, exactly it is going to do above step.
- Lable Encoder:
	- it is mainly used to convert Categorical variables into a sequence of numbers like 0, 1, 2, 3, 4, 5 and etc.. based on the upper limit.
	- It is important to remember that the index starts from 0 and ends with upper limit.
	- once the encoding is done we can see our encoded data.
	- to perform the task, run the below command
	
	from sklearn.preprocessing import LabelEncoder, OneHotEncoder
	lableEnc = LabelEncoder()
	
	X[:,0] = labelencoder_X.fit_transform(X[:,0]) # 0 represents the Encoding column.
	
	- The above code will select all the rows (because :) of the first column (because 0) and fit the LabelEncoder to it and transform the values.
	- Here we will create a new problem if there are more than two categories.
	- As we keep assigning different integers to different categories, it may create a confusion for the algorithm to learn the Relationship(trend)
	- to solve this problem we are going to use OneHotEncoder
- OneHotEncoder:
	- it is recommended to have this in pipeline after LableEncoder completed.
	- The transformation behind OneHotEncoder is very simple it follows the operation of Binary Transformation, hope you might remembered the relationship between interger to Binary format.
	- Here we are going to convert the values encoded using LableEncoder to Binary form.
	- it has an important parameter called categorical_features to accomplish the tast.
	- by running the below code in our dataset, it will select the first column to OneHotEncode the categories.
	- then simple calling fit_transform method wil do te remain for us.
	onehotencoder = OneHotEncoder(categorical_features =[0])
	X = onehotencoder.fit_transform(X).toarray()
	
	- If you check your dataset now, all your categories will have been encoded to 0s and 1s.
	
### 3. Spliting your data-set into Dev/Training/Test set
- It is recommended to split your data-set to Dev/Training/Test sets to complete our ddevelopment, training and Tests.
- Usually in internet you can find only Training/Test set separation only, you can follow any method. for your understanding we are going to use only Training/Test sepparation only.
- We will train our machine learning models on our training set, i.e our machine learning models will try to understand any correlations in our training set and then we will test the models on our test set to check how accurately it can predict.
- A general rule of the thumb is to allocate 80% of the dataset to training set and the remaining 20% to test set.
- test_train_split is a calss of sklearn.model_selection library, which is going to do the task.

from sklearn.model_selection import train_test_split
X_train, X_test, Y_train, Y_test = train_test_split(X,Y, test_size=0.2)

- The above code will split out dataset into training and test set based on 80/20 ratio. and will assing the data into 4 new variables called X_train, X_test, Y_train, Y_test.
- For our understanding we are using the name as X_train, X_test, Y_train, Y_test. you can keep any name based on your understanding.

### 4. Feature Scaling
- The final step of data preprocessing is to apply the very important feature scaling.
- Feature scaling is a method used to standardize the range of independent variables or features of data. 
- Why it is important:
	- A lot of machine learning models are based on Euclidean distance.
	- for example, the values in one column (x) is much higher than the value in another column (y), (x2-x1) squared will give a far greater value than (y2-y1) squared.
	- it chows clearly that one square difference dominates over the other square difference.
	- In the machine learning equations, the square difference with the lower value in comparison to the far greater value will almost be treated as if it does not exist.
	- That is why it is necessary to transform all our variables into the same scale.
- There are several ways of scaling the data. we are going to follow one of the mostly used way called Standardization.
- For every observation of the selected column, our program will apply the below formula of standardization and fit it to a scale.
- StandardScaler is a class of sklearn.preprocessing library, which is going to do the task.
	
	from sklearn.preprocessing import StandardScaler
	sc_X = StandardScaler()
	X_train = sc_X.fit_transform(X_train)
	X_test = sc_X.transform(X_test)

- Note: the above step is required when you have too large values Predictor/Independent variable.
