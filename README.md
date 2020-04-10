# Boston-house-prices_project

This is an end-to-end machine learning project that uses the Boston house prices dataset. Each record in the database describes a Boston suburb or town. The data was drawn from the Boston Standard Metropolitan Statistical Area (SMSA) in 1970. The attributes are deﬁned as follows (taken from the UCI Machine Learning Repository :   
CRIM: per capita crime rate by town  
ZN: the proportion of residential land zoned for lots over 25,000 sq.ft.  
INDUS: the proportion of non-retail business acres per town  
CHAS: Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)  
NOX: nitric oxides concentration (parts per 10 million)  
RM: average number of rooms per dwelling  
AGE: the proportion of owner-occupied units built before 1940  
DIS: weighted distances to ﬁve Boston employment centers  
RAD: index of accessibility to radial highways  
TAX: full-value property-tax rate per $10,000  
PTRATIO: pupil-teacher ratio by town  
B: 1000(Bk−0.63)2 where Bk is the proportion of blacks by town  
LSTAT: % lower status of the population  
MEDV: Median value of owner-occupied homes in $1000s  
We can see that the input attributes have a mixture of units.

Here is an overview of the steps in this project:

1. Prepare Problem  
a) Load libraries needed for this problem  
b) Load dataset from Kaggle (boston-house-prices)  

2. Summarize Data  
a) Descriptive statistics: summarizing the distribution of each attribute, and getting an idea of the correlation between attributes.  
b) Data visualizations: drawing histograms, densities and box plots of each attribute, to detect  possible exponential and bimodal distributions, also the outliers; Visualizing interactions between attribute using scatter matrix  

3. Evaluate Algorithms  
a) Split-out test dataset: using 80% of the dataset for modeling and hold back 20% for test.  
b) Spot Check Algorithms: evaluating some alogorithms to get an idea on the performance of each algorithm, using the 10-fold cross-validation :  
      - Linear Algorithms: Linear Regression (LR), Lasso Regression (LASSO) and ElasticNet (EN)  
      - Nonlinear Algorithms: Classiﬁcation and Regression Trees (CART), Support Vector Regression (SVR) and K-Nearest Neighbors (KNN)    
c) Compare Algorithms: Kepping the algorithm with the lowest error (KNN), based on the evaluation metric (NMSE in this case)  

4. Improve Accuracy  
a) Algorithm Tuning: iterating on the tunning parameter (n_neighbors) of the KNN algorithm to improve its  accuracy   
b) Ensembles:   
Evaluating four diﬀerent ensemble machine learning algorithms : Boosting Methods [AdaBoost (AB) and Gradient Boosting (GBM)], Bagging Methods [Random Forests (RF) and Extra Trees (ET)]  
Tuning the Extra Trees to further lift the performance  

5. Finalize Model  
Predictions on test dataset: training the model on the entire training dataset, then predicting the test dataset
