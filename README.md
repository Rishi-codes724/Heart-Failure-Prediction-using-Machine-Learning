# Heart Failure Prediction using Machine Learning

## 📌 Overview
This project applies **machine learning algorithms** to predict heart disease based on clinical parameters such as age, cholesterol, blood pressure, and exercise-induced angina.  
The dataset is sourced from **Kaggle** and the target variable is **HeartDisease** (binary classification: 1 = disease, 0 = normal).

Algorithms implemented:
- **Random Forest**
- **XGBoost**
- **K-Nearest Neighbors (KNN)** with multiple distance metrics (Euclidean, Manhattan, Minkowski, Jaccard)
- **K-Means Clustering** with different distance measures

---

## ⚙️ Methodology
- **Data Preprocessing**
  - Encoding categorical variables (ChestPainType, ST_Slope, Sex, etc.)
  - Normalization/standardization of numerical features (RestingBP, Cholesterol, MaxHR, Oldpeak)
  - Handling class imbalance if required

- **Model Training**
  - Random Forest: Ensemble of decision trees
  - XGBoost: Gradient boosting with tuned hyperparameters
  - KNN: Tested with multiple distance metrics
  - K-Means: Clustering with Minkowski, Euclidean, Mahalanobis, and Jaccard distances

- **Evaluation Metrics**
  - Accuracy
  - Precision, Recall, F1-score
  - Confusion Matrix
  - AUC-ROC (for classification models)

---

## 📊 Results

| Model / Method              | Distance Metric | Accuracy (%) |
|------------------------------|-----------------|--------------|
| Random Forest (Classification) | -               | **89.49** |
| XGBoost (Classification)     | -               | 85.87 |
| KNN (Classification)         | Euclidean/Manhattan/Minkowski/Jaccard | ~82–85 |
| K-Means (Clustering)         | Minkowski       | 82.35 |
| K-Means (Clustering)         | Euclidean       | 82.89 |
| K-Means (Clustering)         | Mahalanobis     | 55.33 |
| K-Means (Clustering)         | Jaccard         | 59.04 |

---

## 🔑 Key Insights
- **Age, Cholesterol, and MaxHR** were the most influential features.
- **Random Forest** provided strong accuracy with balanced precision and recall.
- **XGBoost** achieved the highest predictive power but required more computational resources.
- **KNN** performance varied depending on the chosen distance metric.
- **Clustering approaches** were less effective compared to supervised learning.

---

## 🚀 Conclusion
Machine learning offers promising solutions for **early detection of heart disease**.  
- **XGBoost** achieved the highest accuracy, showcasing its ability to handle complex feature interactions.  
- **Random Forest** provided a simpler and computationally efficient alternative.  
- **KNN** highlighted the importance of distance metric selection.  

This project demonstrates how data-driven approaches can improve healthcare analytics, enabling faster diagnosis, personalized treatment, and better resource allocation.
