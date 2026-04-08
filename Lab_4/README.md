# Lab 4 – Convolutional Neural Networks and Architecture Experiments

Course: DS3040 – Introduction to Deep Learning  
Student: Parv  

## Objective
Implement and analyze Convolutional Neural Networks (CNNs) using PyTorch on the Fashion-MNIST dataset, explore architectural variations, study dropout regularization, and compare performance with a pretrained VGG19 model.

## Tasks Performed

### 1. Basic CNN Implementation
- Loaded Fashion-MNIST dataset using `torchvision.datasets.FashionMNIST`
- Used `Subset` from `torch.utils.data` for train/test split
- Built a CNN with:
  - 3 Convolutional layers
  - ReLU activation after each layer
  - Max Pooling layers
  - 2 Fully Connected layers
- Trained the model and evaluated on test data
- Plotted accuracy curve over epochs

### 2. Architecture Variations

#### a. Changing Depth
- Implemented CNNs with:
  - 2 Convolutional layers
  - 5 Convolutional layers
- Trained and evaluated each model
- Compared test accuracies

#### b. Dropout Experiments
- Added dropout in two configurations:
  - After each convolutional layer
  - After each fully connected layer
- Trained both models and recorded performance

#### c. Observations
- Analyzed the effect of:
  - Model depth
  - Dropout placement
  - Overfitting and generalization

### 3. Comparison with VGG19

#### a. VGG19 Implementation
- Loaded VGG19 model from `torchvision.models`
- Modified final layer to output 10 classes
- Trained and evaluated on Fashion-MNIST

#### b. Performance Comparison
- Compared VGG19 with custom CNN models based on:
  - Accuracy
  - Model complexity
  - Generalization ability

## Key Concepts
- Convolutional Neural Networks (CNNs)
- Feature Extraction and Spatial Hierarchies
- ReLU Activation and Max Pooling
- Dropout Regularization
- Model Architecture Design
- Transfer Learning (VGG19)

## Conclusion
This lab demonstrated how CNN architecture choices and regularization techniques influence model performance. It also showed that deeper pretrained models like VGG19 can achieve better generalization, while introducing higher computational cost.