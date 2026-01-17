<h1 align="center">📊 Sampling Techniques & Machine Learning</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--Learn-ML-orange?style=for-the-badge&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" />
</p>

<p align="center">
  <i>Analyzing the impact of different sampling techniques on machine learning model performance using an imbalanced credit card fraud dataset.</i>
</p>

---

## 📌 Problem Statement

Given a **highly imbalanced credit card dataset**, the goal is to:
1. Balance the dataset using **SMOTE**
2. Apply **5 different sampling techniques**
3. Evaluate **5 different ML models**
4. Determine which sampling technique works best for each model

---

## 📂 Dataset

| Property | Value |
|----------|-------|
| **Source** | [Credit Card Dataset](https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv) |
| **Rows** | 772 |
| **Features** | 30 |
| **Target** | `Class` (0 = Legit, 1 = Fraud) |
| **Initial Balance** | Highly Imbalanced ⚠️ |

---

## ⚙️ Methodology
```
┌─────────────────────────────────────────────────────────────────┐
│  1. Load Data  →  2. Balance (SMOTE)  →  3. Create 5 Samples    │
│                                                                 │
│  4. Train 5 Models on Each Sample  →  5. Compare Accuracies     │
└─────────────────────────────────────────────────────────────────┘
```

### 🔹 Sampling Techniques

| # | Technique | Description |
|:-:|-----------|-------------|
| 1 | **Simple Random** | Random selection without any criteria |
| 2 | **Stratified** | Maintains class distribution ratio |
| 3 | **Systematic** | Selects every k-th element |
| 4 | **Cluster** | Divides into clusters, samples from selected cluster |
| 5 | **Bootstrap** | Random sampling with replacement |

### 🔹 Machine Learning Models

| # | Model | Type |
|:-:|-------|------|
| M1 | Logistic Regression | Linear |
| M2 | Decision Tree | Tree-based |
| M3 | Random Forest | Ensemble |
| M4 | SVM | Kernel-based |
| M5 | Gradient Boosting | Boosting |

---

## 📊 Results

### Accuracy Table (%)

| Model | Simple Random | Stratified | Systematic | Cluster | Bootstrap |
|:------|:-------------:|:----------:|:----------:|:-------:|:---------:|
| Logistic Regression | 87.07 | 91.38 | 89.66 | 86.96 | **95.69** |
| Decision Tree | 93.97 | 93.97 | **98.28** | 86.96 | 93.10 |
| Random Forest | 98.28 | 98.28 | **100.00** 🏆 | 96.74 | 95.69 |
| SVM | 59.48 | 68.97 | **73.28** | 53.26 | 67.24 |
| Gradient Boosting | 96.55 | 95.69 | **98.28** | 93.48 | 94.83 |

---

## 🏆 Best Sampling Technique for Each Model

| Model | Best Technique | Accuracy |
|:------|:--------------:|:--------:|
| Logistic Regression | Bootstrap | 95.69% |
| Decision Tree | Systematic | 98.28% |
| **Random Forest** | **Systematic** | **100.0%** 🥇 |
| SVM | Systematic | 73.28% |
| Gradient Boosting | Systematic | 98.28% |

---

## 📈 Visualizations

<p align="center">
  <img src="images/heatmap.png" width="600" alt="Accuracy Heatmap"/>
</p>

<p align="center"><i>Heatmap showing accuracy of each model with different sampling techniques</i></p>

---

## 💡 Key Findings
```
✅ Random Forest + Systematic Sampling achieved 100% accuracy (Best Combination)

✅ Systematic Sampling performed best for 4 out of 5 models

✅ Cluster Sampling showed lowest performance across all models

✅ SVM had the lowest overall accuracy compared to other models

✅ Tree-based models (Decision Tree, Random Forest, Gradient Boosting) 
   consistently outperformed linear models
```

---

## 🎯 Final Conclusion

| Metric | Result |
|--------|--------|
| 🥇 **Best Model** | Random Forest |
| 🥇 **Best Sampling Technique** | Systematic Sampling |
| 🏆 **Best Combination** | Random Forest + Systematic (100%) |
| ⚠️ **Worst Sampling** | Cluster Sampling |
| ⚠️ **Worst Model** | SVM |

---

## 🚀 Quick Start
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/Sampling_Assignment.git

# Install dependencies
pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn

# Run the notebook
jupyter notebook Sampling_Assignment.ipynb
```

---

## 📁 Project Structure
```
Sampling_Assignment/
│
├── 📄 README.md
├── 📓 Sampling_Assignment.ipynb
├── 📊 Creditcard_data.csv
├── 📋 sampling_results.csv
├
└── 📁 images/
    └── heatmap.png
```

---

## 🛠️ Technologies Used

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/NumPy-013243?style=flat-square&logo=numpy&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--Learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white" />
  <img src="https://img.shields.io/badge/Matplotlib-11557C?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/Seaborn-3776AB?style=flat-square&logo=python&logoColor=white" />
</p>

---

## 👤 Author

<h3>Prabhleen Kaur</h3>

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/prabhleen003)

---

<p align="center">
  <b>⭐ Star this repository if you found it helpful!</b>
</p>
