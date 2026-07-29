# 🧠 Social Anxiety Detection AI

A full-stack AI-powered web application that analyzes user text using **NLP, Machine Learning, semantic embeddings, and sentiment analysis** to classify anxiety levels and provide supportive suggestions.

🔗 **Live Demo:** https://social-anxiety-detection.vercel.app

## ✨ Features

- AI-powered text and sentiment analysis
- Anxiety classification: **Low, Moderate, High**
- NLP preprocessing and semantic text analysis
- High-risk phrase detection
- Supportive suggestions and prediction history
- User authentication with Supabase
- PostgreSQL database for storing user interactions
- Interactive insights dashboard

## 🧠 AI / ML

- **NLP:** NLTK, Tokenization, Stopword Removal, Lemmatization
- **Feature Engineering:** Word & Character TF-IDF
- **Embeddings:** Sentence Transformers (`all-MiniLM-L6-v2`)
- **Models:** Logistic Regression, LinearSVC, Multinomial Naive Bayes
- **Ensemble:** Voting Classifier
- **Safety Layer:** Rule-based risk phrase detection

### Prediction Pipeline

```text
User Text
   ↓
NLP Preprocessing
   ↓
TF-IDF / Semantic Embeddings
   ↓
Machine Learning Model
   ↓
Risk Detection
   ↓
Anxiety Level + Suggestions
```

## 📈 Model Performance

### Semantic Embedding + Logistic Regression

| Metric | Score |
|---|---:|
| Accuracy | **87.09%** |

| Class | Precision | Recall | F1 |
|---|---:|---:|---:|
| Low | 0.86 | 0.91 | 0.89 |
| Moderate | 0.58 | 0.81 | 0.67 |
| High | 0.95 | 0.86 | 0.90 |

The ensemble pipeline also achieved **92%+ accuracy** under its V6 feature-engineering configuration.

## 🛠️ Tech Stack

- **Frontend:** React.js, Vite, Tailwind CSS, Recharts, Axios
- **Backend:** Python, FastAPI, Uvicorn
- **AI/ML:** Scikit-learn, NLTK, TF-IDF, Sentence Transformers
- **Database/Auth:** Supabase, PostgreSQL
- **Deployment:** Vercel
- **Tools:** Git, GitHub, VS Code

## 📊 Dataset

Combined mental-health text classification dataset sourced from **Kaggle**, containing approximately **53,000 records**.

Original categories include Normal, Stress, Anxiety, Depression, and Suicidal, which are processed into:

**Low Anxiety · Moderate Anxiety · High Anxiety**

## 🚀 Run Locally

```bash
git clone https://github.com/Rags-8/social-anxiety-detection-ai.git
cd social-anxiety-detection-ai

# Backend
cd backend
pip install -r requirements.txt
python -m uvicorn app.main:app --host 0.0.0.0 --port 8001 --reload

# Frontend
cd ../frontend
npm install
npm run dev
```

Configure Supabase credentials and the backend URL using environment variables.

## 👩‍💻 Author

**S G Raghavi Sai**  
Computer Science & Engineering (Artificial Intelligence)

[GitHub](https://github.com/Rags-8) • [LinkedIn](https://www.linkedin.com/in/s-g-raghavi-sai-a7a4482bb/)

> ⚠️ This project is for educational purposes and is not a medical diagnostic tool.

**License:** MIT
