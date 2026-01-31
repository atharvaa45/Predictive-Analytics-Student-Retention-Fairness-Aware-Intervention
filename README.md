# Predictive Analytics for Student Retention & Fairness-Aware Intervention

## 📌 Project Overview
This project presents an end-to-end predictive analytics system designed to identify students at high risk of academic dropout using imbalanced educational datasets. Beyond predictive accuracy, the system integrates fairness-aware evaluation and cost–benefit analysis to ensure that data-driven retention strategies are both effective and equitable across demographic groups.

The project combines classical machine learning, dimensionality reduction, and fairness diagnostics to support early intervention decision-making in academic institutions.

---

## 🎯 Problem Statement
Student attrition poses significant academic and financial challenges for universities. Traditional predictive models often:
- Perform poorly on minority or at-risk populations
- Optimize accuracy without considering recall for early-risk identification
- Ignore demographic fairness and intervention costs

This project addresses these gaps by:
- Prioritizing recall-focused prediction of at-risk students
- Auditing algorithmic bias across demographic groups
- Evaluating the financial impact of predictive retention strategies

---

## 🧠 Key Objectives
- Predict student dropout risk on highly imbalanced datasets
- Maximize early-risk detection (recall-focused optimization)
- Reduce multicollinearity via dimensionality reduction
- Evaluate algorithmic fairness across demographic groups
- Quantify financial trade-offs of data-driven interventions

---

## 🛠️ Tech Stack
- **Programming Language:** Python  
- **Machine Learning:** Scikit-learn  
- **Models:** Random Forest, Support Vector Machine (SVM), Stacked Ensemble  
- **Dimensionality Reduction:** Principal Component Analysis (PCA)  
- **Evaluation Metrics:** Average Precision (AP), Recall, Confusion Matrix  
- **Fairness Analysis:** False Positive Rate (FPR) disparity analysis  
- **Visualization:** Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  

---

## 📂 Dataset Description
The project uses three structured datasets containing:
- Academic performance indicators
- Enrollment and progression attributes
- Demographic variables for fairness auditing

The target variable represents student persistence vs. dropout status.  
All datasets exhibit **class imbalance**, motivating recall-focused modeling.

---

## 🔄 Project Pipeline

### 1️⃣ Data Ingestion & Exploration
- Loaded and inspected multiple academic datasets
- Assessed missing values, feature distributions, and class imbalance
- Identified potential data quality issues and inconsistencies

### 2️⃣ Data Preprocessing & Feature Engineering
- Cleaned and standardized numerical features
- Encoded categorical and demographic attributes
- Injected and analyzed synthetic data issues to test robustness
- Applied **PCA** to:
  - Reduce multicollinearity
  - Improve model stability across cross-validation folds

### 3️⃣ Modeling Strategy
- Trained baseline classifiers for comparison
- Built a **stacked ensemble model** combining:
  - Random Forest (nonlinear feature interactions)
  - Support Vector Machine (margin-based generalization)
- Optimized hyperparameters using cross-validation

### 4️⃣ Evaluation & Threshold Optimization
- Evaluated models using **Average Precision (AP)** due to class imbalance
- Achieved **0.93 Average Precision**
- Tuned decision thresholds to maximize **recall**, improving early-risk detection compared to baseline classifiers

### 5️⃣ Fairness-Aware Model Audit
- Conducted subgroup analysis across demographic attributes
- Measured **False Positive Rate (FPR)** disparities
- Identified potential algorithmic bias in intervention targeting
- Compared fairness outcomes before and after threshold adjustments

### 6️⃣ Cost–Benefit Analysis
- Estimated financial impact of false positives vs. false negatives
- Assessed trade-offs between intervention costs and retention gains
- Demonstrated how recall-focused, fairness-aware models improve ROI for retention programs

---

## 📊 Key Results
- **Average Precision:** 0.93  
- **Improved Recall:** Significant gains in early-risk student identification  
- **Stability:** PCA reduced performance variance across CV folds  
- **Fairness Insights:** Highlighted demographic disparities in false-positive rates  
- **Business Impact:** Data-driven interventions showed favorable cost–benefit trade-offs  

---

## 🔍 Why This Project Matters
This project goes beyond “just accuracy” by integrating:
- Imbalanced learning strategies
- Fairness diagnostics
- Financial reasoning

It demonstrates how machine learning can be responsibly applied in education to support equitable and effective decision-making.

---

## ▶️ How to Run
1. Clone the repository:
   ```bash
   https://github.com/atharvaa45/Predictive-Analytics-Student-Retention-Fairness-Aware-Intervention.git

2. Install dependencies:
    ```bash
    pip install numpy pandas scikit-learn matplotlib seaborn

3. Open the notebook:
    ```bash
    jupyter notebook

4. Run all cells sequentially in the main .ipynb file

🚀 Future Enhancements

Incorporate causal inference for intervention effectiveness

Extend fairness metrics (Equal Opportunity, Demographic Parity)

Deploy as an interactive dashboard for academic advisors

Automate model monitoring for drift detection

👤 Author

Atharva H
Graduate Student — Data Science
Focus Areas: Machine Learning, Responsible AI, Applied Analytics