# Water Potability Prediction – ML Project

##  Objective

To develop a machine learning model that predicts whether a given water sample is **safe for human consumption** based on its chemical properties. This helps water testing companies, municipalities, and filtration system providers **automate quality control**, reduce lab testing costs, and protect public health.

---

##  Project Overview

This project uses the [Water Potability Dataset](https://www.kaggle.com/adityakadiwal/water-potability) which contains `3,276` samples with `9 chemical features` (like pH, hardness, turbidity, etc.) to predict the target: `Potability` (0 = Not Safe, 1 = Safe).

###  Steps Performed:

- Data Cleaning (handled missing values: ph, sulfate, trihalomethanes)
- Outlier handling & encoding
- Exploratory Data Analysis (univariate & bivariate)
- Feature Selection (L1 & correlation-based)
- Model Training & Tuning (KNN, Logistic Regression, Decision Tree, Random Forest, XGBoost)
- Hyperparameter Optimization (GridSearchCV)
- Pipeline Saving for Future Inference
- Final Prediction on Unseen Data

---

## Features Used

- `ph`, `Hardness`, `Solids`, `Chloramines`, `Sulfate`, `Conductivity`, `Organic_carbon`, `Trihalomethanes`, `Turbidity`

---

## Results & Performance

Below is the comparison of model performance **before and after feature engineering & hyperparameter tuning**:

| Metric          | Baseline Model (KNN) | Final Model (Random Forest) |
|------------------|----------------------|------------------------------|
| Accuracy (%)     | 61.91                | **66.91**                    |

- Random Forest achieved the highest test accuracy after tuning and outperformed all other models, including the baseline KNN.

---

###  Business Problem

In many regions, water quality testing is **manual, time-consuming, and costly**. Every water sample goes through lab testing, which requires chemicals, skilled technicians, and hours of analysis.

###  Proposed ML Solution

This model automates the classification of water as **potable or non-potable** based on physical and chemical measurements collected via sensors or rapid kits.

###  Business Value

| Area                      | Impact                                 |
|---------------------------|----------------------------------------|
|  Cost Saving             | Reduces need for lab tests by ~50%    |
|  Faster Turnaround       | Instant predictions (<1 sec)          |
|  Efficiency              | Test 1,000+ samples automatically     |
|  Public Health           | Early detection of unsafe samples     |

###  Conclusion

By integrating this model into an IoT-enabled water quality device or web system:
- Municipalities can ensure safer water supplies
- Companies can save time and money on routine checks
- Public can access clean water more reliably

---


## Future Improvements

- Integrate deep learning for feature extraction
- Build a Streamlit interface for easy field use
- Incorporate more sensor-based real-time data

---

##  Author

**Raza Bhatti** – Data Scientist | ML Developer  
Inspired by real-world water safety challenges 



