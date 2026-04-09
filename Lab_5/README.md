# Lab 5 – Recurrent Neural Networks for Language Modeling and Classification

Course: DS3040 – Introduction to Deep Learning  
Student: Parv  

## Objective
Develop and analyze Recurrent Neural Network (RNN) based models for sequence tasks, including next-word prediction and sentence classification. Compare Simple RNN and LSTM architectures and study the impact of hyperparameter tuning on performance.

## Tasks Performed

### 1. Next-Word Prediction using RNN and LSTM

#### a. Data Loading and Preprocessing
- Loaded Shakespeare Hamlet text from NLTK Gutenberg corpus
- Performed text cleaning and preprocessing

#### b. Sequence Preparation
- Tokenized the text into words
- Created sequential input-output pairs
- Applied padding to ensure uniform sequence length

#### c. Model Implementation
- Built language models using:
  - Simple RNN
  - LSTM
- Trained both models on the prepared sequences

#### d. Performance Comparison
- Evaluated both models on next-word prediction
- Compared their effectiveness in capturing context and sequence dependencies

---

### 2. Sentence Classification using RNN and LSTM

#### a. Data Loading and Preprocessing
- Loaded IMDB Dataset
- Cleaned and prepared text data

#### b. Text Representation
- Converted text into numerical sequences using tokenization
- Applied padding to maintain consistent input size

#### c. Model Implementation
- Built and trained a Simple RNN classification model

#### d. LSTM Replacement
- Replaced Simple RNN with LSTM architecture
- Trained and evaluated the model

#### e. Performance Comparison
- Compared RNN and LSTM models based on classification accuracy
- Analyzed which architecture performs better and why

---

### 3. Hyperparameter Tuning

#### a. Model Modification
- Modified LSTM model by changing:
  - Embedding dimension
  - Hidden layer size

#### b. Training
- Trained modified models on the same dataset

#### c. Performance Evaluation
- Compared training accuracy of original and modified models

#### d. Analysis
- Identified the best-performing hyperparameter configuration
- Provided justification based on observed results

---

## Key Concepts
- Recurrent Neural Networks (RNNs)
- Long Short-Term Memory (LSTM)
- Sequence Modeling
- Tokenization and Padding
- Language Modeling
- Text Classification
- Embedding Layers
- Hyperparameter Tuning

---

## Conclusion
This lab explored the application of recurrent neural networks in natural language processing tasks. It demonstrated that while Simple RNNs can model short-term dependencies, LSTMs are more effective in capturing long-term context, leading to improved performance in both language modeling and classification tasks. Hyperparameter tuning further highlighted the importance of selecting appropriate model configurations for optimal results. :contentReference[oaicite:0]{index=0}