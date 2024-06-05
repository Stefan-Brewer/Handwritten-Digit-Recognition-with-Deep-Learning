# Handwritten Digit Recognition with Deep Learning

This project aims to build a deep learning model using Keras to recognize handwritten digits from the MNIST dataset. The MNIST dataset is a widely-used benchmark dataset in machine learning, consisting of 28x28 pixel grayscale images of handwritten digits (0 through 9).

## Overview

The project covers the following steps:

1. **Loading the Dataset**: The MNIST dataset is loaded directly from the Keras library.

2. **Data Preprocessing**: The images are normalized to be between 0 and 1 to improve the training process. They are also flattened from 2D arrays to 1D vectors for input into the neural network.

3. **Neural Network Architecture**: A simple feedforward neural network architecture is defined using Keras. It consists of an input layer, one or more hidden layers with ReLU activation, and an output layer with softmax activation.

4. **Training the Model**: The model is trained on the training dataset, with a portion of the data used for validation to monitor performance during training.

5. **Evaluation**: The trained model is evaluated on a separate test dataset to measure its accuracy in recognizing handwritten digits.

6. **Data Augmentation**: I tried a few versions of the image set, including inverting the pixel values, and scaling them. However, I ran into an issue where all predictions were just 1s.

## Current Status

This project is a work in progress. The initial steps, including data loading, preprocessing, and defining the neural network architecture, have been completed. The model has been trained and evaluated on the MNIST dataset, achieving a test accuracy of approximately 98%. I am currently looking into why the augmented datasets are only predicting 1s, despite it going fine in a test I did on another file.

## Next Steps

- Further optimize the neural network architecture and hyperparameters for better performance.
- Implement strategies to mitigate overfitting, such as regularization and dropout.
- Experiment with different optimization algorithms and learning rates.

## Dependencies

- Python 3.x
- TensorFlow
- Keras
- NumPy
- Matplotlib
