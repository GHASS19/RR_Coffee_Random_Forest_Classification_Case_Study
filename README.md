# RR Diner Coffee

![image](https://user-images.githubusercontent.com/86930309/227387324-7433daa7-cff3-4520-9279-4c154c380ac5.png)

In this case study, you’ll become the lead data scientist for an up-and-coming specialty coffee company seeking to use customer data to justify critically important
business decisions. You will use scikitlearn to build four different decision tree models — two using entropy and two using gini impurity — to ascertain whether a 
potentially business-transforming deal with a mysterious coffee farm in China will take your business to the next level. 

The case study will involve your use of the full data science pipeline, from importing, loading and cleaning the data right through to modeling and concluding. In the
case study, your decision trees will properly implement the supervised learning method of classification, and you will enforce the best practices of:

- Making an appropriate train/test split
- One-hot encoding
- Model evaluation
- Restricting the maximum depth of the tree
- Using random forest to increase predictive accuracy and control overfitting

RR Diner Coffee has a decision about whether to strike a deal with a legendary coffee farm (known as the Hidden Farm) in rural China: there are rumours their coffee tastes of lychee and dark chocolate, while also being as sweet as apple juice.

It's a risky decision, as the deal will be expensive, and the coffee might not be bought by customers. The stakes are high: times are tough, stocks are low, farmers are reverting to old deals with the larger enterprises and the publicity of selling Hidden Farm coffee could save the RR Diner Coffee business.

Your first job, then, is to build a decision tree to predict how many units of the Hidden Farm Chinese coffee will be purchased by RR Diner Coffee's most loyal customers.

Your team has conducted a survey of 710 of the most loyal RR Diner Coffee customers, collecting data on the customers.

## 1. Sourcing and loading

## - Import packages
## - Load data
## - Explore the data

## 2. Cleaning, transforming and visualizing

## - Cleaning the data
## - Train/test split

To execute the train/test split properly, we need to do five things:

Drop all rows with a null value in the Decision column, and save the result as NOPrediction: a dataset that will contain all known values for the decision

Visualize the data using scatter and boxplots of several variables in the y-axis and the decision on the x-axis

Get the subset of coffeeData with null values in the Decision column, and save that subset as Prediction

Divide the NOPrediction subset into X and y, and then further divide those subsets into train and test subsets for X and y respectively

Create dummy variables to deal with categorical inputs

## - Visualize the data

![image](https://user-images.githubusercontent.com/86930309/227389110-e3312092-4a90-4e66-9930-8273332e0fca.png)

There is a wide range of customers that spent money last week on the coffee and that said yes they would buy the hidden farm coffee. The median was 40 dollars. A majority of the customers that said no they would not buy the hidden farm coffee was from 0-30 dollars with a median of 25 dollars.

## 3. Modelling

## - Model 1: Entropy model - no max_depth
## - Model 2: Gini impurity model - no max_depth
## - Model 3: Entropy model - max depth 3
## - Model 4: Gini impurity model - max depth 3

## 4. Evaluating and concluding

## - How many customers will buy Hidden Farm coffee?

Only 69.23 % would potentially buy the Hiddden Farm coffee by our gini model with a max depth of 3.

## - Decision

The prediction is very close to our requirement. I would say yes but we should do another model to insure this is predicting customer behavior correctly. Now we will run a random forrest model which uses lots of trees with similar properties to predict. They are great at combating over-fitting.

## 5. Random Forest

## - Import necessary modules
## - Model

The RF model predicts a higher rate of potenital customers that will buy the hidden coffee of 82.89%.

## - Revise conclusion

The random forest is the best model. Its accuracy score is relevent compared to the others and predicts that more customers would potiental purchase the Hidden Farm coffee. Given that the other model predicted that 69.23% would purchase the coffee and the random forest model predicted 82.89%, I would recommend that they go ahead and create a contract with Hidden Farms to produce the coffee.
