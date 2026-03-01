# Lab 3 – Feedforward Neural Network (From Scratch & PyTorch)

**Course:** DS3040 – Introduction to Deep Learning  
**Student:** Parv  

## Objective
Implement a Feedforward Neural Network (FNN) from scratch using NumPy, perform hyperparameter tuning, re-implement the same architecture using PyTorch, and generalize the model for multiple hidden layers.

---

## Tasks Performed

### 1. From-Scratch Implementation
- Forward Propagation
- Binary Cross Entropy Loss
- Backpropagation (Chain Rule)
- Batch Gradient Descent
- One hidden layer (ReLU) + Output layer (Sigmoid)

### 2. Data Handling
- Feature standardization
- Manual 70-15-15 train/validation/test split
- Reproducible shuffling using fixed random seed

### 3. Hyperparameter Tuning
Grid search over:
- Epochs: 10, 15, 25, 100  
- Hidden Units: 4, 8, 16  
- Learning Rate: 0.2, 0.1, 0.01  

Best model selected based on validation performance and evaluated on test set.

### 4. PyTorch Implementation
- Implemented same architecture using `nn.Module`
- Used `ReLU`, `Sigmoid`, `BCELoss`, and `SGD`
- Compared performance with from-scratch model

### 5. Generalized ANN
- Supports arbitrary number of layers
- Dynamic forward and backward propagation
- Object-oriented implementation

---

## Key Concepts
- Feedforward Neural Networks  
- ReLU & Sigmoid Activations  
- Binary Cross Entropy  
- Backpropagation  
- Gradient Descent  
- Hyperparameter Tuning  

---

## Conclusion
This lab provided a complete understanding of neural network internals by implementing forward and backward propagation manually and comparing results with PyTorch’s automatic differentiation framework.