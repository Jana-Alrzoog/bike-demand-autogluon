
# 🚲 Bike Sharing Demand Prediction with AutoGluon
![image](https://github.com/user-attachments/assets/51e571b3-3dee-4e8b-9826-9e9c164b7668)


This repository contains a complete solution to the Kaggle [Bike Sharing Demand](https://www.kaggle.com/competitions/bike-sharing-demand) competition using **AutoGluon**, an AutoML library by AWS.

---

## 📊 Project Overview

The goal of this project is to predict the number of bike rentals per hour in Washington D.C. based on various features such as time, weather, and holidays.

---

## 🧠 Technologies Used

- Python 3.10+
- AutoGluon
- Pandas
- Matplotlib
- Jupyter Notebook
- Kaggle API

---

## 🔍 Workflow Summary

1. **Initial Model Training**
   - Trained baseline model using AutoGluon.
   - Observed poor performance (RMSLE: 1.77).

2. **Feature Engineering**
   - Added new features like `hour`, `dayofweek`, `is_weekend`, and `temp_bin`.
   - Improved model performance to RMSLE: 0.70.

3. **Hyperparameter Tuning**
   - Tuned `learning_rate`, `max_depth`, and `n_estimators`.
   - Achieved best result: RMSLE = 0.45.

4. **Kaggle Submission**
   - Predictions were submitted to the competition via Kaggle CLI.

---

## 📈 Results

| Model        | learning_rate | max_depth | n_estimators | RMSLE Score |
|--------------|----------------|-----------|--------------|--------------|
| initial      | default        | default   | default      | 1.77         |
| add_features | default        | default   | default      | 0.70         |
| hpo          | 0.05           | 10        | 300          | 0.45         |

---

## 📂 Repository Structure

```

.
├── notebook.ipynb                  # Jupyter notebook with full solution
├── submission.csv                  # Final Kaggle submission
├── model\_train\_score.png           # Training performance plot
├── model\_test\_score.png            # Kaggle submission performance plot
├── Bike\_Sharing\_Report\_Jana.docx  # Full project report
└── README.md                       # Project overview

````

---

## 📌 How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/bike-demand-autogluon.git
   cd bike-demand-autogluon
````

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```bash
   jupyter notebook
   ```

---

## 🏁 Final Thoughts

This project was a great opportunity to explore:

* Automated Machine Learning using AutoGluon
* The importance of feature engineering
* Hyperparameter tuning for better performance
* Submission workflows with Kaggle CLI

Thank you for checking out my work!

```

