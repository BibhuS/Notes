# 1.About the Course:
- Hi, a warm Welcome to you. If you are one of the person who is trying to explore more detail in Machine Learning like others, but don't know where/how to start ? Hooray, you are in the right place at right time.
- The course has been designed by a Professional Machine Learning Engineer, who is trying to create more opportunists in Machine Learning by sharing his knowledge and helping you to solve complex Algorithms in simple way.
- I am going to take you step by step to the world of Machine Learning, With every tutorial in this course you will develop new skills and improve your understanding in Machine Learning.
- Moreover, the course is packed with practical exercises which are based on real-life examples. So you will learn the theory and also get some hands-on practice by building your own models and use-cases.
- The course is structured the following way:
	1. [Data Pre-Processing](https://github.com/ManikandanJeyabal/Notes/tree/master/Python%20+%20Machine%20Learning%20+%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-Data%20Pre-Processing#data-preprocessing)
		1. [Handling Missing Data](https://github.com/ManikandanJeyabal/Notes/tree/master/Python%20+%20Machine%20Learning%20+%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-Data%20Pre-Processing#1-handling-missing-data)
		2. [Handling Categorical Data](https://github.com/ManikandanJeyabal/Notes/tree/master/Python%20+%20Machine%20Learning%20+%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-Data%20Pre-Processing#2-handling-categorical-data)
		3. [Splitting Data-Set into Dev/Training/Test set](https://github.com/ManikandanJeyabal/Notes/tree/master/Python%20+%20Machine%20Learning%20+%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-Data%20Pre-Processing#3-spliting-your-data-set-into-devtrainingtest-set)
		4. [Feature Scaling](https://github.com/ManikandanJeyabal/Notes/tree/master/Python%20+%20Machine%20Learning%20+%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/2-Data%20Pre-Processing#4-feature-scaling)
 	2. Regression Models
	 	1. [Simple Linear Regression](https://github.com/ManikandanJeyabal/Notes/tree/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/3-%20Simple%20Linear%20Regression)
	 	2. Multiple Linear Regression
	 	3. Polynomial Regression
	 	4. SVR
	 	5. Decision Tree Regression
	 	6. Random Forest Regression
 	3. Classification 
	 	1. Logistic Regression
	 	2. K-NN
	 	3. SVM
	 	4. Kernel SVM
	 	5. Naive Bayes
	 	6. Decision Tree Classification
	 	7. Random Forest Classification
 	4. Clustering
	 	1. K-Means
	 	2. Hierarchical Clustering
 	5. Association Rule Learning 
	 	1. Apriori Rule
	 	2. Eclat Rule
 	6. Reinforcement Learning
	 	1. UCB - Upper Confidence Bound
	 	2. Thompson Sampling
 	7. Deep Learning
	 	1. Artificial Neural Networks
	 	2. Convolutional Neural Networks
 	8. Dimensionality Reduction 
	 	1. PCA
	 	2. LDA
	 	3. Kernel PCA
 	9. Model Selection & Boosting
	 	1. k-fold Cross Validation
	 	2. Parameter Tuning
	 	3. Grid Search
	 	4. XGBoost
  
# 2.Targeted Audience:
- Anyone interested in Machine Learning.
- Any data analysts who want to level up in Machine Learning.
- Students who have at least high school knowledge in math and who want to start learning Machine Learning.
- Any intermediate level people who know the basics of machine learning, including the classical algorithms like linear regression or logistic regression, but who want to learn more about it and explore all the different fields of Machine Learning.
- Any people who are not that comfortable with coding but who are interested in Machine Learning and want to apply it easily on datasets.
- Any people who are not satisfied with their job and who want to do something new in Machine Learning.

# 3.What you will Learn:
- Master Machine Learning on Python.
- Have a great intuition of many Machine Learning models.
- Make accurate predictions by powerful analysis methods.
- Make robust Machine Learning models.
- Handle specific topics like Reinforcement Learning, NLP and Deep Learning and Handle advanced techniques like Dimensionality Reduction
# 4.What is Machine Learning:
- **Machine learning** is a method of data analysis that automates analytical model building. 
- It is a branch of artificial intelligence based on the idea that systems can learn from data, find patterns and make decisions with minimal human intervention. 
- While artificial intelligence (AI) is the broad science of mimicking human abilities, machine learning is a specific subset of AI that trains a machine how to learn.
- The processes involved in machine learning are similar to data mining and predictive modeling. Both require searching through data to look for patterns and adjusting program actions accordingly.
- Many people are familiar with machine learning from shopping on the internet and being served ads related to their purchase. This happens because recommendation engines use machine learning to personalize online ad delivery in almost real-time.
- Machine learning algorithms are often categorized as **Supervised** or **Unsupervised** or **Semi-Supervised** Learning.

#### 4.1 Supervised Learning:
- Supervised algorithms require a data scientist or data analyst with machine learning skills to provide both input and desired output, in addition to furnishing feedback about the accuracy of predictions during algorithm training.
- Data scientists determine which variables, or features, the model should analyze and use to develop predictions.
- Once training is complete, the algorithm will apply what was learned to new data.
- In simple terms Supervised Learning is know as "Supervised learning is so named because the data scientist acts as a guide to teach the algorithm what conclusions it should come up with". and it is the more commonly used between the three.
- It includes such algorithms as linear and logistic regression, multi-class classification, and support vector machines and etc... **For Example:** A child might learn arithmetic from a teacher
- Supervised learning requires that the algorithm’s possible outputs are already known and that the data used to train the algorithm is already labeled with correct answers.
- **For Example:** Classification algorithm will learn to identify animals after being trained on a dataset of images that are properly labeled with the species of the animal and some identifying characteristics

#### 4.2 Unsupervised Learning:
- Unsupervised algorithms do not need to be trained with desired outcome data. Instead, they use an iterative approach called deep learning to review data and arrive at conclusions. 
- Unsupervised learning algorithms also uses an area called neural networks, they used for more complex processing tasks than supervised learning systems, including image recognition, speech-to-text and natural language generation.
- These neural networks work by combing through millions of examples of training data and automatically identifying often subtle correlations between many variables. Once trained, the algorithm can use its bank of associations to interpret new data.
- These algorithms have only become feasible in the age of big data, as they require massive amounts of training data.
- Some examples of unsupervised machine learning algorithms include k-means clustering, principal and independent component analysis, and association rules.

#### 4.3 Which algorithm to choose for my problem:
- Choosing to use either a supervised or unsupervised machine learning algorithm typically depends on factors related to the structure and volume of your data and the use case of the issue at hand.
- A well-rounded data science program will use both types of algorithms to build predictive data models that help stakeholders make decisions across a variety of business challenges.

#### 4.4 Semi-Supervised Learning:
- Semi-supervised learning is a class of machine learning tasks and techniques that also make use of unlabeled data for training – typically a small amount of labeled data with a large amount of unlabeled data.
- Semi-supervised learning falls between unsupervised learning (without any labeled training data) and supervised learning (with completely labeled training data).
- Many machine-learning researchers have found that unlabeled data, when used in conjunction with a small amount of labeled data, can produce considerable improvement in learning accuracy over unsupervised learning but without the time and costs needed for supervised learning.
- As you may have guessed, semi-supervised learning algorithms are trained on a combination of labeled and unlabeled data. This is useful for the following  reasons.
	1. the process of labeling massive amounts of data for supervised learning is often prohibitively time-consuming and expensive.
	2. What’s more, too much labeling can impose human biases on the model.
	3. That means including lots of unlabeled data during the training process actually tends to improve the accuracy of the final model while reducing the time and cost spent building it.
- For the above Reasons, semi-supervised learning is a win-win for use cases like webpage classification, speech recognition, or even for genetic sequencing.

#### 4.5 What is required to create a good machine learning systems:
- Data preparation capabilities.
- Algorithms – basic and advanced.
- Automation and iterative processes.
- Scalability.
- Ensemble modeling.
  
#### 4.6 Who's using it ?
- Most industries working with large amounts of data have recognized the value of machine learning technology. Below listed are some of area's Machine Learning models are being used widely.
- **Financial services**:
	- Banks and other businesses in the financial industry use machine learning technology for two key purposes:
	- to identify important insights in data, and prevent fraud.
	- The insights can identify investment opportunities, or help investors know when to trade.
	- Data mining can also identify clients with high-risk profiles, or use Cyber-Surveillance to pinpoint warning signs of fraud.
- **Health care**:
	- Machine learning is a fast-growing trend in the health care industry, thanks to the advent of wearable devices and sensors that can use data to assess a patient's health in real-time. 
	- The technology can also help medical experts analyze data to identify trends or red flags that may lead to improved diagnoses and treatment. 
- **Retail**:
	- Websites recommending items you might like based on previous purchases are using machine learning to analyze your buying history. 
	- Retailers rely on machine learning to capture data, analyze it and use it to personalize a shopping experience, implement a marketing campaign, price optimization, merchandise supply planning, and for customer insights. 
- **Oil and gas**:
	- Finding new energy sources. 
	- Analyzing minerals in the ground. 
	- Predicting refinery sensor failure. 
	- Streamlining oil distribution to make it more efficient and cost-effective. 
	- The number of machine learning use cases for this industry is vast – and still expanding.
    
#### 4.7 Did you know ?
- In machine learning, a target is called a label. where in statistics, a target is called a dependent variable.
- A variable in statistics is called a feature in machine learning.
- A transformation in statistics is called feature creation in machine learning.

# 5.Installing Anaconda and Python in your Machine:
- It is recommended to have at-least machine with 8GB-RAM. i prefer to go with Anaconda since it gives you all the libraries more handy
- Open the following URL in our browser, [Anaconda Installing User Guide](https://conda.io/docs/user-guide/install/windows.html).
- Find 2 Different types of Installation modes available in the Doc Page as shown below.

<p align="center">
  <img width="756" height="305" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/1-Introduction/References/2TypesOfInstallation.JPG?raw=true">
</p>

- If you are installing Anaconda in your Personal PC/Laptop you can proceed to download Anaconda for Python 3.7 and above, run the .Exe will ask you for Anaconda installation path don't change anything leave things as it and completed the installation.
- Usually installation will take 20-30 min. Please find the below image for your reference.

<p align="center">
  <img width="1043" height="466" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/1-Introduction/References/Anaconda%20Installer.JPG?raw=true">
</p>

- If you want to use anaconda in PC/Laptop which does not have Admin access, recommend to use Minicoda a silent version of Anaconda will install everything by default in the machine. (Note: you are the complete responsibility for this action.)
- please find the below images to Download and install Miniconda in your machine.

<p align="center">
  <img width="1039" height="671" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/1-Introduction/References/Miniconda%20Installer.JPG?raw=true">
</p>


<p align="center">
  <img width="740" height="600" src="https://github.com/ManikandanJeyabal/Notes/blob/master/Python%20%2B%20Machine%20Learning%20%2B%20Deep%20Learning/Machine%20Learning%20The%20Complete%20Reference/1-Introduction/References/Installing%20Miniconda%20-%201.JPG?raw=true">
</p>

- Miniconda Installation command `start /wait "" Miniconda4-latest-Windows-x86_64.exe /InstallationType=JustMe /RegisterPython=0 /S /D=%UserProfile%\Miniconda3`. Here replace the Miniconda version with your version
