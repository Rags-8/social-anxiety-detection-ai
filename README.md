# 🧠 Social Anxiety Detection AI

A full-stack AI-powered web application that analyzes user-provided text using Natural Language Processing (NLP), Machine Learning, and Sentiment Analysis to identify emotional patterns and provide supportive, personalized suggestions.

The application combines a React frontend, FastAPI backend, Scikit-learn, NLTK, and Supabase for authentication and database management.

---

## 🌐 Live Demo

🔗 **[Try Social Anxiety Detection AI](https://social-anxiety-detection.vercel.app/)**

---

## 📌 Overview

Social Anxiety Detection AI provides an interactive platform where users can express their thoughts and feelings through text.

The application processes the submitted text using Natural Language Processing and Sentiment Analysis techniques. It analyzes the emotional tone of the input and provides supportive suggestions based on the results.

Users can also securely log in, view their previous interactions, and explore their history and insights.

> **Note:** This project is developed for educational and technological purposes. It is not a medical diagnostic tool and should not be considered a substitute for professional mental-health care.

---

## ✨ Features

### 🧠 AI-Powered Text Analysis

Analyzes user-provided text using Natural Language Processing and Machine Learning techniques to identify meaningful patterns.

### 💭 Sentiment Analysis

Analyzes the emotional tone of user input and provides an interpretation of the detected sentiment.

### 💡 Supportive Suggestions

Provides personalized and supportive suggestions based on the analysis results.

### 📊 History & Insights

Allows users to view previous interactions and understand patterns through history and visual insights.

### 🔐 User Authentication

Uses Supabase Authentication to securely manage user registration, login, and access to personal data.

### 🗄️ Cloud Database

Uses Supabase Database to securely store application data and user-related information.

### ⚡ FastAPI Backend

Uses FastAPI to build APIs and handle communication between the frontend, AI/ML components, and database.

### 🎨 Modern User Interface

Built with React.js, Vite, and Tailwind CSS to provide a responsive and interactive user experience.

---

## 🏗️ System Architecture

The application follows a full-stack architecture where the frontend communicates with the FastAPI backend, which connects the AI/ML processing layer and Supabase services.

```text
                    ┌─────────────────────┐
                    │        User         │
                    │   Web Application   │
                    └──────────┬──────────┘
                               │
                               ▼
                    ┌─────────────────────┐
                    │   React + Vite      │
                    │   Tailwind CSS      │
                    │   Recharts + Axios  │
                    └──────────┬──────────┘
                               │
                         API Requests
                               │
                               ▼
                    ┌─────────────────────┐
                    │   FastAPI Backend   │
                    │       Python        │
                    └──────────┬──────────┘
                               │
                  ┌────────────┴────────────┐
                  │                         │
                  ▼                         ▼
       ┌────────────────────┐    ┌────────────────────┐
       │    AI / ML Layer   │    │      Supabase      │
       │                    │    │                    │
       │ Scikit-learn       │    │ Authentication     │
       │ NLTK               │    │ Database           │
       │ Sentiment Analysis │    │                    │
       └────────────────────┘    └────────────────────┘
## 🛠️ Tech Stack

### Frontend

Technologies used to build the user interface and interactive features.

- React.js
- Vite
- Tailwind CSS
- Recharts
- Axios

### Backend

Used to build APIs and handle application logic.

- Python
- FastAPI
- Uvicorn

### AI / Machine Learning

Used for natural language processing, text analysis, and sentiment analysis.

- Scikit-learn
- NLTK
- Natural Language Processing (NLP)
- Sentiment Analysis

### Database & Authentication

Used to securely manage users and store application data.

- Supabase Database
- Supabase Authentication

### Development Tools

Tools used for development, testing, and version control.

- Git
- GitHub
- VS Code

### Deployment

The application frontend is deployed using:

- Vercel

---

## 📂 Project Structure

The project is organized into separate frontend, backend, and machine-learning components.

```text
social-anxiety-detection-ai/
│
├── backend/                    # FastAPI backend
│   ├── app/
│   │   ├── main.py             # Main backend application
│   │   └── ...
│   ├── requirements.txt        # Backend dependencies
│   └── ...
│
├── frontend/                   # React frontend
│   ├── src/
│   │   ├── components/         # Reusable UI components
│   │   ├── pages/              # Application pages
│   │   └── ...
│   ├── package.json            # Frontend dependencies
│   └── ...
│
├── train_model.py              # Machine learning model training
├── train_nlp_model.py          # NLP model training
├── Combined Data.csv           # Dataset
├── .gitignore                  # Files ignored by Git
├── LICENSE                     # Project license
└── README.md                   # Project documentation
