# Keystroke_Dynamics_Analysis

Cal Poly San Luis Obispo CSC 480 Project instructed by Dr. Rodrigo Canaan. 
Group Members: Joseph Haluska, Lee Conway, Saurav Gupta, Zack Soucek, Ryan  Takahashi
 

The goal of this project is to evaluate the practicality of a KNN and a nueral network classifier for keystroke analysis.

Code from https://www.kaggle.com/code/arjunsingh88/keystroke-dynamics-with-random-forest was used to help create several visualizations.
Code from https://www.kaggle.com/code/arjunsingh88/keystroke-dynamics-with-random-forest was used for the basis of the Binning KNN algorithm.
The libraries the KNN code uses is scikit learn for the KNN model, and numpy and pandas for the tables and data manipulation.
The visualization code mostly uses the matplotlib in combination with pandas.
The Nueral Network uses the torch library to build the Nueral Network.


This project is made of three different ipynb notebooks that can all be run on google colab. All you need to do is run them and the results we talk about within our paper will be reproduced.
Running the system will train and test the models automatically. There is really no user input so it is that simple. One thing we may want to implement in the future is the ability to have someone add themselves as a user to the training set. Then we could allow users to type a password and test on that. However, that is outside of the scope of the current project. Just running the notebooks is all we currently can do.

When the KNN_Classifier notebook is ran many models will be created in order to perform hyperparameterization. In doing so we determine the best K and the best parameters to use. The results are split into two sections: one section where the data was binned, the other the data has not been binned. The results are displayed as a table that displays the parameters, best k (as determined by GridSearchCV), the accuracy, and f1_weighted score. 
(NOTE: You may not want to run it yourself as training and doing the hyperparameter tuning takes quite a long time. However, you can just look at the notebook results within github).

The Nueral Network is very similar because you only need to click run on the notebook to get it to work. To view the results you can scroll to the bottom of the notebook to see the accuracy when we do our testing on the Nueral Network.

The last notebook is one where we kept visualizations of the data. These visualizations helped to give us an idea of the spread of the data and are explained within our paper. This is included as a way to showcase how we created the visualizations. Just to be clear, these are visualizations of the data, not of our results. 

