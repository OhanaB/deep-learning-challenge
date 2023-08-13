# deep-learning-challenge



#Background
The nonprofit foundation Alphabet Soup wants a tool that can help it select the applicants for funding with the best chance of success in their ventures. With your knowledge of machine learning and neural networks, you’ll use the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

#Results

#Data Preprocessing

Target Variable(s) for the model:
IS_SUCCESSFUL: This variable denotes whether the funded organizations used the funds effectively.
Feature Variables for the model:
EIN and NAME—Identification columns
APPLICATION_TYPE—Alphabet Soup application type
AFFILIATION—Affiliated sector of industry
CLASSIFICATION—Government organisation classification
USE_CASE—Use case for funding
ORGANIZATION—Organisation type
STATUS—Active status
INCOME_AMT—Income classification
SPECIAL_CONSIDERATIONS—Special considerations for application
ASK_AMT—Funding amount requested
IS_SUCCESSFUL—Was the money used effectively

Variables Removed:
EIN and NAME: These are identification columns and they were removed fro mthe data 

For all three models, the following details apply:
#1. First Model
APPLICATION_TYPE cutoff = 600
CLASSIFICATION cutoff = 600
layer1 = 15
Activation Function = tanh
layer2 = 7
Activation Function = relu
The model evaluated the data in 268 batches. It achieved an accuracy of roughly 72.73%. The model's loss was 0.5737.

#2. Second Model
APPLICATION_TYPE cutoff = 600
CLASSIFICATION cutoff = 1000
layer1 = 10
Activation Function = relu
layer2 = 8 
Activation Function = sigmoid
layer3 = 6
Activation function = sigmoid
The model was evaluated on 268 batches of data. It achieved a prediction accuracy of about 72.93%, with a loss score of 
0.5529. 

#3. Third Model
APPLICATION_TYPE cutoff = 600
CLASSIFICATION cutoff = 300
layer1 = 18
Activation Function = relu
layer2 = 12
Activation Function = relu
layer3 = 21
Activation function = sigmoid
The model was evaluated on 268 batches of data. It achieved a prediction accuracy of approximately 72.97% with a loss value of 0.5557.


#Summary

Throughout the process, optimization techniques were applied to the deep learning models with the aim of surpassing a predictive accuracy of 75%. Unfortunately, the desired benchmark was not achieved. The accuracies of the models consistently hovered around the 72-73% range across all trials. While these results are promising and provide valuable insights, they fall slightly short of the target. This could be attributed to various factors such as the complexity of the dataset, the potential need for additional feature engineering, or the possibility that the current model architecture isn't the most suitable for this particular dataset.

#Recommendation
Given that the 75% accuracy couldn't be met with the current configurations, it might be beneficial to explore alternative deep learning architectures to push this accuracy higher, a more detailed exploration of the data might be beneficial.It may be worth exploring alternative modeling techniques. Adjustments such as modifying dropout layers, experimenting with different activation functions, or tweaking the number of layers and neurons might be the key to optimizing the model further.
