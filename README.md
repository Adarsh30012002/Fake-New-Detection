# 📰 Fake-New-Detection
This project is a machine learning web application built with **Streamlit** that classifies news articles as **Fake** or **Real**. It uses a **Logistic Regression** model trained on the widely-used `Fake.csv` and `True.csv` datasets.

---

## 📂 Project Structure

.
├── Fake.csv
├── True.csv
├── train_model.py # Script to train and save the model
├── app.py # Streamlit web app
├── vectorizer.jb # Saved TF-IDF Vectorizer
├── lr_model.jb # Trained Logistic Regression model
└── README.md

---

## 🧠 How It Works

1. **Data Loading**: Loads real and fake news datasets.
2. **Preprocessing**: Text cleaning and TF-IDF vectorization.
3. **Training**: Trains a Logistic Regression classifier.
4. **Saving**: Saves the model and vectorizer using `joblib`.
5. **Prediction**: Users can input news articles into the web app to classify them.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/fake-news-detector.git
cd fake-news-detector
2. Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
If requirements.txt doesn’t exist, manually install:

bash
Copy
Edit
pip install pandas scikit-learn streamlit joblib
3. Train the Model
Run this script to train and save the model:

bash
Copy
Edit
python train_model.py
4. Run the Web App
bash
Copy
Edit
streamlit run app.py
