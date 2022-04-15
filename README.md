def minimax(board, maxSymbol, minSymbol, depth, isMaximizing):
    ''' Minimax algorithm for the recursion
    '''
    # Terminal conditions for recursion
    # Fill in the missing conditions to stop the recursion
    if (isWinner(board, maxSymbol)):
        return 10
    elif (isWinner(board, minSymbol)):
        return -10
    elif isBoardFull(board):
        return 0
    # You may use the isWinner and isBoardFull functions if you want
    
    # Keep track of scores at this depth
    scores = []
    available = [position for position, value in board.items() if value == " "]
    
    # Go through all available positions
    for space in available:
    # Fill in all the missing pieces in this code segment
        # Simulate the appropriate move
        if (isMaximizing):
            board[space] = minSymbol
        else:
            board[space] = maxSymbol
        # Find the score for the move
        scores.append(minimax(board, maxSymbol, minSymbol, depth+1, not isMaximizing))
        # Undo the move for simulation
        board[space] = " "
            
    # Return max or min as per the level
    # Fill in the return logic for recursion as per level
    if(isMaximizing):
        return max(scores)
    else:
        return min(scores)
    
    # Remove the following exception when you complete this function
    #raise NotImplementedError
3
4
0 1 1 1
1 0 1 0
1 1 0 1
1 0 1 0
2FA is a security feature that forces users to provide at least 2 proofs of authentication to login.


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
Based on a given set of data, we would like to predict the likelihood of getting cardiovascular disease

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
- How to implement the different machine learning models(Binary Classification, Random Forest, Logistic Regression, XGBoost)
    - How to use hyperparameter tuning in XGBoost
    - Different machine learning models are better suited for different types of data
    - Some machine learning models take very long(a few min) to learn compared to others(a few seconds)
- How to use 2 different datasets(stroke and heart disease) to come up with better insights
    - How to find a dataset for both stroke and heart disease that has health data we can work with(eg height, weight, age, glucose level) instead of data specific to one dataset(eg exercise induced angina, the slope of the peak exercise ST segment)
- How to work with other people 

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

