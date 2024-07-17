**Name** : RAHUL RAJ MEKALA

**Company** : CODTECH IT SOLUTIONS

**ID** : CT4ML2534

**Domain** : MACHINE LEARNING

**Duration** : 20th June 2024 to 20 July 2024

**Mentor** : NEELA SANTHOSH KUMAR

## **Project Overview: ANALYSIS ON MOVIE REVIEWS**

## Objective:

The goal of this project is to perform sentiment analysis on IMDb movie reviews using deep learning techniques with TensorFlow. The sentiment of each review is categorized as either positive or negative based on the textual content.

## Installation

To run the Jupyter Notebook and reproduce the sentiment analysis, make sure you have the following dependencies installed:

- Python 3
- TensorFlow
- TensorFlow Hub
- TensorFlow Datasets
- NumPy
- Matplotlib

## Steps Involved:
**Setup and Data Loading**:
  TensorFlow and TensorFlow Hub are imported for deep learning functionalities.
The IMDb dataset is downloaded using TensorFlow Datasets (tfds.load()). It consists of 50,000 movie reviews split into training and test sets.

**Data Exploration:** 
The dataset is explored to understand its format and content. Each review is associated with a label (0 for negative, 1 for positive).

**Embedding Layer Setup:**

TensorFlow Hub is used to create an embedding layer (hub.KerasLayer) that converts text inputs into embeddings using a pre-trained model (nnlm-en-dim50).

**Model Definition:**

A sequential model is built with the embedding layer followed by two dense layers:
The first dense layer with ReLU activation function.
The output layer with a single unit and sigmoid activation function for binary classification.

**Model Compilation:**

The model is compiled with the adam optimizer and binary_crossentropy loss function, suitable for binary classification tasks. Accuracy is chosen as the metric to monitor during training.

**Validation Set Creation:**

A validation set is created by setting aside 10,000 examples from the original training data to evaluate the model's performance during training.

**Model Training:** 

The model is trained for 40 epochs using mini-batches of 512 samples. Training progress is monitored using both training and validation data.

**Model Evaluation:**

After training, the model's performance is evaluated on the test set to measure its accuracy and loss.

**Visualization:**

Training and validation metrics (loss and accuracy) are plotted over epochs to visualize the model's learning progress and potential overfitting.

**Results:**

The model achieves an accuracy of approximately 87% on the test set. Further refinements or more advanced techniques could potentially improve accuracy closer to 95%.


## OUTPUT
