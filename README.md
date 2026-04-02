# 📝 Text Summarizer

A web-based text summarization app built with **FastAPI** and a fine-tuned **T5 transformer model** from HuggingFace. Paste any long-form text and get a concise summary instantly.

![Text Summarizer App]
<img width="1470" height="799" alt="Screenshot 2026-04-02 at 10 20 02 AM" src="https://github.com/user-attachments/assets/06e4b745-0e1c-44c9-942d-d2e604a1dfc6" />

## 🚀 Features

- Summarizes long text using a fine-tuned T5 model
- Clean and simple web UI
- Fast inference with FastAPI backend
- Supports CPU, CUDA, and Apple MPS (M1/M2) devices

## 🛠️ Tech Stack

- **Backend:** FastAPI, Uvicorn
- **ML Model:** T5 (fine-tuned on SAMSum dataset)
- **Frontend:** HTML, CSS (Jinja2 templates)
- **Libraries:** HuggingFace Transformers, PyTorch

## ⚙️ Setup & Installation

### 1. Clone the repository
```bash
git clone https://github.com/your-username/text_sumarizer.git
cd text_sumarizer
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Download the model
The fine-tuned model is not included in this repo due to its size.
Download it and place it in a folder named `saved_summary_model/` in the root directory.

> The model was fine-tuned on the [SAMSum dataset](https://huggingface.co/datasets/samsum) for dialogue summarization.

### 5. Run the app
```bash
uvicorn app:app --reload
```

Then open your browser and go to `http://127.0.0.1:8000`

## 📁 Project Structure
```
text_sumarizer/
├── app.py                  # FastAPI application
├── templates/
│   └── index.html          # Frontend UI
├── saved_summary_model/    # Fine-tuned T5 model (not included)
├── requirements.txt
└── .gitignore
```

## 🧠 Model

The T5 model was fine-tuned on the SAMSum conversational dataset which contains
thousands of messenger-like dialogues paired with human-written summaries.


## To add it to your repo

bash# create the file
touch README.md
# paste the content above, then:
git add README.md
git commit -m "add README"
git push
