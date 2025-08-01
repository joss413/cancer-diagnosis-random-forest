# 🧬 Cancer Diagnosis Prediction (Decision Tree & Random Forest Classifiers)
This project applies machine learning techniques to predict the presence of cancer based on medical and lifestyle data. 
It compares Decision Tree and Random Forest classifiers and explores hyperparameter tuning to enhance predictive performance.

## 📊 Dataset Overview

🔹 Features

age        genetic_risk     diagnosis
gender     physical_activity
bmi       alcohol_intake
smoking   cancer_history


## 🚀 Project Workflow

1. Data Preprocessing
- Loaded dataset using pandas
- Verified dataset shape and structure
- Checked for missing values
- Selected relevant features and target
- Split dataset (75% training, 25% testing)

2. Modeling
   
🌳 Decision Tree Classifier
- Model: DecisionTreeClassifier() (default)
- Accuracy: 0.86
- Notes: Balanced but tends to overfit on smaller datasets

🌲 Random Forest Classifier (Default)
- Model: RandomForestClassifier(n_estimators=25)
- Accuracy: 0.91
- Notes: Better generalization and improved F1-score

⚙️ Random Forest (Custom Parameters)

RandomForestClassifier(
    criterion='entropy',
    max_depth=15,
    min_samples_split=5,
    min_samples_leaf=3,
    max_features='log2',
    bootstrap=False,
    n_estimators=50
)

📈 Model Evaluation

## 📈 Model Evaluation

| Model                     | Accuracy | Precision | Recall | F1-Score |
|---------------------------|----------|-----------|--------|----------|
| Decision Tree (Default)   | 0.86     | 0.86      | 0.86   | 0.86     |
| Random Forest (Default)   | 0.91     | 0.91      | 0.90   | 0.91     |
| Random Forest (Custom)    | 0.94     | 0.94      | 0.93   | 0.94     |

✅ **Best Model:** Random Forest with custom parameters



## ⚙️ Installation

1. Clone the repo:

```bash
git clone https://github.com/yourusername/cancer-diagnosis-random-forest
cd cancer-diagnosis-random-forest
```
2. **Install dependencies:**:   
```commandline
pip install -r requirements.txt
```

📂 Files in This Repo

- cancer_decision_tree.ipynb: Full notebook with EDA, preprocessing, modeling, and evaluation.
- requirements.txt: List of required Python packages.
- README.md: Project overview and documentation

👨‍💻 Author

Yoseph Negash

📧 yosephn22@gmail.com

📅 2025
