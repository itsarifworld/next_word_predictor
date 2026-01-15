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

---

### 2️⃣ Tokenization (Word → Number Mapping)

Using `Tokenizer`, each unique word is assigned a unique integer.

This step is crucial because **neural networks cannot process text directly** — they work with numbers.

---

### 3️⃣ Sequence Generation

To train the model, the text is converted into **progressive sequences**:

This teaches the model:
> “Given previous words, predict the next word.”

---

### 4️⃣ Padding for Equal Length

Since sentences vary in length, all sequences are **padded to the same size** using pre-padding.

This ensures:
- Uniform input shape
- Proper batch processing during training

---

### 5️⃣ Model Architecture

The neural network architecture consists of:

- **Embedding Layer**
  - Converts word indices into dense vector representations
- **LSTM Layer**
  - Learns long-term dependencies between words
- **Dense Output Layer**
  - Uses softmax to predict the probability of each word in the vocabulary

This architecture allows the model to **understand word order and context**, not just frequency.

---

### 6️⃣ Training the Model

The model is trained using:
- **Categorical Crossentropy loss**
- **Adam optimizer**

During training, the model learns:
- Grammar patterns
- Word relationships
- Sentence structure

---

### 7️⃣ Next Word Prediction Pipeline

When a user inputs a sentence:

1. The text is tokenized
2. It is padded to match training input size
3. The trained model predicts the most probable next word
4. The predicted word index is mapped back to the actual word

