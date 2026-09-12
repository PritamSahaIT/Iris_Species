Iris Species Classification

A beginner-friendly machine learning project that explores the classic Iris dataset and trains a Random Forest classifier to predict flower species from sepal and petal measurements.

📖 Overview

This project is split into two notebooks:

EDA_and_data_clean.ipynb 🔍 — Exploratory data analysis and data cleaning checks on the Iris dataset (previewing the data, checking data types, summary statistics, missing values, and duplicates).
ModelTrain.ipynb 🤖 — Trains a RandomForestClassifier on the training data and evaluates its accuracy on a separate test set.
📊 Dataset

The project uses two CSV files (not included in this repo — add your own or download the Iris dataset):

File	Purpose
Iris_try.csv	Training data
Iris_test.csv	Test data used for evaluating the trained model

Each row contains the following columns:

Id
SepalLengthCm
SepalWidthCm
PetalLengthCm
PetalWidthCm
Species 🌷 (target — one of Iris-setosa, Iris-versicolor, Iris-virginica)
🗂️ Project Structure
.
├── EDA_and_data_clean.ipynb   # Exploratory data analysis & cleaning checks
├── ModelTrain.ipynb           # Model training & evaluation
├── Iris_try.csv               # Training data (add your own)
├── Iris_test.csv              # Test data (add your own)
└── README.md
⚙️ Requirements
🐍 Python 3.x
🐼 pandas
🔬 scikit-learn

Install dependencies with:

bash
pip install pandas scikit-learn
🚀 Usage
📥 Place Iris_try.csv and Iris_test.csv in the project directory.
🔍 Run EDA_and_data_clean.ipynb to explore and validate the training data.
🏋️ Run ModelTrain.ipynb to train the Random Forest model and see its accuracy on the test set.
📈 Results

The Random Forest classifier is trained on all four numeric features (sepal length/width, petal length/width) and evaluated by comparing predictions against the actual species labels in the test set, reporting overall accuracy as a percentage ✅.

📜 License

Feel free to use this project for learning purposes. 🎓
