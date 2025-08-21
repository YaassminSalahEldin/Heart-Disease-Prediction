# ❤️ Heart Disease Prediction

## 📖 Introduction
Heart disease is one of the leading causes of death globally.  
This project aims to use machine learning to **predict the risk of heart disease** based on medical parameters like age, cholesterol, and blood pressure.  

The model is deployed using **Gradio** and **Streamlit**, so users can interact with it easily.

---

## 📊 Dataset
- Source: [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease)  
- Features: 13 input variables (Age, Sex, Chest Pain Type, Resting Blood Pressure, Cholesterol, etc.)  
- Target: 0 = No disease, 1 = Disease  

---

## 🧠 Model
- Base model: **Random Forest Classifier**  
- Calibrated using: **CalibratedClassifierCV (sigmoid method)**  
- Custom thresholds:
  - ✅ Low risk: Probability ≤ 0.6  
  - ⚠️ Borderline risk: 0.6 < Probability ≤ 0.75  
  - 🚨 High risk: Probability > 0.75  

---

## 🚀 Deployment
- **Gradio Interface** (for Colab)  
- **Streamlit App** (for web deployment)  

---

## 📂 Files
- `Heart_Project.ipynb` → Notebook for training & evaluation  
- `final_model.pkl` → Pre-trained model  
- `app.py` → Streamlit web app  
- `requirements.txt` → Dependencies  

---

## 🧪 Example Predictions

| Features (Age, Sex, CP, ...)                            | Prediction |
|----------------------------------------------------------|------------|
| [45, 0, 0, 120, 240, 0, 1, 170, 0, 0.5, 2, 0, 2]         | ✅ Low risk (0.52) |
| [52, 1, 1, 135, 210, 0, 0, 160, 0, 1.0, 1, 0, 2]         | ⚠️ Borderline risk (0.68) |
| [57, 1, 2, 145, 260, 0, 1, 140, 0, 1.5, 1, 1, 2]         | 🚨 High risk (0.83) |

---

## ⚠️ Disclaimer
This project is intended for **educational purposes only**.  
It should not be used as a substitute for professional medical diagnosis.
