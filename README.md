# 📰 Fake News Detector

A machine learning-based web application that classifies news articles as **Real** or **Fake** using Natural Language Processing techniques and a deployed interactive interface.

---

## 🚀 Overview

This project implements an end-to-end pipeline for fake news detection using **TF-IDF feature extraction** and a **Logistic Regression model**.

It includes:

* Data preprocessing and cleaning
* Feature engineering using TF-IDF
* Model training and evaluation
* Interactive web app for real-time predictions

---

## 🎯 Features

* Classifies news as **REAL** or **FAKE**
* Clean and modular ML pipeline
* Command-line prediction support
* Interactive UI using Streamlit
* Model evaluation with metrics and visualizations

---

## 🧠 How It Works

1. **Text Preprocessing**

   * Lowercasing, removing noise (URLs, punctuation, etc.)

2. **Feature Extraction**

   * Convert text → numerical vectors using TF-IDF

3. **Model Training**

   * Logistic Regression learns patterns in fake vs real news

4. **Prediction**

   * Outputs label + probability score

---

## 📁 Project Structure

```
fakenewsdetector/
│
├── data/                # Dataset files
├── outputs/             # Trained model & evaluation results
├── src/                 # Source code
│   ├── train_model.py
│   ├── streamlit_app.py
│   ├── detect_fake_news.py
│   ├── text_clean.py
│   └── utils.py
└── README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/umerriaz392/FakeNewsDetector
cd FakeNewsDetector
pip install -r requirements.txt
```

---

## ▶️ Run the Project

### Train the Model

```bash
python src/train_model.py --real data/True.csv --fake data/Fake.csv --text-col text --outdir outputs
```

### Run Web App

```bash
streamlit run src/streamlit_app.py
```

Then open:

```
http://localhost:8501
```

---

## 📊 Model Details

* Algorithm: Logistic Regression
* Feature Engineering: TF-IDF
* Task: Binary Text Classification

> Note: Performance is high on the provided dataset, but real-world accuracy may vary due to noise and data diversity.

---

## 🧪 Example

Input:

```
"Breaking: Major political event shocks the nation..."
```

Output:

```
Prediction: FAKE
Confidence: 0.78
```

---

## 🛠️ Tech Stack

* Python
* scikit-learn
* pandas / numpy
* matplotlib
* Streamlit

---

## 📌 Future Improvements

* Use transformer models like BERT
* Add explainability (SHAP / LIME)
* Improve dataset diversity
* Deploy online (Streamlit Cloud / Hugging Face)

---

## 👨‍💻 Author

**Muhammad Umer Riaz**
BS Computer Science (2022–2026)
PIEAS

---

## ⭐ Why This Project Matters

Fake news detection is a real-world problem in today’s digital age.
This project demonstrates practical skills in:

* NLP
* Machine Learning
* Model deployment

---
