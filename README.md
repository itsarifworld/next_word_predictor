# Next Word Prediction using LSTM

## 📌 Project Overview

This project implements a **Next Word Prediction system** using **Deep Learning (LSTM)**.  
Given a sequence of words as input, the model predicts the **most likely next word**, based on patterns learned from the training text.

The goal of this project is not just to build a working model, but to **understand and demonstrate how language modeling works internally**, from text preprocessing to sequence learning with neural networks.

---

## 🧠 What I Have Done

- Collected and prepared a **text corpus** (FAQ-style content)
- Converted raw text into **numerical representations** using tokenization
- Generated **input–output sequences** for supervised learning
- Built a **Sequential LSTM-based neural network**
- Trained the model to learn **word sequence patterns**
- Implemented a **prediction pipeline** to generate the next word
- Analyzed model limitations and proposed improvements

---

## 🛠️ Tech Stack & Libraries Used

- **Python**
- **TensorFlow / Keras**
- **NumPy**
- **Tokenizer & Padding utilities**

---

## 🧩 How the Project Works (Step-by-Step)

### 1️⃣ Text Preparation

The model starts with a block of text containing multiple sentences.  
This text acts as the **training corpus** from which the model learns language structure.

Example:
