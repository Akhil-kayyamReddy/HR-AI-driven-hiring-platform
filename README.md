# 🤖 HR AI-Driven Hiring Platform

## 📌 Overview
This project is an AI-powered recruitment system that automates resume screening and candidate evaluation using machine learning and NLP techniques.

The system analyzes resumes and matches them with job descriptions to rank candidates efficiently.

---

## 🚀 Features
- Resume parsing and text extraction
- Candidate-job matching using ML
- Ranking system based on relevance
- Web interface for uploading resumes
- Automated filtering for recruiters

---

## 🛠️ Tech Stack
- Python
- Flask
- Scikit-learn
- Pandas, NumPy
- NLP (TF-IDF / Cosine Similarity)

---

## ▶️ How to Run

```bash
git clone https://github.com/your-username/hr-ai-hiring-platform.git
cd hr-ai-hiring-platform
pip install -r requirements.txt
python app.py

📌 Step-by-Step Workflow:
User Input
Recruiter enters:
Resume text
Job description
Input is taken via the web interface (index.html)
Data Preprocessing
Text is cleaned using utils.py
Removes:
Special characters
Stopwords
Noise
Converts text into a standardized format
Feature Extraction
Uses TF-IDF Vectorizer
Converts resume & job description into numerical vectors
Similarity Calculation
Applies Cosine Similarity
Measures how closely resume matches job role
Scoring & Ranking
Generates a match score (0–100%)
Higher score = better candidate fit
Result Display
Output is shown on the UI (result.html)
Recruiter sees candidate relevance instantly
🏗️ System Architecture

Think of this as a 3-layer pipeline 🧱→🧠→📊

🧩 1. Presentation Layer (Frontend)
Files: templates/, static/
Technologies: HTML, CSS
Responsibilities:
Accept user input
Display results
Provide simple UI

⚙️ 2. Application Layer (Backend)
File: app.py
Framework: Flask
Responsibilities:
Handle HTTP requests
Connect frontend with ML model
Process user inputs

🧠 3. AI/ML Layer
Files: model.py, utils.py
Responsibilities:
Text preprocessing
Feature extraction (TF-IDF)
Similarity calculation
Resume ranking logic

📂 4. Data Layer
Folder: data/
Contains:
Sample resumes
Test inputs


🔗 Architecture Flow (Simple View)
User Input (UI)
      ↓
Flask Backend (app.py)
      ↓
Preprocessing (utils.py)
      ↓
ML Model (model.py)
      ↓
Similarity Score
      ↓
Result Display (UI)


