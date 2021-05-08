# Neural Network Charity Analysis

## Overview of the analysis
Using machine learning and neural networks predictions are made to help Alphabet Soup determine where to make investments. A binary classifier is created that can predict if an applicant will be successful if funding is provided.

## Results

### Data Preprocessing

In order to achieve greater the 75% accuracy the following variables were used:

- The target variable for the model is whether the money is used effectively, this is represented by the IS_SUCCESSFUL variable.

- APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, EIN and NAME are variables that are considered to be the features for this model.

- No variable was removed from the model.

### Compiling, Training, and Evaluating the Model

![Summary](https://github.com/mdhugge/Neural_Network_Charity_Analysis/blob/main/Images/Summary.png)

- This model has 2 hidden layers, the first layer has 80 neurons and the second layer has 30 neurons. The two hidden layers use the relu acitivation function and the output layer uses the sigmoid activation function. 

![Performance](https://github.com/mdhugge/Neural_Network_Charity_Analysis/blob/main/Images/Performance.png)

- The model reached an accuracy of 79%, greater than the 75% target.

- In order to increase model performace I use the EIN and NAME variables as features and I used binning to inocprate them into the data. 

## Summary

By adding the EIN and NAME varibales, which are indentification variables I was able to increase the accuracy of the model. 




