# Neural_Network_Charity_Analysis

## Overview of Analysis

The purpose of this analysis is to use our knowledge of Tensorflow to design a neural network/deep learning model, and to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset provided. Once the binary classification model has been created, it will then be compiled, trained, and evaulated to calculate the model's loss and accuracy.

## Results

### Data Preprocessing

- What variables are considered the targets for your model? 
  
  The column, "IS_SUCCESSFUL" was considered to be the target variable for our neural network model because this column states wheteher or not the charity donation was           effective or not.

- What variables are considered to be the features for your model?
  
  The following columns are the features for our model: "APPLICATION_TYPE", "AFFILIATION", "CLASSIFICATION", "USE_CASE", "ORGANIZATION", "STATUS", "INCOME_AMT",                   "SPECIAL_CONSIDERATIONS", and "ASK_AMT".

- What variables are neither targets nor features, and should be removed from the input data?
  
  The columns, "EIN" and "NAME" are neither targets nor features because they contain identification information, so they should be removed from the input data. 

### Compiling, Training, and Evauluating the Model

- How many neurons, layers and activation functions did you select for your neural network model, and why?
  
  This neural network model consists of two hidden layers with 80 neurons for the first hidden layer and 30 neurons for the second hidden layer. The first and second hidden       layers used the relu activation function. However, the sigmoid acitvation function was used for the output layer. For the compilation, the optimizer is adam and the loss       function is binary_crossentropy. 

- Were you able to achieve the target model performance?
  
  Unfortunately, the model was unable to achieve its target performance of 75% and fell just short at around 73%.

- What steps did you take to try and increase your model performance?
  
  The first step I did to try to increase the model's performance was that I eliminated more columns that I felt were unncessary, such as the "STATUS" and                         "SPECIAL_CONSIDERATIONS" columns and then reran the model.

![optimization1](https://user-images.githubusercontent.com/75760493/120914955-c17b9e00-c666-11eb-8479-d5230c6ee0b9.PNG)

![optimization1score](https://user-images.githubusercontent.com/75760493/120914968-d5270480-c666-11eb-9632-2c1a769f9ff9.PNG)

Since the accuracry was only ..... it still didn't reach the 75% target performance, I tried again but this time I increased the neurons for each hidden layer. I increased the neurons in first hidden layer from 80 to 100 neurons and the second hidden layer from 30 to 50 layers.

![optimization2](https://user-images.githubusercontent.com/75760493/120915124-99d90580-c667-11eb-86df-0af4b31a7c41.PNG)

![optimization2score](https://user-images.githubusercontent.com/75760493/120915129-a65d5e00-c667-11eb-9681-8347601c3a70.PNG)

Since the accuracry was only ..... it still didn't reach the 75% target performance,  I tried again but this time I increased the neurons for each hidden layer, along with adding two additional hidden layers. The first hidden layer had 100 neurons, the second hidden layer had 80 neurons, the third hidden layer had 50 neurons, and the fourth hidden layer had 30 neurons.

![optimization3](https://user-images.githubusercontent.com/75760493/120915206-271c5a00-c668-11eb-9bd3-f1f543e84bb6.PNG)

![optimization3score](https://user-images.githubusercontent.com/75760493/120915219-3c918400-c668-11eb-9da8-6d69af06e7c1.PNG)

Since the accuracry was only ..... it still didn't reach the 75% target performance,  I tried again but this time I reran the model with the tanh activation function for the output layer. 

![optimization4](https://user-images.githubusercontent.com/75760493/120915581-06550400-c66a-11eb-82e5-b5ed77895479.PNG)

![optimization4score](https://user-images.githubusercontent.com/75760493/120915597-1e2c8800-c66a-11eb-9c0c-8e26896acc8b.PNG)




## Summary
