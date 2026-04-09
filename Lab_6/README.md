# Lab 6 – Feature Learning, Dimensionality Reduction, and Sequence Modeling

Course: DS3040 – Introduction to Deep Learning  
Student: Parv  

## Objective
Implement deep learning models for image and text data to extract meaningful feature representations. Apply dimensionality reduction techniques such as PCA and t-SNE for visualization, and analyze how different architectures affect learned representations.

## Tasks Performed

### 1. CNN on CIFAR-10 and Feature Visualization

#### a. Data Loading
- Loaded CIFAR-10 dataset using PyTorch
- Performed necessary preprocessing and normalization

#### b. CNN Implementation
- Built a Convolutional Neural Network with:
  - Convolution Layer (32 filters, 3×3)
  - ReLU Activation
  - Max Pooling (2×2)
  - Convolution Layer (64 filters, 3×3)
  - ReLU Activation
  - Max Pooling (2×2)
  - Fully Connected Layer (128 neurons)
  - Output Layer (10 classes)

#### c. Training
- Used Cross-Entropy Loss
- Optimized using Adam optimizer
- Recorded training loss per epoch
- Plotted training loss curve

#### d. Feature Extraction and Visualization
- Extracted 128-dimensional feature vectors from the fully connected layer
- Stored features for all test samples
- Applied Principal Component Analysis (PCA) for dimensionality reduction
- Applied t-SNE to project features into 2D space
- Visualized embeddings using scatter plots with class labels

---

### 2. Document Representation using BiLSTM

#### a. Data Loading and Preprocessing
- Loaded subset of 20 Newsgroups dataset
- Cleaned and preprocessed text data

#### b. Text Representation
- Tokenized text into sequences
- Applied padding for uniform input size

#### c. Model Implementation
- Built a Bidirectional LSTM (BiLSTM) model
- Trained the model on text data

#### d. Feature Extraction
- Extracted 256-dimensional document representations from BiLSTM layer

#### e. Dimensionality Reduction and Visualization
- Standardized feature representations
- Applied PCA (256 → 50 dimensions)
- Applied t-SNE (50 → 2 dimensions)
- Visualized document embeddings using 2D scatter plots
- Analyzed clustering of documents by topic

---

### 3. Model Improvements and Comparison

#### a. CNN Replacement with ResNet-18
- Replaced custom CNN with pretrained ResNet-18
- Extracted feature representations
- Compared quality of learned features with baseline CNN

#### b. Multi-layer LSTM
- Modified BiLSTM to a multi-layer LSTM architecture
- Trained and extracted document representations
- Compared clustering and representation quality

---

## Key Concepts
- Convolutional Neural Networks (CNNs)
- Feature Extraction and Representation Learning
- Principal Component Analysis (PCA)
- t-Distributed Stochastic Neighbor Embedding (t-SNE)
- Bidirectional LSTM (BiLSTM)
- Document Embeddings
- Transfer Learning (ResNet-18)
- Dimensionality Reduction and Visualization

---

## Conclusion
This lab focused on learning meaningful feature representations from both image and text data. It demonstrated how dimensionality reduction techniques like PCA and t-SNE help visualize high-dimensional embeddings. The results showed that deeper architectures such as ResNet-18 and advanced sequence models like BiLSTM and multi-layer LSTM produce more structured and separable feature representations. :contentReference[oaicite:0]{index=0}