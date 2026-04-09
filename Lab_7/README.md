# Lab 7 – Attention Mechanisms and Transformer-Based Text Classification

Course: DS3040 – Introduction to Deep Learning  
Student: Parv  

## Objective
Implement the scaled dot-product attention mechanism from scratch and build a Transformer-based model for text classification. Analyze attention behavior and understand how Transformer architectures process sequential data.

## Tasks Performed

### 1. Scaled Dot-Product Attention

#### a. Implementation
- Implemented scaled dot-product attention using PyTorch:
  - Computed attention scores using QK^T
  - Applied scaling factor (1 / sqrt(dk))
  - Applied softmax to obtain attention weights
  - Multiplied with V to obtain context vectors
- Returned both:
  - Attention output (context vectors)
  - Attention weight matrix

#### b. Testing
- Tested the function using random tensors of shape (sequence length = 6, dk = 8)
- Verified correctness by printing output shapes

#### c. Visualization
- Used a toy sentence: "The cat sat on the mat"
- Represented tokens using random embeddings
- Applied self-attention (Q = K = V)
- Computed attention weights
- Visualized the 6×6 attention matrix using a heatmap
- Labeled axes with token names and included colorbar

---

### 2. Transformer-Based Emotion Classification

#### a. Data Loading and Preprocessing
- Loaded dataset using pandas
- Converted text to lowercase
- Tokenized using whitespace splitting
- Built vocabulary with special tokens:
  - <pad> = 0
  - <unk> = 1
- Converted text into sequences of indices
- Applied padding to fixed length (50)
- Encoded labels numerically

#### b. Transformer Model Implementation
- Built model with the following components:
  - Embedding layer (dimension = 64)
  - Positional encoding
  - Self-attention layer (using custom attention function)
  - Feedforward network (64 → 128 → 64)
  - Residual connections and layer normalization
  - Two stacked encoder layers
- Applied mean pooling across sequence dimension
- Used a linear layer for final classification

#### c. Training
- Set random seed for reproducibility
- Used DataLoader with batch size = 32 and no shuffling
- Used CrossEntropyLoss
- Optimized using Adam (learning rate = 0.001)
- Trained for 5 epochs
- Printed average training loss per epoch

#### d. Evaluation
- Evaluated model on test dataset
- Computed classification accuracy

#### e. Prediction
- Tested model on custom input:
  - "I feel very happy today"
- Output predicted emotion label

---

## Key Concepts
- Scaled Dot-Product Attention
- Self-Attention Mechanism
- Transformer Architecture
- Positional Encoding
- Residual Connections and Layer Normalization
- Feedforward Networks in Transformers
- Text Tokenization and Vocabulary Building
- Sequence Modeling without Recurrence

---

## Conclusion
This lab provided hands-on experience with attention mechanisms and Transformer architectures. It demonstrated how self-attention captures relationships between tokens and how Transformers can effectively replace recurrent models for sequence tasks. The implementation highlighted the importance of positional encoding and residual connections in maintaining sequence structure and improving model performance. :contentReference[oaicite:0]{index=0}