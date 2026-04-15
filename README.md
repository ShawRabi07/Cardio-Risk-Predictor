
# 🩺 Cardio Risk Predictor
**A Machine Learning Approach to Cardiovascular Disease Assessment**

[![Live App](https://img.shields.io/badge/Streamlit-Live%20App-FF4B4B?style=for-the-badge&logo=Streamlit)]([Your Live Link])
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Profile-0077B5?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/rabi-shaw-6a4223297/)

Cardio Risk Predictor is a professional-grade health analytics application designed to assess the probability of cardiovascular disease (CVD). Utilizing a high-performance **Gradient Boosting** machine learning model, the app processes 14 clinical features—including patient vitals, lifestyle factors, and derived medical metrics—to provide real-time risk classification.

---

## 👤 Author
* **Name:** Rabi Shaw  
* **Email:** [Your Email Address]  
* **LinkedIn:** [https://www.linkedin.com/in/rabi-shaw-6a4223297/](https://www.linkedin.com/in/rabi-shaw-6a4223297/)
* **Portfolio/Live Project:** [[Your Live Link]]

---

## 🚀 Key Features
- **Instant Risk Scoring:** Real-time probability estimation and risk categorization (Low vs. High Risk).
- **Clinical Feature Engineering:** Automatically derives **Body Mass Index (BMI)** and **Pulse Pressure** to enhance prediction sensitivity.
- **Interactive UI:** A clean, intuitive dashboard built with Streamlit for seamless data entry and visualization.
- **Explainable Insights:** Transparent input handling for medical metrics like Systolic/Diastolic BP and Cholesterol levels.

## 🛠️ Tech Stack
* **Language:** Python 3.x
* **ML Framework:** Scikit-Learn (Gradient Boosting Classifier)
* **Data Handling:** Pandas, NumPy
* **Deployment:** Streamlit
* **Model Persistence:** Joblib

## 📂 Project Structure
```text
├── app.py                   # Streamlit Frontend & Logic
├── model.ipynb              # EDA, Feature Engineering & Model Training
├── best_cardio_model_final.joblib  # Pre-trained Production Model
├── requirements.txt         # Dependency List
└── cardio_train.csv         # Raw Dataset for Training
