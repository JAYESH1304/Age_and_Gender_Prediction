# Age and Gender Prediction

This repository contains code for a Convolutional Neural Network (CNN) model trained from scratch on the UTK Face Dataset built using the TensorFlow framework. The model is capable of predicting the age and gender of a person based on their facial images.

# Dataset
The UTK Face Dataset consists of over 20,000 labeled images of faces, including age and gender annotations. The dataset covers a wide range of ages, from 0 to 116 years, and diverse gender categories. The images are preprocessed and split into training, validation, and testing sets.

# Model Architecture

The model consists of the following components:

Input layer: Accepts the input images with the specified input_shape.
Convolutional layers: Four convolutional layers with increasing filter sizes and ReLU activation functions, followed by max pooling layers to reduce spatial dimensions.
Flatten layer: Flattens the output of the last convolutional layer to a 1-dimensional vector.
Fully connected layers: Two fully connected layers with 256 units and ReLU activation functions.
Dropout layers: Apply dropout regularization with a rate of 0.3 to prevent overfitting.
Output layers:
1. Gender Prediction: Dense layer with sigmoid activation, outputting a single value for gender prediction.
   
2. Age Prediction: Dense layer with ReLU activation, outputting a single value for age prediction.


The model is compiled with a binary cross-entropy loss for gender prediction and mean absolute error (MAE) loss for age prediction. The optimizer used is Adam, and the metrics for evaluation include accuracy for gender prediction.


# Evaluation Metrics

The model's performance is assessed using the following evaluation metrics:

Age Prediction: R2 Score

Gender Prediction: Accuracy

