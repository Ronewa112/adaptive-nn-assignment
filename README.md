# COMS4030A – Adaptive Computation and Machine Learning
## Assignment 1: Three-Layer Neural Network

### 📘 Description
This project implements a simple 3-layer neural network **using only NumPy**, as required by the COMS4030A Assignment 1 specification.

**Network architecture:**
- Input layer: 5 nodes  
- Hidden layer: 10 nodes (sigmoid activation)  
- Output layer: 3 nodes (sigmoid activation)  
- All weights and biases initialized to 1  
- Learning rate: 0.1  

The program:
1. Reads 8 float values from standard input (5 inputs + 3 targets)
2. Computes feedforward output and loss
3. Performs one iteration of backpropagation
4. Recomputes the loss and prints both values rounded to 4 decimals

### 🧠 Example Input & Output

**Input:**
3
1
-2
-1
-4
0
1
0
