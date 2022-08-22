# Charity Analysis using Neural Networks

## Overview
The purpose of the module is to demonstrate how simple Neural Networks can train a machine learning model. Different models yield different outcomes, such as having multiple hidden layers and/or having multiple nodes per hidden layer. By applying various models to our data, we can predict the outcome with increased accuracy.

## Results

*What variable(s) are considered the target(s) for your model?*

The targetted variable is the "Is Successful" in the dataset because this show which charities had a positive outcome.

*What variable(s) are considered to be the features for your model?*

Featured variables of interest seem to be "Application Type" and "Classfication".

*What variable(s) are neither targets nor features, and should be removed from the input data?*

Variables that provided little to no value would be: -EIN -Name -Status -Special Considerations

*How many neurons, layers, and activation functions did you select for your neural network model, and why?*

For model 1, I increase the number of hidden layers to hold 4 instead of 2. For all hidden layers, I used 8 nodes. Lastly, the activation function for all input hidden layers still used "Relu". Generally speaking, increasing the hidden layers and nodes per hidden layers is expected to improve the accuracy at the cost of increase computer resources and risk of overfitting. Furthermore, I decided to leave the activation function of "Relu".

The output layer activation function was changed from sigmoid to linear to see if that would improve results.

![Model1](https://user-images.githubusercontent.com/102441140/185858428-86c98b6d-7ebf-4782-be29-27153a659cb2.png)

For model 2, I went back to using 2 hidden layers but increased the nodes. I also changed the activation function back to "sigmoid" since "linear did not have a drastic impact on model 1.

![Model2](https://user-images.githubusercontent.com/102441140/185859058-10068c78-59cd-4996-b7e4-00412bd79134.png)

For model 3, I used 3 hidden layers with the 1st layer having 3 times the nodes as the number of inputs, 2nd layer having 2times the nodes as inputs layers, and the 3rd layer having the same number of nodes as the number of inputs. I also kept the activation function back to "sigmoid".

![Model3](https://user-images.githubusercontent.com/102441140/185859648-2f4b9867-7091-4f40-aad9-d6ec60e3fbba.png)

*Were you able to achieve the target model performance?*

Unfortunately, I was not able to improve the model to achieve the 75% targetted performance. This doesn't mean that the model cannot achieve it, but the three limits I used were not sufficient. The best way would be to find the optimal the number of hidden layers and nodes and apply it. Or to preprocess the data in a different way.

*What steps did you take to try and increase model performance?*

I tried to use different number of hidden layers, I changed the number of nodes in each layer, and I also tried different combinations of nodes and layers to try to optimize a model.


## Summary

The final yield after three attempts of optimization has left us with an approximate accuracy of 71% with a 58% loss of data. A major takeaway is that it is important to remove variables that provide little to no value to training model so the machine learning model only uses the necessary data and isnt slowed down. A recommendation I would do to further improve the model is to use unsupervised machine learning model to see what variables are important. Another recommendation is to study the concept of what's happening on a deeper level in order to devise the optimal number of hidden layers and nodes to use in a model.
