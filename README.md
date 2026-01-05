# Emotion Detection using BiLSTM with Attention

This project implements an emotion detection system using Bidirectional LSTM with an attention mechanism trained on the GoEmotions dataset.  
The model predicts the dominant emotion expressed in a given sentence and provides confidence scores.  
An interactive Gradio interface is included for real-time testing.

# Project Highlights

- Emotion classification with 27 fine-grained emotion classes
- Baseline BiLSTM model (without attention)
- Improved BiLSTM + Attention model
- Fair comparison using identical preprocessing
- Interactive Gradio web application
- Resume and interview-ready NLP project

# Dataset

GoEmotions Dataset (Google)

- 58k+ English sentences
- 27 emotion categories
- Originally multi-label
- Converted to single-label classification for stable training

Sample emotions:
joy, sadness, anger, fear, love, surprise, gratitude, remorse, optimism
# Why Attention?

- Emotion is usually expressed by specific words, not the entire sentence
- Attention allows the model to focus on emotion-bearing tokens
- Improves interpretability and classification performance

Mathematical intuition:
# Tech Stack

- Python
- TensorFlow / Keras
- HuggingFace Datasets
- NumPy
- Gradio

# Training Configuration

- Vocabulary Size: 20000
- Max Sequence Length: 50
- Embedding Dimension: 128
- BiLSTM Units: 128
- Optimizer: Adam
- Loss Function: Sparse Categorical Crossentropy
- Metric: Accuracy

# Evaluation

- Train / Validation / Test splits used
- Models evaluated:
  - BiLSTM (baseline)
  - BiLSTM + Attention
- Attention model shows better emotion sensitivity and generalization

# Gradio Deployment

An interactive Gradio web application is included.

Features:
- Text input
- Predicted dominant emotion
- Confidence score
- Top-3 emotion probabilities

Example inputs:
I feel absolutely amazing today!
I am scared and nervous about the exam.
That was the worst experience ever.
Future Improvements

Multi-label emotion classification

Attention weight visualization per word

Transformer-based models (BERT / RoBERTa)

API deployment using FastAPI or Flask

Author

Arshpreet Walia
NLP | Deep Learning | Emotion Analysis

Support

If you find this project useful, please give it a star ⭐ on GitHub.
