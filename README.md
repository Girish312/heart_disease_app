# 🫀 Heart Disease Detection using Machine Learning

## 📘 Project Overview
Heart disease is one of the leading causes of death worldwide. Early detection can save lives by enabling timely intervention.  
This project applies **Supervised Learning Classification Algorithms** to predict whether a patient is likely to have heart disease based on clinical data.

---

## 🎯 Objectives
- Build and compare multiple classification models (Logistic Regression, Random Forest, SVM).  
- Identify the most accurate and reliable model.  
- Deploy a user-friendly web interface using **Streamlit** for real-time predictions.

---

## 🧠 Machine Learning Models Used
| Model | Description |
|--------|--------------|
| **Logistic Regression** | A linear model for binary classification. |
| **Random Forest Classifier** | An ensemble of decision trees to improve accuracy. |
| **Support Vector Machine (SVM)** | Maximizes the margin between classes for robust classification. |

---

## 🧩 Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Joblib  
- **Frontend:** Streamlit  
- **Backend:** Custom Python utilities (model loading + prediction)  
- **Deployment (optional):** FastAPI + Docker  

---

## 📂 Folder Structure
heart_disease_app/
├── frontend/
│   ├── app.py
├── backend/
│   ├── model_utils.py
├── model/
│   ├── heart_model.pkl
└── requirements.txt


---

## ⚙️ Installation & Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/heart_disease_app.git
   cd heart_disease_app

2. Install dependencies:
   ```bash
   pip install -r requirements.txt


3. Run the Streamlit app:
   ```bash
   streamlit run frontend/app.py

---

🧪 Model Training (Colab)

The model was trained using:

- Dataset: heart_disease_dataset.csv

- Split: 80% Training, 20% Testing

- Evaluation Metrics: Precision, Recall, F1-Score, ROC-AUC

- Best Model: Random Forest Classifier

- The final model is saved as: model/heart_model.pkl

---

🌐 Deployment

To containerize with Docker:
```
docker build -t heart_disease_app .

docker run -p 8501:8501 heart_disease_app
```
---

🧾 Results Summary

| Metric    | Best Model (Random Forest) |
| --------- | -------------------------- |
| Accuracy  | ~0.87                      |
| Recall    | ~0.85                      |
| Precision | ~0.88                      |
| F1-score  | ~0.86                      |
| ROC-AUC   | ~0.91                      |
