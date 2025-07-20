# 💬 Chat Toxicity Detection with Custom Transformer

This project implements a custom **Transformer-based deep learning model** from scratch to detect and classify **toxic chat messages**. The model is trained on labeled data to identify various levels of toxicity in online conversations.

---

## 🚀 Overview

- **Goal**: Build a lightweight Transformer model to classify chat messages as toxic or non-toxic.
- **Approach**: No pre-trained models — the Transformer architecture is implemented from scratch using PyTorch.
- **Application**: Real-time moderation systems for social platforms, games, or forums.

---

## 🧾 Dataset

- **Structure**: Two columns — `text` and `label`
- **Classes**:
  - `0` — Non-toxic
  - `1` — Toxic

> Note: Dataset is preprocessed before training and split into training and validation sets (80/20).

---

## 🛠️ Model Architecture

- **Tokenizer**: Basic whitespace tokenizer with a custom vocabulary
- **Transformer Encoder**:
  - Multi-Head Self-Attention
  - Positional Encoding
  - Layer Normalization
  - Feed Forward Layers
- **Classifier Head**:
  - Linear layer + Softmax/Sigmoid activation

> The model is built from scratch using native PyTorch modules — no `transformers` library used.

---

## 📈 Training Details

- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Epochs**: 10
- **Batch Size**: 16
- **Metrics**: Accuracy, F1 Score

> Model is trained with early stopping and validation performance monitoring.

---

## 🧪 Evaluation

- **Accuracy**: >90%
- **Generalization**: The model performs well on unseen data and is robust to variation in message styles and lengths.

---

## 📊 Features

- Simple and clean implementation of Transformer components
- Easily extendable to multi-label classification (e.g., threat, obscene, insult)
- Modular design for reuse in other NLP tasks

---

## 📦 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/chat-toxicity-transformer.git
   cd chat-toxicity-transformer
