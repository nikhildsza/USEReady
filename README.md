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

### 🛠️ ML Models Used
- Random Forest (Best performer)
- Decision Tree
- Naive Bayes
- K-Nearest Neighbors (KNN)

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
git clone https://github.com/<your-username>/USEReady.git
cd USEReady
