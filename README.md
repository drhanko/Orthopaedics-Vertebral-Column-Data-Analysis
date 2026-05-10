# Orthopaedics Vertebral Column Data Analysis

## 📌 Project Overview

This project analyzes biomechanical features of the vertebral column to classify spinal conditions as **Normal (0)** or **Abnormal (1)** using data analysis and machine learning techniques.

The workflow includes:

* Exploratory Data Analysis (EDA)
* Feature distribution analysis
* Model training using K-Nearest Neighbors (KNN)
* Hyperparameter tuning (K selection)
* Learning curve analysis
* Distance metric comparison

---

## 📊 Dataset

The dataset contains biomechanical measurements of the spine:

* Pelvic incidence
* Pelvic tilt
* Lumbar lordosis angle
* Sacral slope
* Pelvic radius
* Degree of spondylolisthesis

Target:

* **0 = Normal**
* **1 = Abnormal**

---

## 🔍 Exploratory Data Analysis (EDA)

### 🔹 Feature Distribution (Boxplot)

* Abnormal cases generally show **higher median values** across multiple features.
* The abnormal group has **greater variability**, indicating more complex spinal conditions.
* There is **overlap between classes**, explaining why perfect classification is not possible.

### 🔹 Feature Relationships (Scatter Analysis)

* Some feature pairs exhibit **partial separation** between classes.
* No single feature pair can fully distinguish the classes.
* Combining multiple features is necessary for effective classification.

---

## 🤖 Model: K-Nearest Neighbors (KNN)

KNN was used as the primary classification model due to its simplicity and effectiveness for structured data.

---

## ⚙️ Effect of K (Model Complexity)

* **Small K (1–5)**:

  * Very low training error
  * High variance → risk of overfitting

* **Large K (>100)**:

  * Higher bias → underfitting
  * Smoother decision boundary

* **Optimal K = 4**:

  * Best balance between bias and variance
  * Lowest test error observed

---

## 📈 Model Performance

* **Accuracy:** ~94%
* **Precision:** ~93%
* **Recall:** ~98.6%
* **F1-score:** ~95.8%

Confusion Matrix:

* TP: 69
* FN: 1
* TN: 25
* FP: 5

🔹 Insight:

* Very high recall indicates strong ability to detect abnormal cases
* Errors mainly come from false positives rather than false negatives

---

## 📉 Learning Curve Analysis

### 🔹 Effect of K

* Training error decreases as K becomes smaller
* Test error decreases initially, then fluctuates (overfitting at small K)

### 🔹 Effect of Training Size

* **Small dataset (N = 10)**:

  * High and unstable test error (~0.3)
  * Insufficient learning

* **Larger dataset (N = 210)**:

  * Lower and more stable test error
  * Improved generalization

---

## 📏 Distance Metric Comparison

Different distance metrics were evaluated:

### 🔹 Euclidean Distance (L2)

* Best overall performance
* Effective for continuous, scaled features

### 🔹 Manhattan Distance (L1)

* More robust to outliers
* Slightly less sensitive than L2

### 🔹 Chebyshev Distance (L∞)

* Focuses on maximum feature difference
* Performed worse due to overemphasis on single features

---

## 🧠 Key Insights

* Feature distributions differ significantly between classes, but overlap exists
* Model performance is strongly influenced by **K (bias-variance tradeoff)**
* Increasing training data improves stability and generalization
* Distance metric choice impacts model sensitivity
* **Euclidean distance + K = 4 provides the best performance**

---

## 🎯 Conclusion

This project demonstrates that:

* Biomechanical spinal features contain strong signals for classification
* Combining multiple features is essential for accurate prediction
* Proper tuning of K and distance metric is critical in KNN
* Even simple models can achieve high performance with proper analysis

---

## 🛠️ Tech Stack

* Python
* Pandas / NumPy
* Matplotlib / Seaborn
* Scikit-learn

---

## ▶️ How to Run

```bash
git clone https://github.com/drhanko/Orthopaedics-Vertebral-Column-Data-Analysis.git
cd Orthopaedics-Vertebral-Column-Data-Analysis
pip install -r requirements.txt
python main.py
```

---

## 👤 Author

* Wen-Yen(Hank) Hsu
