# ⚡ DeepSeek RAG for Electrical STEM | Fine-Tuned & Colab-Integrated

This project consists of two major components:

1. **Fine-tuning the DeepSeek 8B model** on a domain-specific Electrical and Electronics Engineering (EEE) dataset to assist students, researchers, and professionals.
2. **Building a Retrieval-Augmented Generation (RAG) system** using LangChain and Ollama, fully integrated to run inside Google Colab with Streamlit UI and inbuilt vector store.

---

## 📁 Project Structure

### 1️⃣ Fine-Tuning DeepSeek 8B on EEE Data

This module focuses on enhancing the DeepSeek 8B model with domain-specific knowledge from Electrical and Electronics Engineering.

#### 🧠 Key Highlights:
- Uses **PEFT** techniques: **LoRA**, **QLoRA**, and **Clara** for parameter-efficient fine-tuning.
- Built with **Unsloth** for efficient and memory-optimized training.
- Tailored to answer **technical queries** from EEE students, faculty, and researchers.
- Outputs a quantized, ready-to-deploy model for inference.

---

### 2️⃣ RAG Pipeline with Colab Integration

This part constructs a fully working **Retrieval-Augmented Generation** (RAG) system with:

#### 🔧 Components:
- **LangChain + LlamaIndex** for orchestration and retrieval.
- **Ollama** for running the fine-tuned DeepSeek 8B model inside Colab.
- **Inbuilt Vector Store** (LlamaIndex default) for document embeddings.
- **Streamlit Interface** for live chat with the model.
- **Xtream UI Feature** for enhanced UX in Colab notebooks.
- **Ngrok Tunneling** used to expose the Streamlit app directly from Colab.

#### 🌐 Colab-Friendly Features:
- No server setup required — everything runs **in Colab**.
- Easily adaptable to any fine-tuned LLM checkpoint hosted locally.
- Designed for **interactive EEE knowledge retrieval**.

---

## 🛠️ Tech Stack

| Component          | Description                            |
|-------------------|----------------------------------------|
| **DeepSeek 8B**    | Base model used for fine-tuning        |
| **PEFT (LoRA/QLoRA/Clara)** | Efficient training modules     |
| **Unsloth**        | Lightweight fine-tuning backend        |
| **LangChain**      | Orchestration of RAG pipeline          |
| **LlamaIndex**     | Embedding + Vector Store               |
| **Ollama**         | Model inference inside Colab           |
| **Streamlit**      | Frontend interface for Q&A             |
| **Ngrok**          | Public URL for Streamlit in Colab      |

---

## 🚀 Use Cases

- 📘 **EEE Students** – Get answers to course-related queries.
- 🧑‍🔬 **Researchers** – Retrieve relevant literature-style summaries.
- 👨‍🏫 **Faculty** – Use it as a teaching assistant in labs or tutorials.

---

## 📌 Note

Ensure you have Colab Pro or sufficient runtime to run Ollama with large models. All components are optimized for in-notebook use without local server dependencies.

---

## 📎 Quick Start

Open the two notebooks in order:

1. `fine_tune_deepseek_eee.ipynb` – Train your model on your dataset.
2. `rag_with_ollama_colab.ipynb` – Launch Streamlit RAG inside Colab.

Happy Hacking! ⚡
