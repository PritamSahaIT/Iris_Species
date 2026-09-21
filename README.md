# 🌸 Iris Flower Classification & Exploratory Data Analysis

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![Scikit-Learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white)](https://scikit-learn.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)


An end-to-end Machine Learning project demonstrating Exploratory Data Analysis (EDA), data cleaning, and multi-class classification on the classic **Iris Dataset** using a **Random Forest Classifier**.

---

## 📌 Project Overview

The goal of this project is to accurately classify Iris flowers into one of three species (*Iris setosa*, *Iris versicolor*, and *Iris virginica*) based on morphological measurements of their sepals and petals.

### 🎯 Key Highlights
- **Exploratory Data Analysis (EDA):** Statistical summaries, inspection of data distributions, null value identification, and duplicate checks.
- **Data Preprocessing & Cleaning:** Feature-target separation and dataset validation.
- **Machine Learning Modeling:** Supervised classification implemented with an ensemble **Random Forest Classifier**.
- **Model Evaluation:** Out-of-sample evaluation on an independent test dataset (`Iris_test.csv`) to assess predictive performance and accuracy.

---

## 📂 Project Structure

```text
Iris Project/
│
├── EDA_and_data_clean.ipynb   # Jupyter Notebook for EDA, data inspection & cleaning
├── ModelTrain.ipynb           # Jupyter Notebook for training & evaluating the Random Forest model
├── Iris_try.csv               # Primary training dataset
├── Iris_test.csv              # Holdout test dataset for model evaluation
├── database.sqlite            # SQLite database containing dataset records
└── README.md                  # Project documentation
```

---

## 📊 Dataset Description

The dataset consists of measurements across 4 features for 3 distinct species of Iris flowers:

| Feature | Description | Type |
| :--- | :--- | :--- |
| `SepalLengthCm` | Length of the sepal in centimeters | Float (Continuous) |
| `SepalWidthCm` | Width of the sepal in centimeters | Float (Continuous) |
| `PetalLengthCm` | Length of the petal in centimeters | Float (Continuous) |
| `PetalWidthCm` | Width of the petal in centimeters | Float (Continuous) |
| **`Species`** *(Target)* | `Iris-setosa`, `Iris-versicolor`, `Iris-virginica` | Categorical |

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/iris-flower-classification.git
cd iris-flower-classification
```

### 2. Create a Virtual Environment (Optional but Recommended)
```bash
# Using venv
python -m venv venv

# Activate on Windows:
venv\Scripts\activate

# Activate on macOS/Linux:
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install pandas numpy scikit-learn jupyter
```

### 4. Launch Jupyter Notebook
```bash
jupyter notebook
```

---

## 🔬 Methodology & Workflow

### 1. Exploratory Data Analysis (`EDA_and_data_clean.ipynb`)
- **Structure Inspection:** `head()`, `tail()`, and `info()` checks to understand column types and entry counts.
- **Summary Statistics:** `describe()` to analyze central tendency, dispersion, and quartiles.
- **Integrity Validation:** Checked for missing values (`isnull().sum()`) and duplicate records (`duplicated().sum()`).

### 2. Model Training & Evaluation (`ModelTrain.ipynb`)
- **Feature Extraction:** Splitting feature matrix ($X$) and target vector ($y$).
- **Model Training:** Initializing and fitting a `RandomForestClassifier` on the training dataset.
- **Inference & Testing:** Making predictions on the unseen test set (`Iris_test.csv`).
- **Accuracy Evaluation:** Comparing predicted classes against ground truth labels.

```python
from sklearn.ensemble import RandomForestClassifier

# Initialize and train
model = RandomForestClassifier(random_state=42)
model.fit(x, y)

# Predict on unseen test set
predictions = model.predict(x_test.values)
```

---

## 📈 Results

- **Model:** Random Forest Classifier
- **Task:** Multi-class Classification (3 Classes)
- **Accuracy:** Reached high classification accuracy on the holdout test set with clean separation between *Iris-setosa*, *Iris-versicolor*, and *Iris-virginica*.

---

## 🛠️ Tech Stack

- **Language:** Python 3.x
- **Libraries:**
  - `pandas` - Data manipulation & analysis
  - `scikit-learn` - Machine learning & evaluation
  - `sqlite3` - Database exploration
  - `Jupyter Notebook` - Interactive development environment

---


