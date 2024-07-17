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
![Screenshot 2024-07-18 011831](https://github.com/user-attachments/assets/f70796c6-3eed-48a8-bacf-88f66c8ed011)
![Screenshot 2024-07-18 011817](https://github.com/user-attachments/assets/bb0459ab-06c3-47f5-becd-832b55f58f34)
![Screenshot 2024-07-18 011757](https://github.com/user-attachments/assets/c222df47-2d36-4712-b3af-a5c84db6841a)
![Screenshot 2024-07-18 011858](https://github.com/user-attachments/assets/c5f0b1fa-57f0-4472-ad5c-3d7f74a5a56a)
![Screenshot 2024-07-18 011932](https://github.com/user-attachments/assets/7f85c33a-9d9a-4db5-b121-990e8186f218)
![Screenshot 2024-07-18 011917](https://github.com/user-attachments/assets/5bddca47-d5af-4e3c-9a0c-9f1a5ec2c33f)


