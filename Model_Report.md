## Overview of the analysis:

The non-profit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With our knowledge of machine learning and neural networks, we will use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

## Compile, Train, and Evaluate the Model
Using my knowledge of TensorFlow and Keras, I designed a neural network model to create a binary classification model that can predict if an Alphabet Soup-funded organization will be successful based on the features in the dataset. Once I completed this step, I compiled, trained, and evaluated my binary classification model to calculate the model’s loss and accuracy.
![image](https://github.com/kaurn6538/deep-learning-challenge/assets/98873779/99a7e8fd-4c62-4a11-83e1-11ee111256fb)
![image](https://github.com/kaurn6538/deep-learning-challenge/assets/98873779/bd3472ec-08a8-49b0-925e-d76ac5de90ff)

## Optimize the Model
Using my knowledge of TensorFlow, I optimized my model to achieve a target predictive accuracy higher than 75%. This was achieved by Drop the non-beneficial ID columns, ASK_AMT of the database, adding more neurons to the hidden layers and more epochs.

Second attempt
For the second attempt, I used the same activation function relu, however increased the  number of nodes for each layer, as I felt that it would help with achieving a higher than 75% accuracy. See image below.


First attempt
For the first attempt, I used the relu activation function. There were two layers - layer 1 had 8 hidden nodes and layer 2 had 5 hidden nodes. Epochs was 100. For the outer layer, I used sigmoid.

![image](https://github.com/kaurn6538/deep-learning-challenge/assets/98873779/9190d071-76c5-463d-8f36-5905fb11d349)
![image](https://github.com/kaurn6538/deep-learning-challenge/assets/98873779/2ff9bc98-a355-487f-86f3-d4d7403f4829)

## Final try
In the second attempt achieved 73% predictive accuracy.I used the same activation function relu, however increased the number of layers and the number of nodes for each layer, as I felt that it would help with achieving a higher than 75% accuracy. See image below.
![image](https://github.com/kaurn6538/deep-learning-challenge/assets/98873779/9ccb22b5-3e45-4d8c-8323-14c206d8db28)

![image](https://github.com/kaurn6538/deep-learning-challenge/assets/98873779/9159e18c-14f9-4f4c-801c-8cb2da8f2e47)


## Data Preprocessing

1. What variable(s) are the target(s) for your model?
*    The target variable is the 'IS_SUCCESSFUL' column from application_df
2. What variable(s) are the features for your model?
*    The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe
3. What variable(s) should be removed from the input data because they are neither targets nor features?
*    Both 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.
Compiling, Training, and Evaluating the Model
4. How many neurons, layers, and activation functions did you select for your neural network model, and why?
*    In the first attempt, i used 8 hidden_nodes_layer1 and 5 hidden_nodes_layer2 -- these were just random guesses from which to iterate upon in the second try.
5. Were you able to achieve the target model performance?
*    I was not able to achieve the 75% model accuracy target
6. What steps did you take in your attempts to increase model performance?
*    I added more layers, removed more columns, added additional hidden nodes, and switched up the activation functions associated with each layer in an attempt to achieve higher model accuracy.
7. What steps did you take in your attempts to increase model performance?

     § I will attempt to:

     § Adjust the input data to ensure that no variables or outliers are causing confusion in the model, such as:

     § Dropping more or fewer columns.

     § Creating more bins for rare occurrences in columns.

     § Increasing or decreasing the number of values for each bin.

     § Add more neurons to a hidden layer.

     § Add more hidden layers.

    § Use different activation functions for the hidden layers.

    § Add or reduce the number of epochs to the training regimen.

## Summary: 

Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.

Overall, the deep learning model was around 73% accurate in predicting the classification problem. Using a model with greater correlation between input and output would likely result in higher prediction accuracy. This could be achieved by doing additional data cleanup up front, as well as by using a model with different activation functions and iterating until higher accuracy is reached.
