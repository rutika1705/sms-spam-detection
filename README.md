# 📱 SMS Spam Detection

A machine learning project that classifies SMS messages as **Spam** or **Ham (Not Spam)** using Natural Language Processing (NLP) techniques. The trained model is deployed as an interactive web application using Streamlit.

---

## 🚀 Demo

Run the app locally and enter any SMS message to instantly find out if it's spam!

---

## 📂 Project Structure

```
sms-spam-detection/
├── app.py                      # Streamlit web application
├── sms-spam-detection.ipynb    # Jupyter Notebook (EDA, training, evaluation)
├── spam.csv                    # Dataset (SMS messages labeled spam/ham)
├── model.pkl                   # Trained ML model (serialized)
├── vectorizer.pkl              # TF-IDF Vectorizer (serialized)
└── requirements.txt            # Python dependencies
```

---

## 🧠 How It Works

1. **Data Preprocessing** — The raw SMS text is cleaned by removing punctuation, stopwords, and applying stemming/lemmatization.
2. **Feature Extraction** — Messages are transformed into numerical features using **TF-IDF Vectorization**.
3. **Model Training** — A classification model (e.g., Naive Bayes / Logistic Regression) is trained on the labeled dataset.
4. **Prediction** — The trained model and vectorizer are saved as `.pkl` files and loaded in the web app to predict new messages in real time.

---

## 📊 Dataset

The project uses the classic [SMS Spam Collection Dataset](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset), which contains 5,572 SMS messages labeled as:
- `ham` — Legitimate messages
- `spam` — Unwanted/spam messages

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Python | Core programming language |
| Pandas / NumPy | Data manipulation |
| Scikit-learn | ML model & TF-IDF vectorizer |
| NLTK | Text preprocessing |
| Streamlit | Web application UI |
| Jupyter Notebook | EDA & model development |

---

## ⚙️ Installation & Setup

### 1. Clone the repository
```bash
git clone https://github.com/rutika1705/sms-spam-detection.git
cd sms-spam-detection
```

### 2. Install dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit app
```bash
streamlit run app.py
```

The app will open in your browser at `http://localhost:8501`.

---

## 📈 Model Performance

The model was evaluated on a held-out test set. Key metrics:

| Metric | Score |
|---|---|
| Accuracy | ~97–98% |
| Precision | High |
| Recall | High |
| F1-Score | High |

> Detailed evaluation results can be found in `sms-spam-detection.ipynb`.

---

## 🖥️ App Preview

1. Open the app in your browser.
2. Type or paste any SMS message into the input box.
3. Click **Predict** to see whether it's **Spam 🚨** or **Ham ✅**.

---

## 📌 Future Improvements

- Add deep learning model (LSTM / BERT) for better accuracy
- Deploy to a cloud platform (Heroku / Streamlit Cloud / AWS)
- Support for multiple languages
- Add confidence score display

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

---

## 👩‍💻 Author

**Rutika** — [@rutika1705](https://github.com/rutika1705)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
