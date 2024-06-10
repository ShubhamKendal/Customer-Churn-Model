# SpeakX-Assignment

Predicting Customer Churn in a Telecommunications Company

Monday, 10 June 2024

By Shubham Kendal (12301314)
 
Steps I followed to make the Prediction model are as follows :-

•	In starting I import the dataset by using the Pandas library of Python.


•	Then, I have converted the Categorical data into Numerical data by using the sklearn library of Python.

•	EDA : I have done these steps while performing the EDA on the dataset :
1.	Compute the Five Number Summary.
2.	Find the different column names that we have in our data.
3.	Find the no. of unique values present in each column.
4.	Then, I found is there any null values present in the dataset and found that there are no null values present in the data.
5.	Compute Correlation matrix of our data try to find out the correlation between our target variable i.e. Churn and other columns.
6.	Then by using the Seaborn library I plot pairplot for the data.
7.	Plot the histogram for the Monthly Charges and Total Charges.
 The conclusion I get after performing EDA is that by using correlation matrix, we can see that there are certain columns which are highly correlated with the target column. So, as a result we drop that columns from the data to make our model more precise and faster.

•	Now, we can see that the difference between the values of column named as Tenure and Monthly Charges and Total Charges are very high which can affect the precision and accuracy of our model. So, to resolve that issue I have done scaling on these columns where I have used MinMaxScaler from sklearn  library of Python.

•	Since now we get our required columns which are highly correlated with target column and they are scaled also. Now, I have break down my data into input variable and Target variable where Churn is the target variable and all others are input variable.

•	Now, Splitting the data into Train and Test sets where we use Train set for fitting the model and Test set is used for predicting the  model and finding the accuracy of the model. I have taken the test size as 20% which means 20% of the data will be used for Test set and left 80% for Train set.

•	Now, Building the model here we will be using Random Forest Algorithm. In Random Forest Algorithm we make multiple decision trees and we predict the output on the basis of majority of the results which we get from multiple decision trees.

•	Then, Fitting the model and checking the accuracy of the model by two methods that are R-square score and Confusion matrix.

•	The accuracy of my Random Forest Prediction model is 79.25%.

The problem that I have faced during building the model is that i want to improve the accuracy of the model but i just got the 79.25% highest R-square value for my model.

Thank You.
