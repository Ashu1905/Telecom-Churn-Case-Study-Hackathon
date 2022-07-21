# Telecom Churn Case Study _(IIIT BANGLORE_2022)_ <br>
# `Ashwini Abhang`
## Problem Statement <br>
In the telecom industry, customers are able to choose from multiple service providers and actively switch from one operator to another. In this highly competitive market, the telecommunications industry experiences an average of 15-25% annual churn rate. Given the fact that it costs 5-10 times more to acquire a new customer than to retain an existing one, customer retention has now become even more important than customer acquisition.

For many incumbent operators, retaining high profitable customers is the number one business
goal. To reduce customer churn, telecom companies need to predict which customers are at high risk of churn. In this project, you will analyze customer-level data of a leading telecom firm, build predictive models to identify customers at high risk of churn.

In this competition, your goal is to build a machine learning model that is able to predict churning customers based on the features provided for their usage. <br>

## Objectives
The main goal of the case study is to build ML models to predict churn. The predictive model that you’re going to build will the following purposes:

It will be used to predict whether a high-value customer will churn or not, in near future (i.e. churn phase). By knowing this, the company can take action steps such as providing special plans, discounts on recharge etc.

It will be used to identify important variables that are strong predictors of churn. These variables may also indicate why customers choose to switch to other networks.

Even though overall accuracy will be your primary evaluation metric, you should also mention other metrics like precision, recall, etc. for the different models that can be used for evaluation purposes based on different business objectives. For example, in this problem statement, one business goal can be to build an ML model that identifies customers who'll definitely churn with more accuracy as compared to the ones who'll not churn. Make sure you mention which metric can be used in such scenarios.

## Recommend strategies to manage customer churn based on your observations.

## Data Understanding, Preparation, and Pre-Processing :
Data understanding, identification of potentially useful and non-useful attributes and variable importance and impact estimation
Data preparation, performing data cleaning, missing values imputation, outlier removal, and column level standardization (for e.g., date, etc.) into one format
 
## Exploratory Data Analysis :
Performing basic preliminary data analysis including finding the correlation between variables and scatter plots to identify relationships between variables
Performing advanced data analysis, including plotting relevant heatmaps, histograms, and basic clustering to find patterns in the data
 
## Feature Engineering and Variable Transformation :
Feature engineering and performing one or more methods on attributes that can lead to the creation of a new potentially useful variable; for e.g., day from the date
Variable transformation and applying categorical variable transformations to turn into numerical data and numerical variable transformations to scale data
 
## Model Selection, Model Building, and  Prediction :
Identifying the type of problem and making a list of decisive models from all available choices
Choosing a training mechanism; for e.g., cross-validation, etc., and tuning hyperparameters of each model
Testing each model on the respective model evaluation metric
Choosing the best model based on the fit of the data set and output variable
Using ensemble options to improve the efficacy based on the evaluation metric stated in the problem

## Conclusion:-
In this case study I have first handled the missing data with the help of various data pre-processing techniques such as sklearn's Iterative Imputer and standard scalar for standardisation of data. After pre-processing the data I performed Exploratory data analysis (EDA). During which I observed that the data was heavly imbalanced towards the '0' class.

I handledthis imbalanced data with the help of various sampling techniques like Synthetic Minority Over Sampling Technique with Edited Nearest Neighbours (SMOTEENN). After which I handled the outliers using the boxcox transformation.

Once the EDA was completed I performed Feature Engineering on the features to derive new features so as to enhance and consolidate the data and improve it's accuracy. After feature engineering I started with the Model Selection process in which I used Recursive Feature elimination(RFE) eliminating unimportant features. Here I used models like Logistic Regression, Random Forest, Support Vector Machine, Adaboost, CatBoost and LGBM.

I also used PCA for dimensionality reduction. Finally I used LGBM classifier over random forest as it had better recall than random forest. In the end I found out the feature importances of LGBM classifier and created a pipeline with it and observed train accuracy of `100%` and testing accuracy of `92.32%`


## Technologies Used
Jupyter Notebook

## Acknowledgements
- This project was inspired by IIIT Banglore

## Contact
Created by `[@Ashu1905]` - feel free to contact me!
