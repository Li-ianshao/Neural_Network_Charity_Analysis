# Neural Network Charity Analysis

## Overview
An analysis was done on data provided by Alphabet Soup to help determine which investments are most likely to prove successful.

## Results: 
### Data Preprocessing

What variable(s) are considered the target(s) for your model?

* IS_SUCCESSFUL

What variable(s) are considered to be the features for your model?

* APPLICATION_TYPE
* AFFILIATION
* CLASSIFICATION
* USE_CASE
* ORGANIZATION
* STATUS
* INCOME_AMOUNT
* ASK_AMT

What variable(s) are neither targets nor features, and should be removed from the input data?

* EIN
* NAME
* SPECIAL_CONSIDERATIONS


### Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?

* 4 layers
* Layer 1:
    - 120 neurons were used because its ~3x the input features
    - Rectified Linear Unit (ReLU) activation function was used.
* Layer 2:
    - 60 neurons
    - ReLU activation function
* Layer 3:
    - 30 neurons
    - tanh activation function 
* Output Layer:
    - tanh activation function

Were you able to achieve the target model performance?

* Target model performance of >75% was not reached.
* 73% accuracy and 56% loss

What steps did you take to try and increase model performance?

* remove a noisy variable from SPECIAL_CONSIDERATIONS column



## Summary:

Overall the deep learning model was not very sucessfull in predicting the success of an application. With a max accuracay score of 73% reached, and even that with a high loss value of 56%, the benefits of this model were few. Training the model and changing various components in order to attempt optimization was also quite time-consuming.
