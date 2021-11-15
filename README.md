# Neural_Network_Charity_Analysis
Business Funding Analysis with Neural Networks

## Overview of Project
To use Neural Networks and Machine Learning to create a binary classifier that is able to determine successful applicants after being funded by Alphabet Soup by creating a neural network that will be trained and optimized over iterations.

## Results

- Data Preprocessing

The variable that was considered a target for the model was "IS_SUCCESSFUL" variable which was obviously chosen since it was the ultimate goal of the model to determine if an applicant was funded or not. Then the "APPLICATION_TYPE", "CLASSIFICATION" and "ASK_AMT" were considered the features of the model since they were what the Alphabet Soup and the government classified themselves respectively, and the "ASK_AMT" was what levels of funding applicants were asking for. Finally, we could drop the "STATUS" variable since whether the applicant was active or not did not really seem relevant to whether its overall application was successful or not.

- Compiling, Training, and Evaluating the Model

The original model called for 2 hidden layers with 80 and 50 neurons respectively, and the standard relu model for the hidden layers with the sigmoid function for the outer layers. The two hidden layers were accounting the for two major features in the model, with the neurons selected to hopefully reflect all the factors within those features. Unfortunately, we were unable to achieve our target model performance of around 75% with those original parameters, which meant more optimizations were required. Subsequent optimizations were made increasing the neurons, hidden layers and changing the model of the activation function as well as manipulating the bins, but they were unsuccessful in terms of increasing optimization.

## Summary

Unfortunately, the current deep learning model used was unsuccessful in terms of trying to go above 75% of model performance. Most optimizations used were marginal at best in terms of improving the accuracy, but the loss was still close to 50% on all optimizations used. Overall, the biggest factor that could contribute to the failure in obtaining an accurate model was the large number of categorical variables, which could contribute in making results more disparate, preventing an accurate model. In the future, using a Support Vector Model might work better in the future, since a Support Vector Models would help in two linearly separable groups since our results are either a successful result or unsuccessful result.