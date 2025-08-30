# 🧠 Predict the Introverts from the Extroverts  
**Kaggle Playground Series – Season 5, Episode 7 (S5E7)**  

This project tackles the Kaggle competition [“Predict the Introverts from the Extroverts”](https://www.kaggle.com/competitions/playground-series-s5e7/overview), where the goal is to classify individuals as either **introverts** or **extroverts** based on behavioral features.  

---

## 📌 Project Overview  

- 🎯 **Competition:** Playground Series – Season 5, Episode 7  
- 🔍 **Objective:** Binary classification – introvert vs. extrovert  
- 📏 **Evaluation Metric:** Accuracy Score  
- 🛠 **Techniques Used:**  
  - Data preprocessing & feature engineering  
  - Label encoding / labeling  
  - Random Forest Classifier  

---

## 📂 Project Structure  

```

├── data/
│   ├── train.csv              # Training dataset from Kaggle
│   ├── test.csv               # Test dataset from Kaggle
│   └── sample\_submission.csv  # Sample submission template
├── notebooks/
│   └── Untitled.ipynb         # Notebook: EDA, preprocessing, modeling
├── requirements.txt           # Project dependencies
├── sub.csv                    # Kaggle submission file
└── README.md                  # Project documentation

````

---

## 🧹 Data Preprocessing  

1. 📥 Loaded datasets from Kaggle.  
2. 📊 Conducted Exploratory Data Analysis (EDA) – distributions, correlations, missing values.  
3. 🔡 Applied **label encoding** to categorical features.  
4. ⚖️ Normalized & transformed selected features.  
5. 🏷 Prepared target labels (`introvert` vs. `extrovert`).  

---

## 🌲 Modeling Strategy  

- **Model:** Random Forest Classifier 🌳  
- **Training Steps:**  
  - Train/validation split for model evaluation.  
  - Hyperparameter tuning (number of estimators, depth, etc.).  
  - Final training on full dataset.  
- **Evaluation:** Accuracy on validation + Kaggle public leaderboard submission.  

✅ 96.86% !  


---

## ⚡ Usage  

Clone the repo and set up dependencies:  

```bash
git clone https://github.com/yourusername/introverts-vs-extroverts.git
cd introverts-vs-extroverts

# Create virtual environment
python -m venv venv
source venv/bin/activate      # macOS/Linux
venv\Scripts\activate         # Windows

# Install dependencies
pip install -r requirements.txt
````

Run the notebook:

```bash
jupyter notebook notebooks/Untitled.ipynb
```

If you saved your model:

```python
import joblib
model = joblib.load("models/rf_model.pkl")
preds = model.predict(new_data)
```

---

## 🚀 Future Improvements

* 🔬 Try advanced models (XGBoost, LightGBM, Stacking).
* 🔧 More feature engineering (interactions, polynomial features).
* 🤖 Build a full Kaggle pipeline for automated submissions.

---

## 📚 References

* 📌 [Kaggle Competition Page](https://www.kaggle.com/competitions/playground-series-s5e7/overview)
* 📂 [Kaggle Dataset](https://www.kaggle.com/competitions/playground-series-s5e7/data)
* 📝 [Evaluation Metric – Accuracy](https://www.kaggle.com/competitions/playground-series-s5e7/overview)

---

✨ *Made with passion for Machine Learning & Kaggle challenges!* ✨

```
