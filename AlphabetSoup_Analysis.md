# Overview
The purpose of the analysis is to help the charity, Alphabet Soup, select applicants for funding which have the best chance of success. 

Using predictive analysis in this way help the business maximize the efectivness of their funding by focusing their limited resources on projects most likely to succeed.

# Results

## Data Preprocessing

* **What variable(s) are the target(s) for your model?**
    * The target variable for this dataset is "IS_SUCCESSFUL". This vairaible is an indication of whether the funding provided was used successfully or not
* **What variable(s) are the features for your model?**
    * The variables included as the features of my model were as follows:
        * APPLICATION_TYPE—Alphabet Soup application type
        * AFFILIATION—Affiliated sector of industry
        * CLASSIFICATION—Government organization classification
        * USE_CASE—Use case for funding
        * ORGANIZATION—Organization type
        * STATUS—Active status
        * INCOME_AMT—Income classification
        * SPECIAL_CONSIDERATIONS—Special considerations for application
        * ASK_AMT—Funding amount requested

* **What variable(s) should be removed from the input data because they are neither targets nor features?**

    * Variables EIN and NAME were tremoved from the input data because they are identification columns and would provide no value to the training of the model

## Compiling, Training, and Evaluating the Model

**How many neurons, layers, and activation functions did you select for your neural network model, and why?**

For the initial attemp at training the model, the were two hidden layers with six neurons each both inpot layers used the ReLu activation function while the out put layer used a sigmoid actication function.

The ReLu activation function was used as a standard first step for training the data. The sigmoid function was used becuase were are tryng to predict a binary outcome - if the funding was successful or not.

**Were you able to achieve the target model performance?**

The highest accuracy score achieved for all three attempts was about 73% which is below the traget model performance

**What steps did you take in your attempts to increase model performance?**

For attempt #2, a third hidden layer was added and the numbet of neurons for each layer was increased to 10 units

For attempt #3, the activation function of the first hidden layer was changed to leaky_relu and he number of neurons for the first hidden layer was updated to 31 to match a best practice principle sourced from [this kaggle article](https://www.kaggle.com/discussions/general/321114)

# Summary

At about 73% accuracy, the model used was only moderately successful in  predicting whether a loan would be successful or not. 

In a future iteration, I would want to use a random forest model to train this dataset for two reasons. First, random forest models have been shown to be stronger that individual decision trees. They also provide more visibility into how and why certain predictions were made. This may be useful to the alphabet soup charity of they need to explain why some projects were approved over others.