
# 📧 Spam Mail Detection Web App

This project is a **machine learning-powered web application** that detects whether an email is spam or not. It compares the performance of five popular ML models, ultimately selecting **Naive Bayes** as the most accurate. A Flask-based web app lets users input email text and get real-time predictions.

---

## 🚀 Features

- Implemented and evaluated five classification models:
  - ✅ **Naive Bayes**
  - Support Vector Machine (SVM)
  - Random Forest
  - Logistic Regression
  - K-Nearest Neighbors (KNN)
- Measured and compared model accuracy
- Saved the best model (`Naive Bayes`) as `model.pkl`
- Built an interactive Flask web interface for live spam prediction

---

## 📊 Model Accuracy Comparison

| Model                | Accuracy   |
|----------------------|------------|
| ✅ Naive Bayes        | **97.14%** |
| Logistic Regression  | 96.67%     |
| SVM                  | 96.19%     |
| Random Forest        | 94.76%     |
| K-Nearest Neighbors  | 77.62%     |

➡️ Based on this evaluation, **Naive Bayes** was chosen as the final model.

---

## 🛠️ Tech Stack

- **Backend**: Python, Flask
- **ML Libraries**: `scikit-learn`, `pandas`, `numpy`, `joblib`
- **Frontend**: HTML, CSS (via `templates` and `static` folders)

---

## 📁 Project Structure

```
SPAM_DETECTION/
├── static/                  # CSS files
├── templates/
│   └── index.html           # Web UI
├── app.py                   # Flask application
├── train.py                 # Preprocessing and training script
├── NB.py                    # Naive Bayes model
├── SVM.py                   # SVM model
├── KNN.py                   # KNN model
├── RF.py                    # Random Forest model
├── LR.py                    # Logistic Regression model
├── model.pkl                # Saved Naive Bayes model
└── README.md                # Project documentation
```

---

## ⚙️ How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/spam-mail-detector.git
cd spam-mail-detector
```

### 2. Create Virtual Environment

```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install flask scikit-learn pandas numpy joblib
```

> Or use a `requirements.txt`:

```text
Flask
scikit-learn
pandas
numpy
joblib
```

### 4. Run the Flask App

```bash
python app.py
```

Then open your browser and go to [http://127.0.0.1:5000](http://127.0.0.1:5000)

---

## 🖥️ Web Interface

- Paste or type your email content
- Hit **Submit**
- Instantly see the result: ✅ Not Spam or 🚫 Spam

---

## 🧠 How It Works

1. Email text is preprocessed (lowercasing, punctuation removal, tokenization).
2. TF-IDF vectorization is applied.
3. The trained Naive Bayes model makes predictions.
4. Result is rendered on the web page.

---

## 📌 Future Scope

- Add support for `.txt` or `.eml` file uploads
- Use deep learning models (e.g., LSTM or BERT)
- Store prediction history for users
- Improve UI with Bootstrap or Tailwind

---

## 👨‍💻 Author

**Srujan Patel**  
BTech CSE @ IIT Indore  
📧 [Your Email]  
🔗 [LinkedIn](https://linkedin.com/in/your-profile)

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
