# Implemented Backpropagation from Scratch using Banknote Authentication Dataset

This file contains a Jupyter Notebook:  
📘 **`Backpropagation_from_Scratch_Using_Banknote_Authentication_Dataset.ipynb`**  
which implements a neural network from scratch using **NumPy** and the **backpropagation algorithm** for binary classification on the Banknote Authentication Dataset.

---

## 📌 Overview

This project demonstrates the fundamental concepts of neural networks and backpropagation. Key steps covered include:

- 🔹 Data loading and preprocessing (scaling and train-test splitting)  
- 🔹 Building a multi-layer neural network from scratch using NumPy  
- 🔹 Sigmoid activation function implementation  
- 🔹 Forward and backward propagation  
- 🔹 Training the network and evaluating performance (loss and accuracy)

---

## 📊 Dataset

The **Banknote Authentication Dataset** is sourced from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/228/banknote+authentication).  
It contains **1372 instances** and **4 features**:

- **Features (X):**
  - Variance of Wavelet Transformed image (continuous)  
  - Skewness of Wavelet Transformed image (continuous)  
  - Curtosis of Wavelet Transformed image (continuous)  
  - Entropy of image (continuous)

- **Target (y):**
  - Class label (integer):  
    `0` = Genuine  
    `1` = Forged

---

## 🧠 Neural Network Architecture & Parameters

| Component            | Value | Description                         |
|----------------------|-------|-------------------------------------|
| Input Layer Size     | 4     | Number of input features            |
| Hidden Layer 1       | 8     | Neurons in 1st hidden layer         |
| Hidden Layer 2       | 6     | Neurons in 2nd hidden layer         |
| Hidden Layer 3       | 4     | Neurons in 3rd hidden layer         |
| Output Layer Size    | 1     | Binary output (genuine/forged)      |
| Activation Function  | Sigmoid | Non-linearity in all layers       |
| Learning Rate (lr)   | 0.001 | Step size for gradient descent      |
| Epochs               | 1000  | Number of training iterations       |
| Test Size            | 0.2   | 20% data reserved for testing       |
| Random State         | 42    | Ensures reproducibility             |

Weights are initialized using `np.random.randn()` and biases with `np.zeros()`.

---
# Results

**Test Loss**: 0.0109
**Test Accuracy**: 0.9818


![Plot](https://github.com/YasirISkhan/CodeThePaper/blob/main/Backpropagation/img/Loss%20over%20epochs.png)



