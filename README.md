# ❤️ Heart Disease Prediction

This project predicts the risk of **heart disease** using a **machine learning model (Random Forest with probability calibration)**.  
The model classifies patients into **Low**, **Borderline**, or **High** risk categories, along with the predicted probability.

---

## 🚀 Features
- ✅ Trained on heart disease dataset (clinical features like age, cholesterol, blood pressure, etc.)  
- ✅ Uses **CalibratedClassifierCV (sigmoid)** to improve probability reliability  
- ✅ Interactive **Gradio app** for easy testing in Colab or locally  
- ✅ Threshold-based interpretation:
  - **Low risk** → Probability < 0.45  
  - **Borderline risk** → 0.45 ≤ Probability ≤ 0.75  
  - **High risk** → Probability > 0.75  

---

## 📂 Project Structure
- `Heart_Project.ipynb` → Notebook (data preprocessing, training, evaluation)  
- `final_model.pkl` → Saved calibrated model (ready to use)  
- `app.py` → (Optional) Streamlit web app for deployment  
- `requirements.txt` → Dependencies for running the project  
- `README.md` → Project documentation  

---

## ⚙️ Installation & Usage

### 🔹 Run in Google Colab
1. Upload the notebook (`Heart_Project.ipynb`) and `final_model.pkl`.  
2. Install dependencies:
   ```bash
   !pip install -r requirements.txt
