# LLM-chatbot
 — pdf-question-answering-bot

 
# 📚 PDF Question Answering Bot

A lightweight command-line tool that extracts text from a PDF and uses a transformer-based question-answering model to answer natural language questions about its content.

---

## 🔍 How It Works

1. 📄 **Extracts text** from each page of the PDF using `PyMuPDF (fitz)`
2. 📚 **Splits the text** into overlapping chunks to ensure context is preserved
3. 🧠 **Uses a pre-trained QA model** (`distilbert-base-cased-distilled-squad`) from HuggingFace Transformers to find the best answer to your question across all chunks

---

## 🛠️ Technologies Used

- [`transformers`](https://huggingface.co/transformers/) (by Hugging Face)
- [`PyMuPDF`](https://github.com/pymupdf/PyMuPDF)
- Python 3.8+

---

## 📦 Installation

```bash
git clone https://github.com/sebtaoui/pdf-question-answering-bot.git
cd pdf-question-answering-bot
pip install -r requirements.txt
