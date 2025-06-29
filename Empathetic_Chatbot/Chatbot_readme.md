# 🤖 Mental Health Support Chatbot

This project implements a simple mental health chatbot fine-tuned on the **EmpatheticDialogues** dataset. The chatbot is designed to provide supportive, emotionally aware responses for users experiencing stress, anxiety, or emotional distress.

---

## 🎯 Objective

To fine-tune a small language model (DistilGPT2) using real human dialogue data so that it can respond with **empathy and understanding**. This is part of a broader effort to explore the capabilities of language models in mental health support settings.

---

## 📚 Dataset

- **Name**: [EmpatheticDialogues](https://huggingface.co/datasets/empathetic_dialogues) by Facebook AI
- **Purpose**: Contains ~25k conversations where a speaker describes a situation and the listener responds empathetically.
- **Format**: JSON with fields like `context`, `utterance`, and `emotion`.

---

## 🧠 Model and Tools

- **Base Model**: `distilgpt2` (small, efficient variant of GPT2)
- **Library**: `transformers` by Hugging Face
- **Fine-tuning API**: Hugging Face `Trainer`
- **Tokenizer**: GPT2 tokenizer
- **Interface**: Jupyter Notebook (with option to add Streamlit or CLI)

---

## ⚙️ Training Setup

- Trained on a **subset** of ~500 examples (for demo purposes)
- Used `Trainer` API with:
  - `num_train_epochs=1`
  - `batch_size=4`
  - `learning_rate=5e-5`
- Saved model using `.save_model()` for reuse

---

## 💬 How It Works

1. Input a user message (e.g., "I'm feeling anxious lately.")
2. The model generates a short, supportive response.
3. Generation parameters (top-p, temperature, etc.) were tuned for empathy and coherence.


## The model is trained locally and excluded due to GitHub's file size limits. You can re-run the notebook to train or load the model.
