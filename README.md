#  Breast Cancer Classification using Machine Learning

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Status-Complete-brightgreen?style=for-the-badge"/>
</p>

<p align="center">
  A supervised machine learning project that classifies breast cancer tumors as <b>Malignant</b> or <b>Benign</b> using three ML algorithms — trained, evaluated, and compared.
</p>

---

##  Table of Contents

- [Overview](#-overview)
- [Dataset](#-dataset)
- [Project Workflow](#-project-workflow)
- [Exploratory Data Analysis](#-exploratory-data-analysis)
- [Models Used](#-models-used)
- [Results](#-results)
- [Tech Stack](#-tech-stack)
- [How to Run](#-how-to-run)
- [Project Structure](#-project-structure)
- [Author](#-author)

---

##  Overview

This project applies supervised machine learning to the **Breast Cancer Wisconsin Dataset** to predict whether a tumor is **malignant** or **benign**. Three models are trained, evaluated, and compared — Logistic Regression, Random Forest, and Support Vector Machine (SVM).

---

##  Project Workflow

```
Load Dataset ──► EDA ──► Preprocessing ──► Train/Test Split ──► Feature Scaling ──► Model Training ──► Evaluation ──► Comparison
```

| Step | Description |
|:---:|:---|
| 1 | Load dataset from sklearn, convert to DataFrame |
| 2 | Exploratory Data Analysis (EDA) |
| 3 | Null & duplicate check, class balance inspection |
| 4 | 80/20 Train-Test Split (`random_state=42`) |
| 5 | StandardScaler applied to all features |
| 6 | Three models trained and evaluated |
| 7 | Accuracy and classification reports compared |

---

##  Exploratory Data Analysis

| Analysis | Method |
|:---|:---|
| Data Overview | `.head()`, `.info()`, `.describe()` |
| Null Check | `.isna().sum()` |
| Duplicate Check | `.duplicated().sum()` |
| Class Distribution | Value counts, Pie chart, Count plot |
| Outlier Detection | Box plots for all 30 features |
| Feature Correlation | Heatmap (`seaborn`, `coolwarm` palette) |

**Class Distribution:**

| Class | Label | Count | Percentage |
|:---:|:---|:---:|:---:|
| 1 | Benign | 357 | 62.7% |
| 0 | Malignant | 212 | 37.3% |

---

##  Models Used

| Model | Library | Key Parameters |
|:---|:---|:---|
| Logistic Regression | `sklearn.linear_model` | `max_iter=500` |
| Random Forest Classifier | `sklearn.ensemble` | `random_state=42` |
| Support Vector Machine | `sklearn.svm` | Default RBF kernel |

> All models trained on **StandardScaler-normalized** features.

---

##  Results

| Model | Accuracy |
|:---|:---:|
| Logistic Regression | ~97% |
| Random Forest | ~96% |
| **SVM** | **~98%**  |

Each model evaluated using:

-  Accuracy Score
-  Classification Report (Precision, Recall, F1-Score)
-  Confusion Matrix

>  Exact values may vary slightly. Results based on `random_state=42` with 80/20 split.

---

##  Tech Stack

| Tool | Purpose |
|:---|:---|
| Python | Core language |
| Pandas | Data manipulation |
| NumPy | Numerical operations |
| Matplotlib | Visualization |
| Seaborn | Statistical plots |
| Scikit-learn | ML models & evaluation |
| Jupyter Notebook | Development environment |

---

##  How to Run

**1. Clone the repository**

```bash
git clone https://github.com/your-username/breast-cancer-classification.git
cd breast-cancer-classification
```

**2. Install dependencies**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

**3. Launch Jupyter Notebook**

```bash
jupyter notebook breast_cancer_classification.ipynb
```

**4. Run all cells**

`Kernel` → `Restart & Run All`


---

##  Author

**Sadia Noreen**
*Software Engineering Graduate | AI & ML Enthusiast*


---

<p align="center"> If you found this helpful, consider giving it a star!</p>
