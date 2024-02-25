# 60k Image Classification
## Overview
This project focuses on image classification using Artificial Neural Networks (ANNs). ANNs are a type of neural network where neurons in one layer are connected to all neurons in the next layer.

 ## CIFAR-10 Dataset
The CIFAR-10 dataset comprises 60,000 32x32 color images distributed across 10 classes, with 6,000 images per class. Specifically, there are 50,000 training images and 10,000 test images. The dataset is divided into five training batches and one test batch, each containing 10,000 images. The test batch includes 1,000 randomly-selected images from each class, while the training batches contain the remaining images in random order. However, some training batches may contain more images from one class than another, but overall, each class is represented by exactly 5,000 images.

 ## Data Preprocessing
The dataset is preprocessed as follows:

Load the CIFAR-10 dataset using TensorFlow.
Scale the pixel values of the images to the range [0, 1].
Perform one-hot encoding on the categorical labels to convert them into numerical values.
## Model Architecture
The Artificial Neural Network model consists of the following layers:

Flatten layer: Reshapes the input images into a single-dimensional array.
Dense layer: Fully connected layer with 3000 neurons and ReLU activation function.
Dense layer: Fully connected layer with 1500 neurons and ReLU activation function.
Dense layer: Output layer with 10 neurons (corresponding to the 10 classes) and sigmoid activation function.
## Training
The model is compiled using the Adam optimizer and categorical cross-entropy loss function. The accuracy metric is used to monitor the model's performance during training. The model is trained for 10 epochs using the training data.

## Usage
To use the model for inference, load the trained model and preprocess the input images by scaling their pixel values. Then, use the predict method to obtain predictions for the input images.



