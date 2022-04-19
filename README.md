# Welcome to our data science project page!:wave:


## About this project
This is a mini-project for SC1015. We will be using data based on information about patients doing cardiovascular disease examination.


## Contributors

- @Sele3 
- @lldzlldz 
- @Awon001

## Context
According to the World Health Organization, the world’s biggest killer is ischaemic heart disease, responsible for 16% of the world’s total deaths. Since 2000, the largest increase in deaths has been for this disease, rising by more than 2 million to 8.9 million deaths in 2019. Stroke and chronic obstructive pulmonary disease are the 2nd and 3rd leading causes of death, responsible for approximately 11% and 6% of total deaths respectively.

![Leading causes of death globally](https://lh3.googleusercontent.com/tsJMRht1HYVqW7F7dweI8Yb97ZdMoGrRuNzkIKbZOZ2DOf80e7em-V3XkGgO0ufCLZVCTB04p0PJBq0c3JKc-N5WeOnPAgOL3_-tBrE54XQeoynI_U9svy1LLrIRZ6-_1dRUMOM)



## Problem Definition

1. To see how we can prevent chronic diseases by investigating the factors that cause heart disease. 
2. To investigate if the conditions causing heart diesase also causes other diseases


## Project Summary 
#### Part 1 [Heart Disease](https://github.com/lldzlldz/Data-science-project/blob/main/heart_disease_EDA.ipynb)

The 1st half of our project involves finding the factors that causes heart disease. We first obtain a dataset of 70000 patients containing their medical information and whether they have heart disease.  
Afterwards, we used 4 different classification models to predict whether a patient has heart disease.

#### Part 2 [Stroke](https://github.com/lldzlldz/Data-science-project/blob/main/stroke_EDA.ipynb)

The 2nd half of our project involves finding whether conditions causing heart disease also causes other diseases. Our area of investigation will be on stroke, the second leading cause of death for chronic diseases. We do so by obtaining a dataset of 43400 patients, then using our model to predict whether their current health condition make them at risk of getting heart disease. We then attempt to find out whether there is any relationship between the two diseases. Subsequently, we attempt to find a causal relationship between the two.



## Models Used
1. Binary Classification
2. Random Forest
3. Logisitic Regression 
4. XGBoost:white_check_mark:

# Conclusion

## What did we learn from this project?
- How to find a good dataset:sob:
    - [some datasets mainly had categorical variables](https://www.kaggle.com/datasets/shivamb/netflix-shows)
    - [others had too many obscure data that was only applicable to cardiovascular disease](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- Heart disease is the leading cause of death 
    - Learnt some new terms like systolic blood pressure and diastolic blood pressure 
- How to use 2 different datasets(stroke and heart disease) to come up with better insights
    - How to find a dataset for both stroke and heart disease that has health data we can work with(eg height, weight, age, glucose level) instead of data specific to one dataset(eg exercise induced angina, the slope of the peak exercise ST segment)

## Addtional things that we learnt beyond this course
- How to implement the different machine learning models(Binary Classification, Random Forest, Logistic Regression, XGBoost)
    - How to use hyperparameter tuning in XGBoost
    - Different machine learning models are better suited for different types of data
    - Some machine learning models take very long(a few min) to learn compared to others(a few seconds)
- We learnt about hypothesis testing (Chi-squared test)
    - Chi-squared test can be used to determine whether there is a relationship between categorical variables
    - We define the null hypothesis (H0) and alternative hyperpothesis (H1), then subsequently run a chi-squared test on the data
    - If the p-value is below the significance level of 0.05, then we reject the null hypothesis and accept the alternative hypothesis
- We also learnt about forming causality models using Bayesian Networks (bnlearn)
    - We can use directed acrylic graphs to represent relationship between variables
    - A directed edge E(V, W) indicates that W is conditionally dependent on V
    - We can subsequently calcuate conditional probabilty on our model to determine whether there may be a causal relationship
- Better ways to check which machine learning model is the most appropriate(besides using accuracy)
    - We used Precision, Accuracy, Recall, F1 Score

## Data sets used
- https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset
- https://www.kaggle.com/fedesoriano/stroke-prediction-dataset 

## Other references
- https://www.who.int/news-room/fact-sheets/detail/the-top-10-causes-of-death
- https://www.cdc.gov/stroke/risk_factors.htm?CDC_AA_refVal=https%3A%2F%2Fwww.cdc.gov%2Fstroke%2Fconditions.htm
- https://builtin.com/data-science/random-forest-algorithm
- https://learn.g2.com/logistic-regression
- https://machinelearningmastery.com/gentle-introduction-xgboost-applied-machine-learning/
- https://towardsdatascience.com/why-random-forest-is-my-favorite-machine-learning-model-b97651fa3706
- https://scikit-learn.org/stable/modules/tree.html#
- https://www.health.harvard.edu/heart-health/throughout-life-heart-attacks-are-twice-as-common-in-men-than-women#:~:text=Researchers%20found%20that%20throughout%20life,mass%20index%2C%20and%20physical%20activity
- https://www.hopkinsmedicine.org/health/wellness-and-prevention/weight-a-silent-heart-risk
- https://ochsnerlg.org/about-us/news/how-obesity-affects-stroke-risk
- https://ochsnerlg.org/about-us/news/how-obesity-affects-stroke-risk
- https://worldpopulationreview.com/countries/life-expectancy
- https://www.bloomberg.com/news/articles/2018-09-19/u-s-near-bottom-of-health-index-hong-kong-and-singapore-at-top
- https://www.cdc.gov/nchs/data/nhsr/nhsr112.pdf
- https://www.thelancet.com/journals/langlo/article/PIIS2214-109X(18)30357-7/fulltext
