🧠 Personality Prediction Using Text Data (MBTI Classification)
This project aims to predict personality types based on a person's text using Natural Language Processing (NLP) and Machine Learning techniques.
The dataset used contains MBTI (Myers–Briggs Type Indicator) personality types along with users' text posts.


📌 Objectives
  - Preprocess and clean user-generated text

  - Convert text to numerical features using TF-IDF

  - Train classification models to predict MBTI types

  - Handle class imbalance using SMOTE

  - Evaluate using accuracy, precision, recall, F1-score, and confusion matrix
    


📊 Dataset
  - Source: Kaggle - MBTI Personality Dataset

  - Size: ~8600 samples

  - Features:

    - type: MBTI personality type (16 types)

    - posts: Text data (user-generated content)

🧹 Preprocessing:

Cleaning, stopword removal, tokenization, stemming


✨ Vectorization:

TF-IDF


⚖️ Class Imbalance Handling

SMOTE (Synthetic Minority Oversampling Technique)


🧪 Models Used:-

  1)Logistic Regression

  2)Random Forest

  

📈 Model Evaluation
Metric	Value
Accuracy	~65.1%
Macro F1	~0.55
Weighted F1	~0.66


💡 Key Insights
Class imbalance had a significant impact on model performance

SMOTE helped improve recall for underrepresented personality types (like ESTJ, ISFP, ESFJ)

TF-IDF worked well for this task

Models struggled where personality types had overlapping traits


🛠 Tech Stack
  Python (NLP & ML)

  Libraries: pandas, scikit-learn, matplotlib, seaborn, imbalanced-learn


📁 Files
  - PersonalityPredictor.ipynb: Jupyter Notebook with code

  - README.md: This file

📌 To Do
  - Try deep learning models (e.g., LSTM, BERT)

  - Improve preprocessing with better lemmatization

  - Add personality-type-specific analysis

