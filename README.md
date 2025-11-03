# password-strength-inspector
# 🔐 Password Strength NLP

A Natural Language Processing (NLP) and Machine Learning project that classifies passwords as **Weak**, **Moderate**, or **Strong** using character-level and statistical text features.

---

## 1️ Project Overview
This project identifies password strength through feature analysis of textual patterns.  
By applying NLP-inspired techniques, the model evaluates each password based on its length, digits, uppercase/lowercase balance, and special characters to predict its security level.

**Objectives:**
- Extract linguistic and structural features from passwords.  
- Train ML models to classify password strength.  
- Visualize key patterns and predictive insights.

---

## 2️ Dataset Description
**File:** `password_data.sqlite`

| Column | Description |
|---------|-------------|
| `password` | Password text |
| `strength` | Label — 0 = Weak   1 = Moderate   2 = Strong |

**Source:** Provided dataset for academic use  
**Size:** Several thousand labeled passwords

---

## 3️ Methodology
1. **Data Loading** — Read dataset from SQLite into Pandas DataFrame  
2. **Data Cleaning** — Remove duplicates or blanks  
3. **Feature Engineering** — Extract:
   - Password length  
   - Digit count  
   - Upper/lowercase ratio  
   - Special character frequency  
4. **EDA** — Examine feature distributions and correlations  
5. **Model Training** — Apply Logistic Regression   
6. **Evaluation** — Compute accuracy and confusion matrix  
7. **Visualization** — Display class balance and feature importance  

---

## 4️ Tech Stack / Libraries

| Category | Tools |
|-----------|-------|
| Language | Python 3.10+ |
| Data Handling | Pandas · NumPy |
| Machine Learning | Scikit-learn |
| Visualization | Matplotlib · Seaborn |
| Storage | SQLite3 |

---

## 5️ Results & Insights
**Model Accuracy:** ≈ 85 – 90 % 

**Observations**
- Password length and diversity of characters have the highest impact.  
- Short or single-type passwords are predominantly weak.  
- Balanced feature engineering improves prediction reliability.

**Outputs**
- Confusion Matrix  
- Strength Distribution Graph  
- Feature Importance Plot  

---

## 6️ Future Enhancements
- Add Deep Learning models (LSTM / Transformer).  
- Build a Web App for real-time strength checking.  
- Use larger, more diverse datasets.  
- Implement model interpretability (SHAP / LIME).

---


