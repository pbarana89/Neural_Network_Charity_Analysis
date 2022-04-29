# Neural_Network_Charity_Analysis
- The goal of this project was to use the knowledge of Machine Learning to use Neural Networks to help create a prediction model. Using information from the dataset of over 34,000 organizations, we were able to create a classifier that would be able to predict if applicants would be successful if funded by Alphabet Soup.

## Overview of the Analysis

- The target variable of our model was the "Is Successful?" variable, on which applications had been successful in the past.

- Our feature variables were application type, affiliation, classification, organization status, income amount, special consideration, and ask amount. In additional models we added an earned income variable as well to see if that helped the model become more precise.

- We chose to remove the EIN and Name features as they would have hindered the model.

- For the initial model our model had 43 input features with 80 neurons, 2 hidden layers with relu activation functions, and for the output layer we chose sigmond as we were answering a yes or no question, we felt like this would be the strongest choices as they are meant for binary classification.

- The model and subsequent tries were not able to reach the threshold of 75% accuracy. The initial model returned an accuracy of 72.5% and our best accuracy after multiple changes was to return 73.1% accuracy.

- Using the keras hypertuner package, we were able to try and determine the most optimal model for 3 variations. Our first was to use the hyper tuner to run trials with over 180 eligible different variations of the neuron, layer, and activation choices. Once this was complete, we trained the "optimal model" and this returned an accuracy of 73%. Then we changed the amount of inputs to the classification and application type features and engineered an earned income feature and then ran it through the hyper tuner. This also returned accuracy to 73%. Finally, we changed the ranges for the features again and that got an optimal accuracy of 73.1%.

### Summary of the Analysis
- We were very happy with the output of the model as it gave us good insights. We were able to create a predictive model that returned 73% accuracy. With more data and more training, it could very well become a very accurate model. The sheer amount of time and resources that this model did required leaves something to be desired. It would be interesting to run a RandomForest model and see if it could be as accurate if not better and be a much more accessible resource.