# Telecom Churn Prediction Case Study 

### Problem Statement <BR>
In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business goal. To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. In this project, you will analyze customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn.<BR>

### Goal <BR>
To build predictive models to identify customers at high risk of churn so that the company can take action steps such as providing special plans, discounts on recharge etc. To identify important variables that are strong predictors of churn. These variables may also indicate why customers choose to switch to other networks. To recommend strategies to manage customer churn based on your observations.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- The main objective of this analysis is to create a ML model that identifies customers at high risk of churn so that the company can take action steps such as providing special plans, discounts on recharge etc. and to identify important variables that are strong predictors of churn (variable name churn_probablity). 
- Steps followed for this analysis: 
  1. Reading and understanding of the Data
     - Input dataset used for this analysis had 69999 rows and 172 columns
  2. Missing value / data cleaning treatment
     - The data cleaning step included
        1. Removing columns having missing value greater than 70% 
        2. Fixing missing value issues by '0'
        3. Removing columns having same value as those do not have any variation
        4. Remove columns which are not required for analysis
  3. Feature Engineering
     - Creating new variables based on existing variables
  4. Visualising the data - univariate, bivariate, correlation analysis
     -  Created different plots to understand the relationship between different sets of variables
  5. Outlier treatment
     -  Caping high column values based on threshold
  3. Data preparation for Modeling
        1. Splitting data into Training and Test sets at 70% (for training data) and 30% (for evaluating data) ratio respectively
        3. Rescaling features using Standard Scaler technique so that variables can have comparable scale 
  4. Building Different Models (Logistic regression with PCA,Random Forest,XG Boost )
      - Tried different models and selected logistic regression as final model based on sensitivity / recall criteria
  5. Feature selection
      - Selected important features based on coeeficient values 
  6. Making prediction using final model
      - Final model applied on test dataset
  7. Final Model Building
      - Final logistic regression model is created based on selected features. This gives 0.0960 as Kaggel score 
  8. Summary
      - The customers who satisfies one or more criteria mentioned below, have higher probability of churn:
        - have done lower amount of recharge compared to previous months
        - have used more roaming outgoing compared to previous month
        - have lower amount local incoming and outgoing usage
        - have done late recharge compared to previous months
        - have lower incoming call (of any type) usage
          
     - Telecom company needs to pay attention to the factors mentioned above and should come up with better offer for customers


   
 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
      - The customers who satisfies one or more criteria mentioned below, have higher probability of churn:
        - have done lower amount of recharge compared to previous months
        - have used more roaming outgoing compared to previous month
        - have lower amount local incoming and outgoing usage
        - have done late recharge compared to previous months
        - have lower incoming call (of any type) usage
        
     - Telecom company needs to pay attention to the factors mentioned above and should come up with better offer for customers

  

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.0 and different in-built packages
- Jupyter notebook
- Exploratory Data Anlysis (EDA) Concept
- Logistic regression, Random Forest, XGBoost, PCA Concept

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements

- IIIT Bangalore
- Upgrad 


## Contact
Created by alokkmukherji@gmail.com 


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
