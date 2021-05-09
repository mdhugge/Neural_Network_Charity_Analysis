# Neural Network Charity Analysis

## Overview of the analysis
Using machine learning and neural networks predictions are made to help Alphabet Soup determine where to make investments. A binary classifier is created that can predict if an applicant will be successful if funding is provided.

## Results

### Data Preprocessing

In order to achieve greater than 75% accuracy the following variables were used:

- The target variable for the model is whether the money is used effectively, this is represented by the IS_SUCCESSFUL variable.

- APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT, EIN and NAME are variables that are considered to be the features for this model.

- No variable was removed from the model.

### Compiling, Training, and Evaluating the Model

![Summary](https://github.com/mdhugge/Neural_Network_Charity_Analysis/blob/main/Images/Summary.png)

- This model has 2 hidden layers; the first layer has 80 neurons, and the second layer has 30 neurons. The two hidden layers use the relu activation function and the output layer uses the sigmoid activation function. A model usually has two to three times as many neurons as there are input features. Looking at the input variables in our initial model, 80 is a good start for the first layer and since it’s good to have a lower number of neurons in the following layers 30 is reasonable. 2 layers is also sufficient to decrease the computational power of the model. Using more complex activation functions for hidden layers than the output layer is recommended and is applied to this model.

![Performance](https://github.com/mdhugge/Neural_Network_Charity_Analysis/blob/main/Images/Performance.png)

- The model reached an accuracy of 79%, greater than the 75% target.

- In order to increase model performance I used the EIN and NAME variables as features and I used binning to incorporate them into the data. 

## Summary

By adding the EIN and NAME variables, which are identification variables I was able to increase the accuracy of the model. 

The data that is available to us is in tabular form as a result a random forest model with a sufficient number of estimators and tree depth may have similar accuracy to our model. A random forest model may achieve comparable predictive accuracy on large tabular data with less code and faster performance. 
