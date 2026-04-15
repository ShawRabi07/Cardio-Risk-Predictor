<div align="center">

# 🫀 Cardio Risk Predictor

### AI-Powered Cardiovascular Disease Risk Assessment

[![Streamlit App](https://img.shields.io/badge/Streamlit-Live%20Demo-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://your-live-link.streamlit.app)
[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML%20Framework-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rabi%20Shaw-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rabi-shaw-6a4223297/)

<br/>

> A clinical-grade machine learning application that assesses cardiovascular disease risk in real time using 14 patient features, powered by a high-accuracy Gradient Boosting Classifier.

<br/>

![banner](https://img.shields.io/badge/Accuracy-High%20Performance%20Model-success?style=flat-square) ![status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen?style=flat-square) ![license](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

</div>

---

## 📌 Overview

**Cardio Risk Predictor** is a professional health analytics application that estimates a patient's probability of cardiovascular disease (CVD). It processes clinical inputs — including vitals, lifestyle factors, and automatically engineered medical metrics — and returns a real-time risk classification: **Low Risk** or **High Risk**.

The underlying model is a tuned **Gradient Boosting Classifier** trained on a large clinical dataset, achieving high predictive accuracy across the full feature set.

---

## ✨ Key Features

| Feature | Description |
|---|---|
| ⚡ **Real-Time Scoring** | Instant CVD probability estimation on every input change |
| 🧮 **Feature Engineering** | Auto-derives **BMI** and **Pulse Pressure** from raw inputs |
| 🎯 **Binary Classification** | Clear Low / High Risk output with probability confidence |
| 📊 **Interactive Dashboard** | Clean Streamlit UI for seamless clinical data entry |
| 🔍 **Explainable Inputs** | Transparent handling of BP, cholesterol, glucose, and lifestyle flags |
| 💾 **Persistent Model** | Pre-trained `.joblib` model loads instantly — no re-training needed |

---

## 🖥️ Live Demo

> 🔗 **[Launch the App →]([https://your-live-link.streamlit.app](https://cardiovas.streamlit.app/))**

Enter patient details (age, blood pressure, cholesterol, BMI, etc.) and receive an instant risk assessment with confidence probability.

---

## 🛠️ Tech Stack

```
├── Language          Python 3.x
├── ML Framework      Scikit-Learn — Gradient Boosting Classifier
├── Data Processing   Pandas · NumPy
├── Web Framework     Streamlit
├── Model Persistence Joblib
└── Notebook          Jupyter (EDA + Training Pipeline)
```

---

## 📁 Project Structure

```
cardio-risk-predictor/
│
├── app.py                          # Streamlit frontend & prediction logic
├── model.ipynb                     # EDA, feature engineering & model training
├── best_cardio_model_final.joblib  # Pre-trained production model
├── requirements.txt                # Python dependencies
├── cardio_train.csv                # Raw training dataset
└── README.md                       # Project documentation
```

---

## ⚙️ Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/cardio-risk-predictor.git
cd cardio-risk-predictor
```

### 2. Create a Virtual Environment (Recommended)

```bash
python -m venv venv
source venv/bin/activate        # macOS/Linux
venv\Scripts\activate           # Windows
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Application

```bash
streamlit run app.py
```

The app will open automatically at `http://localhost:8501`.

---

## 🧠 Model Architecture

### Input Features (14 Total)

| Category | Features |
|---|---|
| **Demographics** | Age, Gender, Height, Weight |
| **Vitals** | Systolic BP, Diastolic BP |
| **Lab Results** | Cholesterol Level, Glucose Level |
| **Lifestyle** | Smoking, Alcohol Intake, Physical Activity |
| **Engineered** | BMI (derived), Pulse Pressure (derived) |

### Feature Engineering

Two features are automatically computed from raw inputs to improve model sensitivity:

```python
BMI            = weight (kg) / (height (m)) ** 2
Pulse Pressure = Systolic BP - Diastolic BP
```

### Model Pipeline

```
Raw Patient Input
      │
      ▼
Feature Engineering (BMI, Pulse Pressure)
      │
      ▼
Gradient Boosting Classifier
      │
      ▼
Risk Probability Score  →  Low Risk / High Risk
```

---

## 📊 Dataset

The model is trained on the [Cardiovascular Disease Dataset](https://www.kaggle.com/datasets/sulianova/cardiovascular-disease-dataset) — a clinical dataset containing **70,000 patient records** with 11 features and a binary CVD target label.

| Attribute | Details |
|---|---|
| Records | 70,000 patients |
| Target | Presence/Absence of CVD (`0` / `1`) |
| Balance | ~50/50 class distribution |
| Source | Kaggle / Open Clinical Data |

---

## 🚀 Usage Guide

1. **Launch the app** using the live link or locally via `streamlit run app.py`
2. **Enter patient details** — age, gender, height, weight, BP readings, and lab results
3. **Toggle lifestyle flags** — smoking, alcohol, and physical activity status
4. **Click "Predict"** to get instant risk classification and probability score
5. **Interpret the result** — green for Low Risk, red for High Risk, with a confidence percentage

---

## 📋 Requirements

```text
streamlit
scikit-learn
pandas
numpy
joblib
```

Install all at once:

```bash
pip install -r requirements.txt
```

---

## 🔬 Model Performance

> Detailed evaluation metrics are available in `model.ipynb`.

The Gradient Boosting Classifier was selected after benchmarking multiple algorithms including Logistic Regression, Random Forest, and XGBoost. It was optimized via cross-validation and hyperparameter tuning for best F1-score and AUC-ROC on the held-out test set.

---

## ⚠️ Disclaimer

> This application is intended for **educational and research purposes only**. It is **not a substitute for professional medical advice, diagnosis, or treatment**. Always consult a qualified healthcare provider for clinical decisions.

---

## 👤 Author

<table>
  <tr>
    <td align="center">
      <strong>Rabi Shaw</strong><br/>
      ML Engineer & Data Scientist<br/><br/>
      <a href="https://www.linkedin.com/in/rabishaw07/">LinkedIn</a> ·
      <a href="mailto:rshaw86309@gmail.com">Email</a> ·
    </td>
  </tr>
</table>

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve the model, add new features, or fix issues:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

Made with ❤️ by [Rabi Shaw](https://www.linkedin.com/in/rabishaw07/)

⭐ If you found this project helpful, please give it a star!

</div>
