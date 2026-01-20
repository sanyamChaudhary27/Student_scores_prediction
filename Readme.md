# 📝 **README.md**

# Kaggle Competition — Predicting Student Test Scores

This repository contains my solution for the **Predicting Student Test Scores** hosted on Kaggle.  
My latest submission achieved a **score of 8.8520** on the public leaderboard.

---

## 📂 Project Structure

```

├── data/                # raw and/or processed data (not included)
├── notebooks/
│   └── student_scores.ipynb   # main notebook used for training & submission
├── submissions/
│   └── submission.csv    # final submission file for Kaggle
└── README.md

````

> *Note: Dataset is not included due to Kaggle terms — please download directly from Kaggle.*

---

## 🧠 Problem Description

The objective of the competition is to **predict students' exam scores** using various features such as study hours, class attendance, sleep hours, and other demographic and behavioral data. The performance is evaluated on a hidden test set using the RMSE metric.

---

## 🚀 Approach

### **1. Data Loading & Exploration**
- Imported dataset
- Performed basic EDA
- Checked missing values and data distribution

### **2. Preprocessing**
- Handled missing data
- Feature encoding using OneHotEncoder and custom LabelEncoder
- Train-test splits for validation

### **3. Feature Engineering**
- Created interaction features such as `study_sleep_interaction`, `study_attendance_interaction`, and others
- Binned age into groups and created categorical interactions

### **4. Modeling**
- Used **Random Forest Regressor**
- Performed hyperparameter tuning for `max_samples`, `min_samples_split`, `min_samples_leaf`, `max_depth`, and `max_features`
- Selected the best parameters based on RMSE scores

### **5. Evaluation**
- Metric used by Kaggle: **RMSE**
- Final public leaderboard score: **8.8520**

---

## 📈 Results

| Submission |    Score    |         Notes        |
|------------|-------------|----------------------|
| **v1**     | **8.96873** | basic training       |
| **v2**     | **8.85230** | feature improvements |

---

## 📊 Visualization

The notebook includes visualizations for:
- Dataset analysis
- Correlations between features
- Feature importance using horizontal bar charts
- Model performance metrics

---

## 🏗 Future Improvements

Some potential enhancements:

- Further hyperparameter tuning
- Model stacking/ensembling
- Additional feature engineering
- Better validation techniques

---

## 🧾 Requirements

Install dependencies via:

```bash
pip install -r requirements.txt
````

Required libraries include:

```
numpy
pandas
scikit-learn
matplotlib
seaborn
```

---

## 📦 Reproducing Submission

1. Clone the repository:

```bash
git clone https://github.com/[your-username]/[repo-name].git
cd [repo-name]
```

2. Download dataset from Kaggle and place into `/data`

3. Run the notebook:

```bash
jupyter notebook notebooks/student_scores.ipynb
```

4. Generate `submission.csv`

---

## 🏅 Competition Link

Find the competition here:
[https://www.kaggle.com/competitions/[competition-slug](https://www.kaggle.com/competitions/[competition-slug)]

---

## 👤 Author

**Name:** Sanyam  
**Interests:** Machine Learning, AI, DSA  
**Kaggle Profile:** [https://www.kaggle.com/[your-profile](https://www.kaggle.com/[your-profile)]

---

## 📜 License

This project is licensed under the MIT License — see `LICENSE` for details.
