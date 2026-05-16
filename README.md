# CNN Image Classification Project (Cat Vs Dog)

## Overview

This project implements a **Convolutional Neural Network (CNN)** using **TensorFlow** and **Keras** for image classification. The model is trained on a dataset containing two classes (Cats and Dogs) and predicts whether an input image belongs to a cat or dog category.

Project Description
A binary image classification model that predicts whether an input image is a cat or a dog using a CNN built with TensorFlow and Keras.

# Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Jupyter Notebook

---

# CNN Architecture

The model consists of:

1. Convolution Layers
2. Max Pooling Layers
3. Flatten Layer
4. Fully Connected Dense Layers
5. Output Layer with Sigmoid Activation

The CNN uses:

* ReLU activation for hidden layers
* Sigmoid activation for binary classification
* Adam optimizer
* Binary Crossentropy loss function

---

# Data Preprocessing

Image preprocessing is performed using `ImageDataGenerator`.

Techniques used:

* Rescaling
* Shear transformation
* Zoom augmentation
* Horizontal flipping

# Prediction

The trained CNN predicts whether the uploaded image is:

* Cat
* Dog

---



# Author

Priya Singh

---
