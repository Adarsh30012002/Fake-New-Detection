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

yaml
Copy
Edit

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
📊 Dataset
The project uses:

Fake.csv

True.csv

Each contains news articles labeled as fake or real.

📦 Model Details
Vectorizer: TfidfVectorizer (stopwords = "english")

Classifier: LogisticRegression

Accuracy: Depends on data split, generally above 90%.

🧪 Example
Try pasting this in the web app:

pgsql
Copy
Edit
The President announced a new economic policy today that is expected to boost growth.
The app will classify it as likely Real or Fake.

📌 To Do
 Add support for news headlines only

 Display model confidence score

 Add explanatory model visualizations using SHAP/LIME

📃 License
MIT License

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

✉️ Contact
For questions or suggestions, reach out at your.email@example.com

yaml
Copy
Edit

---

Let me know if you'd like a `train_model.py` script to go along with this README or a `requirements.txt` file generated.







