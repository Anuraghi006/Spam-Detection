
# NLP Spam Detection System

## Overview

This project implements a **Spam Message Detection System using Natural Language Processing (NLP) and Machine Learning**. The model analyzes text messages and classifies them as **Spam** or **Ham (Not Spam)**.

Spam messages are commonly found in SMS and email communication and often contain advertisements, scams, or malicious links. Manually filtering such messages is inefficient, so this system automates the process using machine learning techniques.

The model is trained on a labeled SMS dataset and learns patterns that typically appear in spam messages. Once trained, the system can predict whether a new incoming message is spam or legitimate.

---

## Features

* Automatic spam detection using machine learning
* Text preprocessing using NLP techniques
* Feature extraction using **Bag of Words (CountVectorizer)**
* Model training using **Scikit-learn**
* Real-time message prediction
* Model saving using **Pickle** for future use
* High accuracy spam classification

---

## Technologies Used

* Python
* Pandas
* NLTK
* Scikit-learn
* CountVectorizer (Bag of Words)
* Pickle
* Jupyter Notebook

---

## Project Workflow

### 1. Import Libraries

Necessary Python libraries such as Pandas, NLTK, and Scikit-learn are imported for data processing and model building.

### 2. Data Loading

The dataset containing labeled SMS messages is loaded and prepared for analysis.

Example dataset format:

| Label | Message                               |
| ----- | ------------------------------------- |
| ham   | Hello, how are you?                   |
| spam  | Congratulations! You have won a prize |

---

### 3. Text Preprocessing

Before training the model, the text data is cleaned and processed using NLP techniques:

* Converting text to lowercase
* Removing punctuation
* Removing stopwords
* Tokenization

This step helps the model understand the important words in the messages.

---

### 4. Text Vectorization

Machine learning models require numerical input. Therefore, text messages are converted into numerical vectors using:

**CountVectorizer (Bag of Words)**

This technique represents each message based on the frequency of words appearing in the text.

---

### 5. Train-Test Split

The dataset is divided into:

* **Training Data** – used to train the model
* **Testing Data** – used to evaluate model performance

---

### 6. Model Training

A machine learning classifier is trained on the processed dataset to identify patterns that distinguish spam messages from normal messages.

---

### 7. Prediction System

The trained model can classify new messages.

Example:

predict_spam("Congratulations! You won a free ticket")

Output:
Spam

---

### 8. Model Saving

The trained model and vectorizer are saved using **Pickle** so that they can be reused later without retraining.

---

## Model Performance

The model achieves approximately **97% accuracy** in detecting spam messages on the test dataset.

Common words that frequently appear in spam messages include:

* free
* win
* claim
* prize

---

## Applications

This spam detection system can be used in:

* Email spam filters
* SMS filtering systems
* Chat applications
* Messaging platforms
* Cybersecurity tools

---

## Future Improvements

Possible enhancements to this project include:

* Deploying the system as a **web application using Flask or Streamlit**
* Using **Deep Learning models such as LSTM or BERT**
* Training on **larger datasets** to improve accuracy
* Integrating with **real-time messaging systems**

---

