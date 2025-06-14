{
 "cells": [
  {
   "cell_type": "markdown",
   "id": "290ec20c-0a08-4abb-9b2a-5cb1b4497010",
   "metadata": {},
   "source": [
    "# 🧠 Personality Prediction Using Text Data (MBTI Classification)\n",
    "\n",
    "This project aims to predict personality types based on a person's text using Natural Language Processing (NLP) and Machine Learning techniques. The dataset used contains MBTI (Myers–Briggs Type Indicator) personality types along with users' text posts.\n",
    "\n",
    "---\n",
    "\n",
    "\n",
    "## 📌 Objectives\n",
    "\n",
    "- Preprocess and clean user-generated text\n",
    "- Convert text to numerical features using TF-IDF\n",
    "- Train classification models to predict MBTI types\n",
    "- Handle class imbalance using SMOTE\n",
    "- Evaluate using accuracy, precision, recall, F1-score, and confusion matrix\n",
    "\n",
    "---\n",
    "\n",
    "## 📊 Dataset\n",
    "\n",
    "- **Source**: [Kaggle - MBTI Personality Dataset](https://www.kaggle.com/datasnaek/mbti-type)\n",
    "- **Size**: ~8600 samples\n",
    "- **Features**:\n",
    "  - `type`: MBTI personality type (16 types)\n",
    "  - `posts`: Text data (user-generated content)\n",
    "\n",
    "---\n",
    "\n",
    "## 🧹 Techniques Used\n",
    "\n",
    "- **Preprocessing**: Cleaning, stopword removal, tokenization, stemming\n",
    "- **Vectorization**: TF-IDF\n",
    "- **Class Imbalance Handling**: SMOTE (Synthetic Minority Oversampling Technique)\n",
    "- **Models**: Logistic Regression, Random Forest, etc.\n",
    "- **Evaluation**: Accuracy, F1-score, confusion matrix, visualization\n",
    "\n",
    "---\n",
    "\n",
    "## 🧪 Model Performance (After SMOTE)\n",
    "\n",
    "| Metric       | Value        |\n",
    "|--------------|--------------|\n",
    "| Accuracy     | ~65.1%       |\n",
    "| Macro F1     | ~0.55        |\n",
    "| Weighted F1  | ~0.66        |\n",
    "\n",
    "> SMOTE helped improve recall for underrepresented classes such as ESTJ, ISFP, and ESFJ.\n",
    "\n",
    "---\n",
    "\n",
    "## 📈 Key Insights\n",
    "\n",
    "- **Class imbalance** had a significant impact on model performance.\n",
    "- **TF-IDF** vectorization worked effectively for this task.\n",
    "- **SMOTE** improved performance across less frequent personality types.\n",
    "- Models struggled where personality types have overlapping traits.\n",
    "\n",
    "---\n"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python [conda env:base] *",
   "language": "python",
   "name": "conda-base-py"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 3
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython3",
   "version": "3.12.7"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 5
}
