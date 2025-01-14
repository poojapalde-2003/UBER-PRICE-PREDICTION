# UBER-PRICE-PREDICTION
**TITLE:** Predict the price of the Uber ride from a given pickup point to the agreed drop-off 
location.
Perform following tasks:
1. Pre-process the dataset.
2. Identify outliers.
3. Check the correlation.
4. Implement linear regression and random forest regression models.
5. Evaluate the models and compare their respective scores like R2, RMSE, etc.
   
**AIM: **Aim of this practical is to demonstrate data pre-processing techniques, identify and remove 
outliers, implement and evaluate performance of different regression models.

**OBJECTIVES:** Based on above main aim following are the objectives 
1. To understand data preprocessing steps
2. To identify and remove outliers
3. To implement different regression models. (Linear Regression & Random Forest)
**What is Data Preprocessing?**
Data preprocessing is a data mining technique which is used to transform the raw data in a 
useful and efficient format.
**Steps Involved in Data Preprocessing: **
**1. Data Cleaning: **
The data can have many irrelevant and missing parts. To handle this part, data cleaning is 
done. It involves handling of missing data, noisy data etc. 
(a). Missing Data: 
This situation arises when some data is missing in the data. It can be handled in various ways. 
Some of them are: 
1. Ignore the tuples: 
This approach is suitable only when the dataset we have is quite large and multiple 
values are missing within a tuple. 
2. Fill the Missing values: 
There are various ways to do this task. You can choose to fill the missing values 
manually, by attribute mean or the most probable value. 
(b). Noisy Data: 
Noisy data is a meaningless data that can’t be interpreted by machines. It can be generated 
due to faulty data collection, data entry errors etc. It can be handled in following ways:
1. Binning Method: 
This method works on sorted data in order to smooth it. The whole data is 
divided into segments of equal size and then various methods are performed 
to complete the task. Each segmented is handled separately. One can replace 
all data in a segment by its mean or boundary values can be used to complete 
the task. 
2. Regression:Here data can be made smooth by fitting it to a regression function.The regression used 
may be linear (having one independent variable) or multiple (having multiple independent 
variables). 
3. Clustering: 
This approach groups the similar data in a cluster. The outliers may be undetected or it will 
fall outside the clusters. 
**2. Data Transformation: **
This step is taken in order to transform the data in appropriate forms suitable for mining 
process. This involves following ways: 
1. Normalization: 
It is done in order to scale the data values in a specified range (-1.0 to 1.0 or 0.0 to 1.0) 
2. Attribute Selection: 
In this strategy, new attributes are constructed from the given set of attributes to help the 
mining process. 
3. Discretization: 
This is done to replace the raw values of numeric attribute by interval levels or conceptual 
levels. 
4. Concept Hierarchy Generation: 
Here attributes are converted from lower level to higher level in hierarchy. For Example-
The attribute “city” can be converted to “country”. 
**3. Data Reduction: **
Since data mining is a technique that is used to handle huge amount of data. While working 
with huge volume of data, analysis became harder in such cases. In order to get rid of this, we uses data 
reduction technique. It aims to increase the storage efficiency and reduce data storage and analysis 
costs. 
**The various steps to data reduction are: **
1. Data Cube Aggregation: 
Aggregation operation is applied to data for the construction of the data cube. 
2. Attribute Subset Selection: 
The highly relevant attributes should be used, rest all can be discarded. For performing attribute 
selection, one can use level of significance and p- value of the attribute.the attribute having p-
value greater than significance level can be discarded. 
3. Numerosity Reduction: 
This enable to store the model of data instead of whole data, for example: Regression Models. 
4. Dimensionality Reduction: 
This reduce the size of data by encoding mechanisms.It can be lossy or lossless. If after 
reconstruction from compressed data, original data can be retrieved, such reduction are called 
lossless reduction else it is called lossy reduction. The two effective methods of dimensionality 
reduction are:Wavelet transforms and PCA (Principal Component Analysis)
Outlier: An outlier is an object that deviates significantly from the rest of the objects. They can 
be caused by measurement or execution error. The analysis of outlier data is referred to as 
outlier analysis or outlier mining.

**Detecting Outlier:**
Clustering based outlier detection using distance to the closest cluster:
In the K-Means clustering technique, each cluster has a mean value. Objects belong to the 
cluster whose mean value is closest to it. In order to identify the Outlier, firstly we need to 
initialize the threshold value such that any distance of any data point greater than it from its 
nearest cluster identifies it as an outlier for our purpose. Then we need to find the distance of 
the test data to each cluster mean. Now, if the distance between the test data and the closest 
cluster to it is greater than the threshold value then we will classify the test data as an outlier.
**Algorithm:**
1. Calculate the mean of each cluster
2. Initialize the Threshold value
3. Calculate the distance of the test data from each cluster mean
4. Find the nearest cluster to the test data
5. If (Distance > Threshold) then, Outlier
   
**Correlation Matrix:** Correlation is an indication about the changes between two variables. In our 
previous chapters, we have discussed Pearson’s Correlation coefficients and the importance of 
Correlation too. We can plot correlation matrix to show which variable is having a high or low 
correlation in respect to another variable.
Linear Regression: Linear Regression is a machine learning algorithm based on supervised 
learning. It performs a regression task. Regression models a target prediction value based on 
independent variables. It is mostly used for finding out the relationship between variables and 
forecasting. Different regression models differ based on – the kind of relationship between 
dependent and independent variables they are considering, and the number of independent 
variables getting used.
Linear regression performs the task to predict a dependent variable value (y) based on a given 
independent variable (x). So, this regression technique finds out a linear relationship between x 
(input) and y(output). Hence, the name is Linear Regression.
In the figure above, X (input) is the work experience and Y (output) is the salary of a person. The 
regression line is the best fit line for our model.
Hypothesis function for Linear Regression:
