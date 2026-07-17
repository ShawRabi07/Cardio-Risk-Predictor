<div align="center">

# ❤️ AI-Based Heart Disease Risk Prediction

### Machine Learning-Powered Heart Disease Risk Assessment

[![Streamlit App](https://img.shields.io/badge/Streamlit-Live%20Demo-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white)](https://cardiovas.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML%20Framework-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rabi%20Shaw-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rabi-shaw-6a4223297/)

<br/>

> An AI-powered machine learning application that predicts heart disease risk in real time using 14 clinical and lifestyle features, powered by a high-performance Gradient Boosting Classifier.

<br/>

![banner](https://img.shields.io/badge/Accuracy-High%20Performance%20Model-success?style=flat-square)
![status](https://img.shields.io/badge/Status-Production%20Ready-brightgreen?style=flat-square)
![license](https://img.shields.io/badge/License-MIT-blue?style=flat-square)

</div>

---

# 📌 Overview

**AI-Based Heart Disease Risk Prediction** is a machine learning-powered Streamlit web application that predicts the likelihood of heart disease using a trained **Gradient Boosting Classifier**. The application accepts patient demographics, vital signs, laboratory results, and lifestyle information, automatically computes **BMI** and **Pulse Pressure**, and generates a real-time probability score with a corresponding **Low Risk** or **High Risk** classification.

Designed with an intuitive user interface, the application enables fast and reliable heart disease risk assessment, making it suitable for educational, research, and machine learning demonstration purposes.

---

# ✨ Key Features

| Feature | Description |
|---------|-------------|
| ⚡ **Real-Time Prediction** | Instantly predicts heart disease risk with confidence probability |
| 🧮 **Automatic Feature Engineering** | Computes BMI and Pulse Pressure automatically |
| 🤖 **Machine Learning Model** | Uses a trained Gradient Boosting Classifier |
| 📊 **Interactive Dashboard** | Clean and responsive Streamlit interface |
| 🎯 **Binary Classification** | Predicts Low Risk or High Risk |
| 🔍 **Clinical Inputs** | Uses demographics, vitals, lab values, and lifestyle factors |
| 💾 **Pre-trained Model** | Loads a saved `.joblib` model without retraining |

---

# 🖥️ Live Demo

### 🔗 https://cardiovas.streamlit.app/

Try the application by entering patient details and receive an instant heart disease risk prediction with probability.

---

# 🛠️ Tech Stack

```
Language           : Python 3.x
Machine Learning   : Scikit-Learn
Model              : Gradient Boosting Classifier
Web Framework      : Streamlit
Data Processing    : Pandas, NumPy
Model Persistence  : Joblib
Development        : Jupyter Notebook
```

---

# 📁 Project Structure

```
AI-Based-Heart-Disease-Risk-Prediction/
│
├── app.py
├── model.ipynb
├── best_cardio_model_final.joblib
├── cardio_train.csv
├── requirements.txt
├── README.md
└── assets/
```

---

# ⚙️ Installation

## 1. Clone the Repository

```bash
git clone https://github.com/your-username/AI-Based-Heart-Disease-Risk-Prediction.git

cd AI-Based-Heart-Disease-Risk-Prediction
```

---

## 2. Create Virtual Environment (Optional)

### Windows

```bash
python -m venv venv

venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv

source venv/bin/activate
```

---

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 4. Run the Application

```bash
streamlit run app.py
```

The application will launch at

```
http://localhost:8501
```

---

# 🧠 Model Architecture

## Input Features (14)

### Demographics

- Age
- Gender
- Height
- Weight

### Vital Signs

- Systolic Blood Pressure
- Diastolic Blood Pressure

### Laboratory Measurements

- Cholesterol
- Glucose

### Lifestyle Factors

- Smoking
- Alcohol Intake
- Physical Activity

### Engineered Features

- BMI
- Pulse Pressure

---

## Feature Engineering

The application automatically computes two additional medical indicators before prediction.

```python
BMI = Weight (kg) / Height² (m²)

Pulse Pressure = Systolic BP - Diastolic BP
```

---

## Prediction Pipeline

```
Patient Information
        │
        ▼
Data Validation
        │
        ▼
Feature Engineering
(BMI + Pulse Pressure)
        │
        ▼
Gradient Boosting Classifier
        │
        ▼
Prediction Probability
        │
        ▼
Low Risk / High Risk
```

---

# 📊 Dataset

The model was trained using a publicly available cardiovascular clinical dataset containing approximately **70,000 patient records** with demographic information, vital signs, laboratory measurements, lifestyle habits, and disease labels.

### Dataset Summary

| Attribute | Value |
|------------|-------|
| Records | 70,000 |
| Target | Heart Disease (0 / 1) |
| Features | Clinical & Lifestyle Variables |
| Source | Kaggle Cardiovascular Disease Dataset |

---

# 🚀 How to Use

1. Launch the application.
2. Enter patient information.
3. Provide blood pressure values.
4. Select cholesterol and glucose levels.
5. Specify smoking, alcohol, and physical activity status.
6. Click **Predict**.
7. View the predicted heart disease probability and risk classification.

---

# 📋 Requirements

```
streamlit
pandas
numpy
scikit-learn
joblib
```

Install all dependencies using

```bash
pip install -r requirements.txt
```

---

# 🔬 Machine Learning Model

The prediction model was developed using **Scikit-Learn's Gradient Boosting Classifier**.

The workflow includes:

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Feature Selection
- Model Training
- Hyperparameter Tuning
- Cross Validation
- Model Evaluation
- Model Serialization using Joblib

The Gradient Boosting model was selected after comparing its performance against several algorithms, including:

- Logistic Regression
- Decision Tree
- Random Forest
- K-Nearest Neighbors
- Support Vector Machine
- AdaBoost
- XGBoost

Performance evaluation was carried out using:

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

---

# ⚠️ Disclaimer

> This project is intended solely for educational, research, and machine learning demonstration purposes. It is **not** a medical diagnostic tool and should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult qualified healthcare professionals for medical decisions.

---

# 👨‍💻 Author

**Rabi Shaw**

Machine Learning Engineer | Data Science Enthusiast

- 💼 LinkedIn: https://www.linkedin.com/in/rabishaw07/
- 📧 Email: rshaw86309@gmail.com

---

# 🤝 Contributing

Contributions are welcome!

If you'd like to improve the project:

1. Fork the repository.
2. Create a feature branch.

```bash
git checkout -b feature/new-feature
```

3. Commit your changes.

```bash
git commit -m "Add new feature"
```

4. Push the branch.

```bash
git push origin feature/new-feature
```

5. Open a Pull Request.

---

# 📄 License

This project is licensed under the **MIT License**.

---

<div align="center">

## ⭐ If you found this project useful, consider giving it a star!

Made with ❤️ by **Rabi Shaw**

</div>
