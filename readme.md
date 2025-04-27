# 🫀 Heart Disease Predictor

Predict the likelihood of heart disease based on patient medical data using machine learning models.

---

## 📚 Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Features](#features)
- [EDA and Preprocessing](#eda-and-preprocessing)
- [Modeling](#modeling)
- [Evaluation Metrics](#evaluation-metrics)
- [Results](#results)
- [Usage](#usage)
- [Dependencies](#dependencies)
- [License](#license)

---

## 🧩 Project Overview

Heart disease is one of the world's leading causes of death.  
This project applies machine learning algorithms to clinical features in order to predict whether an individual has heart disease.

---

## 📈 Dataset

The dataset used is the [UCI Heart Disease Dataset](https://archive.ics.uci.edu/ml/datasets/heart+Disease).

- **Number of samples**: 303
- **Target**: `target` (1 = heart disease present, 0 = no heart disease)

---

## 🧪 Features

| Feature    | Description                                           |
| :--------- | :---------------------------------------------------- |
| `age`      | Age in years                                          |
| `sex`      | Gender (1 = male, 0 = female)                         |
| `cp`       | Chest pain type (0-3)                                 |
| `trestbps` | Resting blood pressure (mm Hg)                        |
| `chol`     | Serum cholesterol (mg/dl)                             |
| `fbs`      | Fasting blood sugar > 120 mg/dl (1 = true, 0 = false) |
| `restecg`  | Resting electrocardiographic results (0-2)            |
| `thalach`  | Maximum heart rate achieved                           |
| `exang`    | Exercise-induced angina (1 = yes, 0 = no)             |
| `oldpeak`  | ST depression induced by exercise relative to rest    |
| `slope`    | Slope of the peak exercise ST segment                 |
| `ca`       | Number of major vessels colored by fluoroscopy        |
| `thal`     | 3 = normal; 6 = fixed defect; 7 = reversible defect   |
| `target`   | Heart disease diagnosis (1 = disease, 0 = no disease) |

---

## 🔍 EDA and Preprocessing

- **Data Cleaning**: No missing values detected.
- **Exploratory Data Analysis (EDA)**:
  - Heatmaps to visualize feature correlations
  - Pairplots for initial patterns
- **Preprocessing Steps**:
  - Label encoding for categorical variables
  - Feature scaling with `StandardScaler`
  - Data splitting into training and test sets (80/20 split)

---

## 🤖 Modeling

The following machine learning models were trained and evaluated:

- **Logistic Regression**
- **K-Nearest Neighbors (KNN)**
- **Decision Tree Classifier**
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**
- **XGBoost Classifier**

**Additional Techniques:**

- Hyperparameter Tuning:
  - GridSearchCV
  - KNN optimization with best `k` search
- Cross-Validation for robust model evaluation

---

## 📊 Evaluation Metrics

Each model was evaluated using:

- **Accuracy Score**
- **Confusion Matrix**
- **Classification Report** (Precision, Recall, F1-score)

---

## 🏆 Results

| Model               | Accuracy |
| :------------------ | :------- |
| Logistic Regression | ~85%     |
| K-Nearest Neighbors | ~84%     |
| Decision Tree       | ~79%     |
| Random Forest       | ~87%     |
| SVM                 | ~82%     |
| XGBoost             | ~88%     |

✅ **XGBoost Classifier achieved the best performance overall**.

---

## ⚙️ Usage

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/heart-disease-predictor.git
cd heart-disease-predictor
```

### 2. Create and Activate a Virtual Environment

```bash
# Create a virtual environment
python -m venv venv

# Activate the virtual environment
# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Run the Notebook(in Jupyter or your IDE)

```
Heart_Disease_Predictor.ipynb
```
