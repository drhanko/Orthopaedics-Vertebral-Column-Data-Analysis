# Orthopaedics Vertebral Column Data Analysis

## 📌 Project Overview

This project applies data analysis and machine learning techniques to classify spinal conditions based on biomechanical features of the vertebral column.

I independently built an end-to-end data analysis pipeline, including data preprocessing, exploratory data analysis (EDA), model training, and evaluation, to identify patterns that distinguish normal and abnormal spinal conditions.

---

## 🎯 Key Achievements

* Built multiple classification models and achieved up to **XX% accuracy** (fill in your result)
* Identified key biomechanical features (e.g., pelvic incidence, lumbar lordosis) that strongly influence diagnosis
* Improved model performance through feature scaling and model comparison
* Translated raw medical data into actionable insights via visualization

---

## 🧠 What I Did

* Cleaned and preprocessed real-world dataset (handling data consistency & normalization)
* Performed exploratory data analysis to uncover feature relationships and distributions
* Implemented and compared multiple machine learning models:

  * Logistic Regression
  * K-Nearest Neighbors (KNN)
  * Support Vector Machine (SVM)
  * Decision Tree / Random Forest
* Evaluated models using:

  * Accuracy
  * Confusion Matrix
  * Precision / Recall / F1-score
* Visualized data trends and correlations using Matplotlib / Seaborn

---

## 📊 Dataset

The dataset contains biomechanical measurements of the spine, including:

* Pelvic incidence
* Pelvic tilt
* Lumbar lordosis angle
* Sacral slope
* Pelvic radius
* Degree of spondylolisthesis

Target labels:

* Normal
* Abnormal (Hernia / Spondylolisthesis)

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 📈 Results & Insights

* **Best Model:** (e.g., SVM with XX% accuracy)
* **Key Insight:** Certain spinal angles (e.g., pelvic incidence) show strong correlation with abnormal conditions
* **Observation:** Feature scaling significantly improved model performance for distance-based models (e.g., KNN, SVM)

---

## ▶️ How to Run

```bash
git clone https://github.com/drhanko/Orthopaedics-Vertebral-Column-Data-Analysis.git
cd Orthopaedics-Vertebral-Column-Data-Analysis
pip install -r requirements.txt
python main.py
```

---

## 📁 Project Structure

```
├── data/          # dataset
├── notebooks/     # EDA & experiments
├── src/           # core logic / models
├── results/       # outputs / plots
├── main.py
└── README.md
```

---

## 🔍 Future Improvements

* Hyperparameter tuning (GridSearch / RandomSearch)
* Add ensemble models (XGBoost, LightGBM)
* Deploy as an interactive web app (e.g., Streamlit)

---

## 👤 Author

* Your Name

---
