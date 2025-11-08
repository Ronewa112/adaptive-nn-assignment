# Adaptive Computation and Machine Learning: Assignment 1

This repository contains the solution for **Assignment 1** for the COMS 4030A course on Adaptive Computation and Machine Learning. The assignment required implementing a simple, three-layer feedforward neural network from scratch using only the `numpy` library.

## Project Overview

The core task was to implement the fundamental mechanics of a neural network:

1.  **Network Architecture:** A three-layer network (input, hidden, output) with a defined number of nodes.
2.  **Activation Function:** The **sigmoid function** for both the hidden and output layers.
3.  **Initialization:** All weights and biases are initialized to **1.0**.
4.  **Learning Rate:** A fixed learning rate of **0.1** is used.
5.  **Core Operations:** Implementation of **feedforward**, **sum-of-squares loss** calculation, and **backpropagation** for weight/bias updates.

## ⚙️ Network Specifications

| Layer | Number of Nodes | Activation Function |
| :--- | :--- | :--- |
| **Input** | 5 | None (Input) |
| **Hidden** | 10 | Sigmoid |
| **Output** | 3 | Sigmoid |

## 🚀 Execution and Output

The provided Python script (`adaptive_assignment_1.py`) performs the following steps when run:

1.  Reads **eight floating-point numbers** from standard input.
    * The **first five** are the network's input features (X).
    * The **last three** are the target values (T).
2.  Performs the **initial feedforward** and computes the **initial sum-of-squares loss**.
3.  Executes **one iteration of backpropagation** to update all weights and biases.
4.  Performs a **final feedforward** using the same input and computes the **final loss** with the updated network.
5.  Outputs two values to standard output, each rounded to 4 decimal places:
    * The **loss before training**.
    * The **loss after one backpropagation step**.

### Example Input/Output

| Step | Input | Expected Output |
| :--- | :--- | :--- |
| **Example 1** | `3, 1, -2, -1, -4, 0, 1, 0` | `0.8142` (Initial Loss) \
  `0.8043` (Final Loss) |
| **Example 2** | `-3, 1, -5, 0, -1, 0.3, 0.2, 0.7` | `0.2362` (Initial Loss) \
  `0.2344` (Final Loss) |

## 📁 `adaptive_assignment_1.py`

This file contains the full Python implementation. Key functions include:

* `sigmoid(x)` and `sigmoid_derivative(x)`
* `feedforward(X)`
* `compute_loss(y, t)`
* `backpropagation(X, hidden_output, output, target)`

The main script section handles initialization, reading input, performing the forward/backward pass, and printing the required losses.