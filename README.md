
# 📰 Fake News Detection App

A machine learning web application that detects whether a news article is **Fake** or **Real** using **TF-IDF vectorization** and a **Logistic Regression** model. Built with **Streamlit** for interactive predictions.

## 🚀 Features

- Real-time fake news classification
- Built with Scikit-learn and Streamlit
- TF-IDF vectorization of news content
- Easy-to-use interface

## 🗂️ Project Structure

```
.
├── Fake.csv              # Fake news dataset
├── True.csv              # Real news dataset
├── train_model.py        # Model training script
├── app.py                # Streamlit application
├── vectorizer.jb         # Saved TF-IDF vectorizer
├── lr_model.jb           # Trained model
└── README.md             # Project documentation
```

## 🔧 Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/fake-news-detector.git
cd fake-news-detector
```

### 2. Create Virtual Environment (Optional but Recommended)

```bash
python -m venv venv
```

Activate it:

- On macOS/Linux:

  ```bash
  source venv/bin/activate
  ```

- On Windows:

  ```bash
  venv\Scripts\activate
  ```

### 3. Install Dependencies

If you have a `requirements.txt` file:

```bash
pip install -r requirements.txt
```

Or install manually:

```bash
pip install pandas scikit-learn streamlit joblib
```

## 🧠 Model Training

Train your model and save the vectorizer and model:

```bash
python train_model.py
```

Outputs:
- `vectorizer.jb`
- `lr_model.jb`

## 💻 Run the Web App

Launch the Streamlit app locally:

```bash
streamlit run app.py
```

Access it at [http://localhost:8501](http://localhost:8501) in your browser.

## 🧪 Example Input

Try pasting this into the app:

```
Scientists discovered a new energy source that could change the world.
```

Click **Check News** – the app will tell you whether it’s real or fake.

## 📄 Example Configuration (YAML)

```yaml
name: Fake News Detector
version: 1.0
dependencies:
  - pandas
  - scikit-learn
  - streamlit
  - joblib
author: Adarsh Kumar
license: MIT
```

## 🖥️ Bash Script Example

```bash
#!/bin/bash

echo "Training model..."
python train_model.py

echo "Launching app..."
streamlit run app.py
```

Save this as `run.sh` if you want to automate your workflow.

## 📊 Dataset

This project uses:
- [Fake and Real News Dataset on Kaggle](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)

Labels:
- `0` – Fake news
- `1` – Real news

## ✅ Requirements

- Python 3.7+
- pandas
- scikit-learn
- streamlit
- joblib

## 📌 Future Enhancements

- Show model confidence score
- Add support for headline-only classification
- Deploy using Streamlit Cloud or Hugging Face Spac
