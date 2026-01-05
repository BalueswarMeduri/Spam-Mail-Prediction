Spam Mail Detection System

A full-stack Spam Mail Detection web application that uses Machine Learning + FastAPI + React.js to classify emails as Spam or Safe in real time.

Project Overview

This project detects whether an email message is spam or not using Natural Language Processing (NLP) techniques.
The trained ML model is exposed via a FastAPI REST API, and a React.js frontend is used to interact with the model.

🧠 Machine Learning Model
🔹 Dataset

SMS Spam Collection Dataset
Source: Kaggle
Total messages: 5,574

Labels:
spam → spam email
ham → normal (safe) email

🔹 Data Preprocessing

Removed null values
Converted labels:
spam → 0
ham → 1

Text data transformed using TF-IDF Vectorization
Stop words removed
Text converted to lowercase

🔹 Model Used
Logistic Regression
Feature Extraction: TfidfVectorizer
Train/Test Split: 80% / 20%
Achieved high accuracy on both training and testing data

🔹 Model Files
Saved after training:
spam_model.sav → trained Logistic Regression model
tfidf_vectorizer.sav → TF-IDF vectorizer

⚙️ Backend (FastAPI)
🔹 API Framework
FastAPI
Pydantic for request validation

🔹 API Endpoint
POST /spam_prediction
🔹 CORS

Enabled for all origins to allow frontend integration

🌐 Deployment
🔹 Backend Deployment

Backend exposed using ngrok
Public API URL example:
https://wilton-gadgety-boozily.ngrok-free.dev/spam_prediction


Note: ngrok URLs are temporary and may change on restart.

🎨 Frontend (React.js)
🔹 Tech Stack
React.js
Tailwind CSS
Fetch API for backend communication


🟢 Green → Safe

Responsive design (mobile & desktop)

Dataset & GitHub resource links
