 #Heart Stroke Predictions 💗

A Streamlit web app that predicts heart disease / stroke risk using a Logistic Regression model trained on patient health data.

🔗 **Live App:** https://heart-disease-suraj.streamlit.app/




## 📋 Overview

This app takes in a patient's health details — age, sex, chest pain type, blood pressure, cholesterol, blood sugar, ECG results, and more — and predicts their risk of heart disease using a trained machine learning model.

## ✨ Features

- Interactive sliders and dropdowns for entering patient data
- Real-time prediction with a single click
- Clean, simple UI built with Streamlit
- Lightweight and fast — no server setup required to use it

## 🧠 Model Details

- **Algorithm:** Logistic Regression
- **Library:** scikit-learn
- **Input features:**
  - Age
  - Sex
  - Chest Pain Type
  - Resting Blood Pressure (mm Hg)
  - Cholesterol (mg/dL)
  - Fasting Blood Sugar (> 120 mg/dL)
  - Resting ECG
  - Max Heart Rate
  - Exercise-Induced Angina
  - Oldpeak (ST Depression)
  - ST Slope
- **Preprocessing:** Features are scaled using a saved `StandardScaler` (`scale_heart.pkl`) before prediction
- **Model file:** `log_heart.pkl`
- **Expected columns:** `coloumns.pkl` ensures input data matches the format the model was trained on

<!-- If you know your model's accuracy, precision, recall, etc., add them here. Example:
**Accuracy:** 87%
**Precision:** 0.85
**Recall:** 0.83
-->

## 🛠️ Tech Stack

- **Frontend/App:** [Streamlit](https://streamlit.io/)
- **Machine Learning:** scikit-learn
- **Data Handling:** pandas
- **Model Persistence:** joblib

## 🚀 Run It Locally

1. Clone the repository
   ```bash
   git clone https://github.com/surajpatel07-rgb/Heart-Disease-Predictions.git
   cd Heart-Disease-Predictions
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Run the app
   ```bash
   streamlit run app1.py
   ```

4. Open the local URL Streamlit gives you (usually `http://localhost:8501`)

## 📁 Project Structure

```
Heart-Disease-Predictions/
├── app1.py              # Main Streamlit app
├── log_heart.pkl        # Trained Logistic Regression model
├── scale_heart.pkl      # Fitted StandardScaler
├── coloumns.pkl         # Expected input columns
├── requirements.txt     # Python dependencies
└── README.md
```

## 🔮 Future Improvements

- [ ] Add prediction probability/confidence score, not just a yes/no result
- [ ] Try other models (Random Forest, XGBoost) and compare performance
- [ ] Add input validation (e.g. realistic ranges for blood pressure, cholesterol)
- [ ] Display feature importance so users understand what's driving the prediction
- [ ] Add a results history/download option (e.g. export prediction as PDF)
- [ ] Improve UI styling and add data visualizations (e.g. risk factor charts)
- [ ] Add unit tests for the prediction pipeline

## ⚠️ Disclaimer

This app is for educational/portfolio purposes only and is **not a substitute for professional medical advice, diagnosis, or treatment**. Always consult a qualified healthcare provider for any health concerns.

## 👤 Author

**Suraj Patel**
GitHub: [@surajpatel07-rgb](https://github.com/surajpatel07-rgb)
