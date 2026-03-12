# Titanic---Machine-Learning-from-Disaster
# Titanic Survival Prediction – Machine Learning Experiments

## Project Overview

This repository contains multiple machine learning experiments performed on the **Titanic Dataset** from the **Kaggle** competition *Titanic - Machine Learning from Disaster*.
The goal of the project is to build predictive models that determine whether a passenger survived the Titanic disaster using features such as age, class, fare, and family relationships.

The experiments focus on comparing different machine learning algorithms and improving predictive performance through **hyperparameter tuning and model stacking**.

---

## Methodology

The workflow used in these experiments includes:

1. Data preprocessing and feature engineering
2. Handling missing values and categorical variables
3. Feature scaling when required by algorithms
4. Model training using different machine learning techniques
5. Hyperparameter optimization
6. Ensemble learning using stacking methods
7. Evaluation using Kaggle public leaderboard scores

The models were trained and evaluated using the standard Titanic dataset provided in the Kaggle competition.

---

## Experiments and Results

The following models were trained and submitted to Kaggle. The scores represent the **public leaderboard accuracy**.

### 1. Tuned XGBoost with Stacking – Version 2

**Score:** 0.78708

This model combines a tuned gradient boosting model with additional base learners through stacking.
Hyperparameters of the gradient boosting model were optimized to improve generalization. The stacking approach helps combine the strengths of multiple models and reduce variance.

**Key characteristics**

* Gradient boosting based primary model
* Multiple base learners combined through stacking
* Tuned hyperparameters for improved performance
* Best performing model among the experiments

---

### 2. Tuned XGBoost with Stacking – Version 1

**Score:** 0.76794

This experiment represents an earlier version of the stacked ensemble. The model used a similar architecture but with fewer tuning iterations and slightly different feature engineering steps.

**Key characteristics**

* Ensemble model with stacking
* Early stage hyperparameter tuning
* Improved performance compared to single models

---

### 3. Optimized Support Vector Machine

**Score:** 0.78468

This experiment uses a **Support Vector Machine classifier** with optimized hyperparameters. Feature scaling and parameter tuning were applied to improve model performance.

**Key characteristics**

* Kernel-based classification
* Hyperparameter tuning for regularization and kernel parameters
* Strong performance close to ensemble methods

---

### 4. XGBoost Baseline Model

**Score:** 0.75358

This experiment uses a basic **gradient boosting model** without extensive tuning or stacking. It serves as a baseline for comparison with the more advanced models.

**Key characteristics**

* Gradient boosting model
* Minimal hyperparameter tuning
* Baseline reference for further improvements

---

## Result Summary

| Model                                | Kaggle Score |
| ------------------------------------ | ------------ |
| Tuned XGBoost + Stacking (Version 2) | 0.78708      |
| Optimized SVM                        | 0.78468      |
| Tuned XGBoost + Stacking (Version 1) | 0.76794      |
| XGBoost Baseline                     | 0.75358      |

The results show that **ensemble learning and hyperparameter tuning significantly improve performance** compared to baseline models.

---

## Key Insights

* Ensemble models such as stacking can improve predictive performance by combining multiple algorithms.
* Hyperparameter optimization plays a critical role in boosting model accuracy.
* Support Vector Machines remain competitive with modern boosting techniques when properly tuned.
* Baseline models provide useful references for measuring improvements.

---

## Repository Structure

```
.
├── notebooks/
│   ├── tuned_xgboost_stacking_v1.ipynb
│   ├── tuned_xgboost_stacking_v2.ipynb
│   ├── optimized_svm.ipynb
│   └── xgboost_baseline.ipynb
│
├── data/
│   └── titanic_dataset
│
├── results/
│   └── kaggle_scores
│
└── README.md
```

---

## Tools and Libraries

* Python
* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Matplotlib / Seaborn

---

## Future Improvements

Potential directions for improving performance include:

* Advanced feature engineering
* More extensive cross-validation
* Additional ensemble techniques such as blending
* Neural network based models

---

## Author

Machine learning experiments developed as part of hands-on practice with supervised learning and ensemble methods on the Titanic survival prediction problem.
