# 🎵 Music Generation using RNN (LSTM)
## 🚀 Overview

This project implements a **Recurrent Neural Network (RNN) using Long Short-Term Memory (LSTM)** to generate music in **ABC notation**.
The model is trained on a dataset of Irish folk songs and learns to generate new music by predicting the **next character in a sequence**.

---
## 🧠 Key Concepts

* Recurrent Neural Networks (RNN)
* Long Short-Term Memory (LSTM)
* Sequence Modeling
* Character-level Text Generation
* Embedding Layers
* Cross Entropy Loss
* Backpropagation
* Generative AI

---
## ⚙️ Model Architecture

The model consists of the following layers:

```
Embedding Layer (vocab_size → embedding_dim)
        ↓
LSTM Layer (embedding_dim → hidden_size)
        ↓
Fully Connected Layer (hidden_size → vocab_size)
```

---
## 🔄 Workflow

```
Music Dataset (ABC notation)
        ↓
Convert characters → integers (vectorization)
        ↓
Embedding Layer
        ↓
LSTM Network
        ↓
Linear Layer
        ↓
Predict next character
        ↓
Train using teacher forcing
        ↓
Generate new music
```

---

## 📊 Training Details

* **Batch Size:** 8
* **Sequence Length:** 100
* **Embedding Dimension:** 256
* **Hidden Size:** 1024
* **Learning Rate:** 0.005
* **Training Iterations:** 3000

### 📉 Training Results

* Initial Loss: ~4.46
* Final Loss: ~0.54

The significant decrease in loss indicates that the model successfully learned patterns in the dataset.

---

## 🎼 Sample Generated Output

```
X:1
T:Generated Tune
M:4/4
K:D
A2 AB d2 AF | G2 FE D4 |
FA AB d2 AF | G2 FE D4 |
```

---

## 🛠️ Technologies Used

* Python
* PyTorch
* NumPy
* Google Colab
* Comet ML (for experiment tracking)

---

## 📌 Key Learnings

* Built and trained an LSTM-based sequence model
* Understood how neural networks process sequential data
* Learned how to convert text into numerical representations
* Implemented training loops using PyTorch
* Explored generative AI concepts through music generation

---
## 💡 Applications

This project demonstrates the core idea behind modern generative models used in:

* Text generation (e.g., ChatGPT)
* Code generation
* Music generation
* Speech modeling

---
## ▶️ How to Run

1. Clone the repository:

```
git clone https://github.com/your-username/AI-Music-Generation-RNN.git
```

2. Open the notebook:

```
music-generation-rnn.ipynb
```

3. Run all cells (preferably with GPU enabled).

---

## 📖 Conclusion

This project showcases how **LSTM-based neural networks can learn patterns in sequential data** and generate new content.
It highlights the power of deep learning in creative domains such as music generation and forms a foundation for understanding modern generative AI systems.

---
## ⭐ Acknowledgements

* MIT Introduction to Deep Learning (6.S191)
* PyTorch Documentation

---
