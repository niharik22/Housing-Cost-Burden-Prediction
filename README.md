#  Predicting Housing Cost Burden with Privacy-Preserving ML

This project aims to classify housing cost burden levels—**Not Burdened**, **Moderately Burdened**, and **Severely Burdened**—for owner-occupied households using only **proxy variables** (no income or rent data). Built as part of a research-backed course project at Cleveland State University.

---

## 🔍 Key Highlights

-  No sensitive income or rent data used — purely non-financial, privacy-conscious features  
-  Addressed **multi-class imbalance** with ROS, RUS, SMOTE, and SMOTE + Tomek Links  
-  Evaluation based on **Macro F1 Score** and **Macro PR AUC** for fairness across classes  
-  **SHAP explainability** (global + local) to visualize key feature impacts  
-  Models compared: Logistic Regression, Random Forest, XGBoost  
-  Top features:  
  - **Fair Market Rent (FMR)** – proxy for local housing costs  
  - **Income-to-Poverty Ratio (IPOV)** – economic strain indicator  
  - **Age of Householder (AGE1)** – demographic vulnerability signal  
  - **Persons per Room (PER)** – potential overcrowding indicator

---

##  Project Structure

```
housing-burden-ml/
├── data/                  # Raw and cleaned datasets
├── notebooks/             # EDA, modeling, and SHAP explainability notebooks
├── models/                # Serialized models (optional)
├── visuals/               # SHAP plots, confusion matrices, PR/ROC curves
├── requirements.txt       # Python dependencies
└── README.md              # Project documentation
```


## 📊 Data Source

- **Name**: Housing Affordability Data System (HADS)  
- **Source**: U.S. Department of Housing and Urban Development (HUD)  
- **Records**: 64,535 owner-occupied households  
- **Access**: [HADS Dataset](https://archives.huduser.gov/portal/datasets/hads.html)

---

## 🙌 Contributors

- Niharika Kalpam  
- Diana Greeby, MBA  
- Harshith Raju  
- Yawei Tang  
- Mentor: Prof. Michael Mina (Cleveland State University)

---

## 📄 License

MIT License — Feel free to reuse with credit.
