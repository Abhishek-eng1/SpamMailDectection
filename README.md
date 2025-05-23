# 📧 Spam Mail Detection using Machine Learning

A machine learning-based system that detects and classifies emails as spam or not spam using NLP techniques.

---

## 📁 Project Structure

``` bash

Spam-Mail-Detection/
├── spam.csv # Training dataset
├── test_emails.csv # Test email samples for prediction
├── model.pkl # Saved trained model
├── vectorizer.pkl # Saved TF-IDF vectorizer
├── predictions.csv # Output predictions
├── spam_detector.py # Complete Python code (training + prediction)
├── requirements.txt # Required Python packages
└── README.md # Documentation file
```

---

## 🧠 How It Works

- Preprocesses email content (removing punctuation, stopwords, stemming).
- Converts text to numeric format using **TF-IDF Vectorizer**.
- Trains a **Multinomial Naive Bayes** model.
- Predicts whether new emails are spam or ham.
- Outputs results in a new file (`predictions.csv`).

---

## 📦 Requirements

Install dependencies using:

```bash
pip install -r requirements.txt
requirements.txt content:
nginx
Copy
Edit
pandas
scikit-learn
nltk
joblib
🧪 Dataset Used
📄 spam.csv
Used for training the model.

Contains 2 columns:

v1 — the label (spam or ham)

v2 — the email content

📄 test_emails.csv
Contains new email samples for testing predictions.

Should have one column: message

📄 predictions.csv
Output file containing:

message — original test email

label — predicted class (spam or ham)
