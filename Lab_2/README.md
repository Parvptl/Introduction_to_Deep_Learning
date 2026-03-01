# Lab 2 – Feedforward Neural Networks  
**Course:** DS3040 – Introduction to Deep Learning  
**Student:** Parv Patel  

## Overview
This lab implements Feedforward Neural Networks (FNNs) for:
1. Regression
2. Binary Classification
3. Multiclass Classification with Hyperparameter Tuning

The focus is on model design, training, validation, regularization, and evaluation.

---

## Question 1 – Regression (Graduate Admission Dataset)

- Architecture: 7 → 7 → 1 (ReLU activations)
- Loss: MSELoss
- Optimizer: Adam
- Evaluation: Test Loss & R² Score
- Training and validation loss curves plotted

---

## Question 2 – Binary Classification (Heart Disease Dataset)

- Architecture: 8 → 4 → 1 (Sigmoid)
- Compared:
  - Model without Dropout
  - Model with 50% & 30% Dropout
- Loss: BCELoss
- Evaluation: Accuracy, Loss Curves
- Dropout effect analyzed for generalization

---

## Question 3 – Multiclass Classification (Modified Fashion MNIST)

- Flexible FNN architecture
- Hyperparameters tuned:
  - Hidden layers
  - Learning rate
  - Dropout rate
  - Batch size
  - Epochs
  - Optimizer
- Loss: CrossEntropyLoss
- Best configuration selected using validation accuracy
- Final test accuracy reported

---

## Key Concepts Covered

- Train / Validation / Test split
- Hold-out validation for hyperparameter tuning
- Dropout regularization
- Mini-batch training with DataLoader
- Proper use of `train()`, `eval()`, and `no_grad()`
- Logits handling with CrossEntropyLoss

---

## Conclusion

This lab demonstrates practical implementation of neural networks for regression and classification, along with structured hyperparameter tuning and evaluation using validation-based model selection.