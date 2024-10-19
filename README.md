# Image-Processing-Model

 Image Classification using Transfer Learning & Neural Networks

This project implements image classification on the MNIST dataset using neural networks and hyperparameter tuning. Several models are trained using different activation functions, optimizers, and dropout techniques. Additionally, transfer learning with pretrained models (VGG-16 and VGG-19) is applied for image classification tasks in the provided datasets.

 Project Overview

 Models Implemented
1. Sequential Dense Layers Model: Four different sequential models were implemented using various activation functions (sigmoid, tanh, relu, selu) and optimizers (SGD, Adam, AdamW, Nadam) with dropout layers for regularization.
2. Hyperparameter Tuning with Keras Tuner*: Used Keras Tuner for hyperparameter optimization (number of units, learning rate, and batch size) to enhance model accuracy.
3. Transfer Learning (VGG-16 & VGG-19): 
    - Applied pretrained VGG-16 and VGG-19 models, extracted deep features, and classified using Random Forest for the two-class skin cancer and three-class orange dataset classification tasks.

 Datasets
- MNIST Dataset: A standard dataset of handwritten digits used for image classification.
- Skin_Cancer RGB Dataset*: For binary classification of skin cancer.
- Orange Dataset*: For three-class classification of oranges.

 Code Structure

- Main Model Training: Several models were created using the Sequential API from Keras. The models were trained with different configurations, activation functions, optimizers, and dropout layers to prevent overfitting.
- Hyperparameter Tuning: Random search was applied to find the optimal number of units, learning rates, and batch sizes.
- Evaluation: Each model was evaluated based on test accuracy after training on the MNIST dataset.

 Installation

1. Install the required dependencies:

   pip install keras
   pip install tensorflow
   pip install keras-tuner
