# Neural_Network_Charity_Analysis

## Overview 

Explain the purpose of this analysis.

Using a deep learning neural network, we want to see if we can create a model that is able to classify if an applicant will be successful if funded by Alphabet Soup.

## Results: 

Data Preprocessing
What variable(s) are considered the target(s) for your model?

The target for this model is the IS_SUCCESSFUL column



What variable(s) are considered to be the features for your model?

The variables that are considered as the features are: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT.

![Screen Shot 2022-02-28 at 12 30 29 AM](https://user-images.githubusercontent.com/87248687/155929285-e34ca551-6fdf-44db-81eb-d9740a30b3b9.png)

What variable(s) are neither targets nor features, and should be removed from the input data?

The EIN and NAME columns are neither targets or features and provide no benefit, so we removed those 2 from the input data.

![Screen Shot 2022-02-28 at 12 31 30 AM](https://user-images.githubusercontent.com/87248687/155929371-e2b423b6-67f8-47d2-950d-8d0ed7118896.png)


Compiling, Training, and Evaluating the Model
How many neurons, layers, and activation functions did you select for your neural network model, and why?

For our model, we have one input layer, 2 hidden layers (with 80 and 30 neurons respectively), and an outputlayer.  For the 2 hidden layers, we used the relu activation function and we used the sigmoid function for our output since we're expecting a binary outcome.

![Screen Shot 2022-02-28 at 12 32 04 AM](https://user-images.githubusercontent.com/87248687/155929418-76698d78-1de2-420d-85d0-875a6ed32f7b.png)


Were you able to achieve the target model performance?

We didn't achieve our target model performance of 75% accuracy.  Our model achieved only 72.4% accuracy.

![Screen Shot 2022-02-28 at 12 22 46 AM](https://user-images.githubusercontent.com/87248687/155928573-d1e250bf-3373-4e5b-bcf0-687c4ea6b5c5.png)

What steps did you take to try and increase model performance?

In efforts to try and optimize our model's performance, we tried adding an additional hidden layer, we tried increasing the epochs from 100 to 200, and we even tried adding additional neurons to our original 2 hidden layers.  None of these optimizations techniques were able to improve our model to our goal of 75% accuracy unfortunately.
## Summary

Based on the results of our deep learning model, I think it's safe to say that this particular model did not perform well enough.  Since this is a classification problem, we could try using a supervised machine learning model such as a Random Forestr Classifier. Another route we could do could be to provide more data to our existing model to see if it could help provide better results.

