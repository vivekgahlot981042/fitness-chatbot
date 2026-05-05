# 🏋️ Intent-based AI Fitness Chatbot

> An NLP-powered chatbot that understands fitness-related queries using BERT, GPT, LSTM, and Transformer models.

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)

---

## 📌 Overview

This project is an AI-powered chatbot designed to answer fitness-related questions. It can understand the **intent** behind a user's query (e.g., asking about diet, workout, or injury recovery) and respond accordingly using fine-tuned language models.

---

## ✨ Features

- 🧠 **Intent Recognition** — Classifies user messages into fitness intents (diet, workout, recovery, etc.)
- 🔍 **Entity Extraction** — Extracts key fitness terms from queries (e.g., "protein", "chest day", "cardio")
- 🔄 **Transfer Learning** — Fine-tuned BERT and GPT on a custom fitness dataset
- 📚 **Sequence Understanding** — LSTM handles conversational context; Transformer handles complex queries
- 💬 **Contextual Responses** — Understands follow-up questions within a conversation

---

## 🛠️ Tech Stack

| Component | Technology |
|---|---|
| Language | Python |
| Deep Learning | TensorFlow, Keras |
| Pre-trained Models | BERT, GPT (HuggingFace Transformers) |
| Sequence Models | LSTM, Transformer |
| Environment | Google Colab |

---

## 🏗️ Architecture

```
User Query
    │
    ▼
Text Preprocessing (Tokenization, Cleaning)
    │
    ▼
BERT / GPT Encoder (Transfer Learning)
    │
    ▼
Intent Classifier → Intent Label (e.g., "ask_diet")
    │
    ▼
Entity Extractor → Key Terms (e.g., "protein", "weight loss")
    │
    ▼
Response Generator
    │
    ▼
Chatbot Response
```

---

## 📂 Project Structure

```
fitness-chatbot/
│
├── data/
│   └── fitness_intents.json       # Custom fitness Q&A dataset
│
├── models/
│   ├── intent_classifier.py       # BERT-based intent classifier
│   ├── entity_extractor.py        # NER model
│   └── response_generator.py      # GPT-based response generator
│
├── notebooks/
│   └── training_pipeline.ipynb    # Full training notebook (Colab)
│
├── app.py                         # Main chatbot runner
├── requirements.txt
└── README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repo
git clone https://github.com/comedivek/fitness-chatbot.git
cd fitness-chatbot

# 2. Install dependencies
pip install -r requirements.txt

# 3. Run the chatbot
python app.py
```

---

## 📊 Model Performance

| Model | Accuracy |
|---|---|
| BERT Intent Classifier | ~88% |
| GPT Response Quality | High contextual relevance |
| LSTM Context Memory | Handles 5+ turn conversations |

---

## 🔮 Future Improvements

- Add voice input/output support
- Deploy as a web app using Flask or FastAPI
- Integrate with a fitness tracking API (calories, steps)
- Add multilingual support (Hindi + English)

---

## 👨‍💻 Author

**Vivek Gahlot**
[LinkedIn](https://www.linkedin.com/in/vivek-gahlot-371970256) • [GitHub](https://github.com/comedivek) • [Email](mailto:vt981042@gmail.com)
