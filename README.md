## 🫀 CardioGuard – Cardiovascular Disease Prediction System
## 🏥 Overview

CardioGuard is a production-ready Machine Learning web application that predicts the likelihood of cardiovascular disease using a Random Forest Classifier.

The system provides real-time risk analysis based on 11 health indicators through a modern, healthcare-themed responsive interface.

Created by Abhay Javiya.


This project demonstrates:

End-to-end ML workflow

Model deployment with Flask

REST-style prediction API

Cloud deployment readiness

## 🚀 Live Demo

🔗 https://cardio-guard-s94f.onrender.com

## ✨ Key Features

🧠 Machine Learning Prediction Engine (Random Forest)

⚡ Real-time prediction using AJAX (Fetch API)

📊 Probability-based risk scoring

🎨 Modern Glassmorphism UI Design

📱 Fully Responsive Layout

☁️ Cloud Deployment Ready (Render / Railway)

## 🛠️ Tech Stack
🔹 Frontend

HTML5

CSS3

Bootstrap 5

JavaScript (Fetch API)

🔹 Backend

Python

Flask

Gunicorn (Production Server)

🔹 Machine Learning

Scikit-Learn (Random Forest Classifier)

Pandas

NumPy

Joblib (Model Serialization)

🔹 Deployment

Render / Railway

## 📂 Project Structure
```
CardioGuard/
│
├── app.py                 # Flask Application
├── model/
│   └── cardio_model.pkl   # Pre-trained ML Model
│
├── static/
│   ├── css/
│   ├── js/
│   └── plots/
│
├── templates/
│   ├── home.html
│   ├── about.html
│   ├── predict.html
│   ├── model_info.html
│   └── visuals.html
│
├── requirements.txt
├── Procfile
├── .gitignore
└── README.md
```

## ⚙️ Setup & Installation

### Prerequisite
Ensure you have Python 3.8+ installed.

1. **Clone or Download the Project**
   ```bash
   git clone <repo_url>
   cd <project_folder>
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Train the Model** (Important!)
   You must generate the model file first.
   ```bash
   python model/train_model.py
   ```
   *This will create `model/cardio_model.pkl`.*

4. **Run the Application**
   ```bash
   python app.py
   ```
   Open your browser at `http://127.0.0.1:5000`.

## ☁️ Deployment Guide (Render)

1. **Push to GitHub**: Upload this code to a GitHub repository.
2. **Create New Web Service**: Go to [Render Dashboard](https://dashboard.render.com/) -> New -> Web Service.
3. **Connect Repo**: Select your repository.
4. **Settings**:
   - **Environment**: Python 3
   - **Build Command**: `pip install -r requirements.txt && python model/train_model.py` (Adding training here ensures model exists on cloud)
   - **Start Command**: `gunicorn app:app`
5. **Deploy**: Click Create Web Service.

## ⚠️ Disclaimer
This application is for educational purposes only and should not be used as a substitute for professional medical diagnosis.
