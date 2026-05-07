# CNN Image Classification Project

## Overview

This project implements a **Convolutional Neural Network (CNN)** using **TensorFlow** and **Keras** for image classification. The model is trained on a dataset containing two classes (Cats and Dogs) and predicts whether an input image belongs to a cat or dog category.

The notebook demonstrates:

* Building a CNN architecture
* Image preprocessing and augmentation
* Model training
* Model evaluation
* Predicting custom images

---

# Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* Jupyter Notebook

---

# Project Structure

```bash
├── CNN.ipynb              # Main Jupyter notebook
├── training_set/          # Training images
├── test_set/              # Testing images
└── README.md              # Project documentation
```

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

Input image size:

```python
(64, 64, 3)
```

---

# Installation

Clone the repository:

```bash
git clone <your-github-repo-link>
cd <repository-name>
```

Install dependencies:

```bash
pip install tensorflow keras numpy matplotlib
```

---

# How to Run

1. Open the notebook:

```bash
jupyter notebook
```

2. Run all cells sequentially.

3. Train the model using the training dataset.

4. Test predictions on new images.

---

# Sample Code

```python
cnn = Sequential()

cnn.add(Conv2D(32,(3,3),input_shape = (64,64,3),activation = "relu"))
cnn.add(MaxPooling2D(pool_size=(2,2)))

cnn.add(Flatten())

cnn.add(Dense(64,activation = "relu"))
cnn.add(Dense(1,activation = "sigmoid"))
```

---

# Model Training

The model is trained using:

```python
cnn.fit()
```

Training and testing datasets are loaded using:

```python
flow_from_directory()
```

---

# Prediction

The trained CNN predicts whether the uploaded image is:

* Cat
* Dog

---

# Future Improvements

* Add more image classes
* Improve accuracy using deeper CNN architectures
* Use Transfer Learning (VGG16, ResNet50)
* Deploy model using Flask or Streamlit

---

# Author

Priya Singh

---
