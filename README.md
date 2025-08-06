# 📄 USEReady Assignment Submissions

This repository contains the solutions to two assignments:

- 🔹 **Assignment 1**: Load Type Classification using Machine Learning
- 🔹 **Assignment 2**: Contract Metadata Extraction using Gemini LLM (Docx, PDF, PNG)

---

## 📁 Contents

| File / Folder         | Description                                     |
|-----------------------|-------------------------------------------------|
| `assign-1.zip`        | Contains the notebook and models for assignment 1 |
| `assign-2.zip`        | Contains backend & frontend code for assignment 2 |
| `requirements.txt`    | All Python dependencies required                |
| `README.md`           | This file                                       |

---

## ✅ Assignment 1 – Load Type Classification (ML)

### 🔍 Description

A classification problem where the goal is to predict the `Load_Type` based on other features like `Usage_kWh` and time-based patterns.

### 💠 ML Models Used
- Random Forest (Best performer)
- Decision Tree
- Naive Bayes

### 📈 Evaluation Metric
- Accuracy
- Precision, Recall, F1-score
- Classification Report for each model

📁 See notebook and results inside `assign-1.zip`.

---

## ✅ Assignment 2 – Contract Metadata Extraction (LLM)

### 🔍 Description

Builds an AI system to extract metadata from `.docx`, `.pdf`, and `.png` scanned documents using **LangChain + Gemini 2.5 API**.

### 📦 Extracted Fields:
- `agreement_value`
- `start_date`
- `end_date`
- `renewal_notice`
- `party_one`
- `party_two`

---

## ⚙️ Setup Instructions

### 1️⃣ Clone the Repo

```bash
git clone https://github.com/nikhildsza/USEReady.git
cd USEReady
```

### 2️⃣ Create and Activate a Virtual Environment

```bash
python -m venv env
source env/bin/activate    # For Linux/macOS
env\Scripts\activate.bat   # For Windows
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Set Up Gemini API Key

Create a `.env` file in the `backend/` folder and add:

```
GOOGLE_API_KEY=your_api_key_here
```

Get the key from: https://makersuite.google.com/app/apikey

---

## 🚀 Running the Project

### ✅ Start FastAPI Backend (Assignment 2)

```bash
cd backend
uvicorn main:app --reload
```

> This exposes the API at: `http://localhost:8000/extract`

### ✅ Start Streamlit Frontend

Open a new terminal:

```bash
cd frontend
streamlit run app.py
```

> This opens a UI in your browser to upload documents and view metadata.

---

## 🧠 Notes

- No RegEx or rule-based logic used — only LLM-powered structured extraction
- Supports `.docx`, `.pdf`, `.png`, `.jpg` via LangChain + Tesseract OCR + Gemini
- Evaluation based on **per-field recall**, as mentioned in the assignment

---

## 🛠️ Tools & Libraries

- FastAPI
- Streamlit
- LangChain
- Gemini 2.5 (Google Generative AI)
- python-docx, PyMuPDF, pytesseract
- scikit-learn, pandas, matplotlib (Assignment 1)

---

## 🤝 Acknowledgments

Submitted as part of USEReady assignments.

---
