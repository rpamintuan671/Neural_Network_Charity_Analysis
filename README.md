# Neural Network Charity Analysis

## Overview:
AlphabetSoup is a non-profit foundation who helps environmental concious organizations with seed money or invenvestments. Alphabet Soup provided a CSV file with over 34,0000 organizations that have received their funding over the years.  The purpose of the analysis is to utilized machine learning by creating binary classifier that is capable of predicting success rate on Alphabet Soup applicants for funding. 

The metadata consist of the following columns before cleaning, processing, training and evaluating the data to utilizing neural network deep learning model.  predict success rate in a potential investment.

* **EIN** and **NAME**—Identification columns
* **APPLICATION_TYPE**—Alphabet Soup application type
* **AFFILIATION**—Affiliated sector of industry
* **CLASSIFICATION**—Government organization classification
* **USE_CASE**—Use case for funding
* **ORGANIZATION**—Organization type
* **STATUS**—Active status
* **INCOME_AMT**—Income classification
* **SPECIAL_CONSIDERATIONS**—Special consideration for application
* **ASK_AMT**—Funding amount requested
* **IS_SUCCESSFUL**—Was the money used effectively


## Resources Utilized to Complete Analysis
Data Sources: charity_data.CSV
Languages: Python
Python Dependencies: scikit-learn, pandas, tensorflow, os
Tools: MS Excel


## Results:

### Data Preprocessing
* **What variable(s) are considered the target(s) for the model?** The "IS_SUCCESSFUL" column is the target as it means that Alphabet Soup investment were use effectively.This target variable is the dependent variable, y.
* **What variable(s) are considered to be the features for the model?** The following variables are considered to be the features for the model: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT. These variables are the independent variables, x.
* **What variable(s) are neither targets nor features, and should be removed from the input data?** The identification columns EIN and NAME were dropped, as they are not beneficial when completing the analysis.

### Compiling, Training, and Evaluating the Model
* **How many neurons, layers, and activation functions were selected for the neural network model, and why?** For the deep neural network model, 100 neurons were in the first hidden layer and 30 neurons were in the second hidden layer. The ReLU activation function was utilized on both hidden layers. An advantage for using the ReLU activation function is that it identifies nonlinear characteristics from the input values. If the output of the linear transformation is less than 0, the neurons will be deactivated. 
* **Was target model performance achieved?** Performance of 75% accuracy was not achieved by the target model, as it attained 73%. 
* **What steps were taken to try and increase model performance?** In an attempt to optimize model performance, a third hidden layer was added with 15 neurons and the activation functions were adjusted. The first hidden layer maintained the ReLU activation function, however the second and third layers utilized the sigmoid activation function. Unfortunately, performance of 75% was not achieved by the optimized model. 


## Summary
An attempt to optimize the model 3 times but the expectation 75% performance was not achieved. It is recommended to adjust the number of hidden layers and neurons, along with the corresponding activation functions for each layer.