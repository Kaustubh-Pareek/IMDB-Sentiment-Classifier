# 🎬 IMDB Sentiment Analysis with Recurrent Neural Networks (RNN)

This repository provides a complete solution to perform Sentiment Analysis on movie reviews from the IMDB dataset using a Simple Recurrent Neural Network (RNN).

The project includes:
* 📦 **Model building and training** using TensorFlow/Keras
* 🧠 **Preprocessing and padding** of input text
* 🌐 An interactive **Streamlit web app** for live sentiment prediction
* 📊 **Binary classification** (Positive / Negative Sentiment)

---

## 📁 Project Folder Structure
```bash
📦imdb-rnn-sentiment/
├── simple_rnn.ipynb       # Training notebook
├── predictions.ipynb      # Testing + Prediction notebook
├── app.py                 # Streamlit app for live prediction
├── simplernn.h5           # Trained RNN model
├── requirements.txt       # Python dependencies
├── README.md              # Project documentation
```

## 🧠 Model Overview

* **Dataset**: IMDB Movie Reviews (Keras built-in)
* **Architecture**:
    * Embedding Layer (128 dimensions)
    * SimpleRNN Layer (128 units, ReLU)
    * Dense Output Layer (Sigmoid activation)
* **Task**: Binary Sentiment Classification
* **Training Data**: 25,000 samples
* **Test Data**: 25,000 samples

---

## 🌐 Web App – Sentiment Classifier

The Streamlit app allows users to:
* Enter their own movie review
* Instantly classify it as Positive or Negative
* View the prediction confidence score

---

## 💾 Setup Instructions

### Clone the Repository
```bash
git clone https://github.com/Kaustubh-Pareek/IMDB-Sentiment-Classifier
cd imdb-rnn-sentiment
```

### Set up a Virtual Environment
```bash
# Create virtual env
python -m venv venv

# Activate on Unix or Mac
source venv/bin/activate

# Activate on Windows
venv\Scripts\activate
```

## Install Dependencies
```bash
pip install -r requirements.txt
```

### Run the Streamlit App
```bash
streamlit run app.py
```

## 📚 Dataset

The IMDB dataset used here is a preprocessed binary sentiment dataset built into keras.datasets.imdb.

- Contains 50,000 movie reviews (25k train + 25k test)
- Encoded as sequences of word indices
- Each review is labeled as 0 (negative) or 1 (positive)

## ✨ Key Features

- Simple and interpretable RNN architecture
- Clean and modular implementation
- Interactive UI with real-time predictions
- Easily extendable to LSTM/GRU models

## 🌐 Live Demo

You're welcome to explore the app by visiting the link provided below.
👉 [Try Yourself](https://imdb-sentiment-classifier-kaowhvyzkasbhy2vuhlcmp.streamlit.app/)