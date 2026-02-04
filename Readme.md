# 🤖 Mini NLP Chatbot (Intent Classification)

A simple chatbot built using **Natural Language Processing (NLP)** and **Machine Learning** to understand user intent and respond accordingly.

This project demonstrates how traditional (pre-LLM) chatbots work under the hood using **TF-IDF vectorization** and **Logistic Regression**.

---

## 📌 Project Overview

The chatbot classifies user input into predefined **intents** such as:
- Greeting
- Goodbye
- Asking the bot’s name
- Asking for help

Based on the detected intent, it returns an appropriate response.

This is a **machine-learning-based chatbot**, not a rule-based one.

---

## 🧠 How It Works (High Level)

1. User enters a sentence
2. Text is converted into numerical features using **TF-IDF**
3. A **Logistic Regression** model predicts the intent
4. The chatbot selects a response mapped to that intent

---

## 🔍 Example Interaction

```

You: hi
Bot: Hey! How can I help you?

You: what can you do
Bot: I can chat with you and answer simple questions!

You: bye
Bot: Bye! Have a great day 👋

```

---

## 🛠️ Tech Stack

- **Python**
- **scikit-learn**
- **TF-IDF Vectorization**
- **Logistic Regression (Multi-class Classification)**

---

## 🧩 Project Structure

```

mini-nlp-chatbot/
│
├── chatbot.py        # Main chatbot logic
├── README.md
└── requirements.txt  # (optional)

````

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/mini-nlp-chatbot.git
cd mini-nlp-chatbot
````

Install dependencies:

```bash
pip install scikit-learn nltk
```

---

## ▶️ Running the Chatbot

```bash
python chatbot.py
```

Type `exit` to quit the chatbot.

---

## 🧠 NLP & ML Explanation

### 1️⃣ Text Vectorization (TF-IDF)

TF-IDF converts text into numbers by measuring:

* How important a word is in a sentence
* How rare the word is across all sentences

This allows the model to understand **semantic patterns** instead of exact text matches.

---

### 2️⃣ Intent Classification (Logistic Regression)

The model learns which words are most associated with each intent.

For example:

* Words like *hi, hello* → Greeting
* Words like *bye, see you* → Goodbye
* Words like *help, support* → Help

The intent with the highest predicted score is selected.

---

## 🚫 Why Not Rule-Based?

❌ Rule-based systems:

* Break easily
* Don’t generalize
* Require many conditions

✅ ML-based systems:

* Handle variations naturally
* Scale better
* Learn from data

---

## 🌱 Future Improvements

* Add text preprocessing (stemming, stopword removal)
* Add confidence thresholds and fallback responses
* Add more intents and dynamic responses
* Convert to a REST API using FastAPI
* Build a web UI (React / Next.js)
* Replace Logistic Regression with a neural network

---

## 🎯 Learning Goals

This project helps understand:

* How NLP works in real applications
* How chatbots were built before LLMs
* Intent classification and text vectorization
* ML decision-making on text data

---

## 📄 License

MIT License — free to use, modify, and learn from.

---

⭐ If you found this project helpful, consider starring the repository!
