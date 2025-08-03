# 🤖 Emotion-Aware Chatbot

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python" alt="Python Version">
  <img src="https://img.shields.io/badge/Hugging%20Face-Transformers-yellow?style=for-the-badge&logo=huggingface" alt="Hugging Face">
  <img src="https://img.shields.io/badge/API-OpenRouter-purple?style=for-the-badge" alt="OpenRouter API">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License">
</p>

A **Python-based emotion-aware chatbot** that leverages a fine-tuned [GoEmotions](https://github.com/google-research/google-research/tree/master/goemotions) model to detect **28 different emotions** and respond empathetically using the **OpenRouter API**. This project was developed as part of a **group collaboration**.

---

## 📋 Table of Contents
- [🚀 Features](#-features)
- [🛠 Setup & Installation](#-setup--installation)
- [📂 Folder Structure](#-folder-structure)
- [📌 My Contributions](#-my-contributions)
- [👥 Collaborators](#-collaborators)

---

## 🚀 Features

-   🎯 **Emotion Detection:** Identifies 28 distinct emotions from user input using a fine-tuned GoEmotions model.
-   💬 **Empathetic Responses:** Generates context-aware, empathetic replies using the powerful **Mixtral-8x7B** model via the OpenRouter API.
-   🖥️ **Console-Based Interaction:** A simple and clean terminal-based chat interface for easy interaction and testing.
-   🛠️ **Custom Fine-Tuning Support:** Designed to be modular, allowing you to easily replace the provided model with your own fine-tuned Hugging Face models.

---

## 🛠 Setup & Installation

Follow these steps to get the chatbot up and running on your local machine.

### 1️⃣ **Clone the Repository**
Open your terminal and run the following commands:
```bash
git clone [https://github.com/YOUR_USERNAME/emotion-aware-chatbot.git](https://github.com/YOUR_USERNAME/emotion-aware-chatbot.git)
cd emotion-aware-chatbot
```

### 2️⃣ **Place Your Fine-Tuned Model**
Place your fine-tuned Hugging Face model folder in the project's root directory. The folder must be named:
```
finetuned_optimized_goemotions
```
Ensure this folder contains the necessary model files, such as:
- `config.json`
- `pytorch_model.bin`
- `tokenizer.json` / `tokenizer_config.json`
- Any other required model or tokenizer files.

### 3️⃣ **Set Up Your API Key**
Edit the `chatbot.py` file and replace the placeholder API key with your own OpenRouter key:
```python
# Find this line in chatbot.py
API_KEY = "YOUR_OPENROUTER_API_KEY"
```

### 4️⃣ **Login to Weights & Biases (Optional)**
If you wish to use Weights & Biases for experiment tracking, log in using your API key.
```bash
wandb login YOUR_WANDB_API_KEY
```

### 5️⃣ **Install Requirements**
Install all the necessary Python packages using pip:
```bash
pip install -r requirements.txt
```

### ▶️ **Run the Chatbot**
You're all set! Start the chatbot with the following command:
```bash
python chatbot.py
```

---

## 📂 Folder Structure

The project directory should be structured as follows:

```plaintext
emotion-aware-chatbot/
├── chatbot.py                      # Main application script
├── requirements.txt                # Project dependencies
├── README.md                       # You are here!
├── sampleImages/                   # Contains sample screenshots
│   ├── chatSample1.png
│   └── chatSample2.png
└── finetuned_optimized_goemotions/ # Your fine-tuned model files
    ├── config.json
    ├── pytorch_model.bin
    └── ... (other model files)
```

---

## 📌 My Contributions

While this was a team project, my primary contributions included:

-   Implementing the core chatbot interaction logic in `chatbot.py`.
-   Integrating the GoEmotions model with the OpenRouter API for generating empathetic responses.
-   Setting up the model loading and emotion classification logic from the fine-tuned model.
-   Managing the `requirements.txt` file and overall project structure for reproducibility.
-   Conducting testing and fine-tuning the response quality through multiple iterations.

---

## 👥 Collaborators

This project was created as part of a fantastic group effort. Credits to all my collaborators:

-   [@LegendarySlayer](https://github.com/LegendarySlayer)
-   [@Strookee](https://github.com/Strookee)
-   [@Brototee](https://github.com/Brototee)
-   [@sanyasingh09](https://github.com/sanyasingh09)
-   [@Utkarsh-Jha171](https://github.com/Utkarsh-Jha171)


> **Note:** This repository contains my personal version of the group project, hosted for portfolio purposes. The original project was collaboratively developed by the team listed above.
