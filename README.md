# Heart_Disease_Prediction


This project is focused on using AI and machine learning to predict heart disease from healthcare datasets. It implements a range of classification algorithms and data pre-processing techniques to deliver accurate, early detection of heart disease, thereby supporting more effective and timely interventions.

## 📊 Dataset

- **Source:** [Kaggle - Heart Disease Dataset](https://www.kaggle.com/datasets/oktayrdeki/heart-disease/data)
- **Size:** 10,000 records
- **Features:** 21
- **Key Variables:**
  - Demographic: Age, Gender
  - Medical: Blood Pressure, Cholesterol, BMI, Homocysteine, CRP, etc.
  - Lifestyle: Smoking, Exercise, Alcohol
  - Target: Heart Disease Status (Binary: 0 = No, 1 = Yes)

## 🔧 Preprocessing Steps

- **Missing Data Handling:** KNN Imputer (n_neighbors=5) for ~3,000 missing values
- **Duplicates:** Removed
- **Categorical Encoding:** Applied to 12 categorical variables
- **Scaling:** Normalized numerical features to [0,1]
- **Class Imbalance:** Up-sampling of the minority class to 50% using synthetic techniques

## 🧠 Models Used

- Random Forest (Best Performing)
- Logistic Regression
- Support Vector Machine (SVM)
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Decision Tree

### ✅ Best Model: Random Forest

- **Parameters:**
  - n_estimators = 200
  - max_depth = 20
  - min_samples_split = 2
- **Performance:**
  - Accuracy: **91%**
  - Precision (Positive Class): **92%**
  - Recall (Positive Class): **91%**
  - AUC Score: **0.90**
- **Top Features:** BMI, Homocysteine Level, CRP Level, Sleep Hours, Triglycerides

## 📈 Evaluation Metrics

- Confusion Matrix & Heatmap
- ROC Curve & AUC
- Precision, Recall, F1-Score

## 📁 Project Structure

├── a2-healthcare-100661485.ipynb # Jupyter Notebook with model implementation
├── Heart_disease_prediction_100661485.pptx # Presentation summarizing the project
└── README.md # Documentation


## 💡 Key Takeaways

- Machine learning models—especially Random Forest—can accurately predict heart disease with minimal input.
- Preprocessing and class balancing significantly improve model reliability.
- KNN imputation is more suitable than mean/median when data relationships matter.

## 👨‍⚕️ Author

**Student ID:** 100661485  
**Module:** Data Mining and Foundations of AI (6CC555)  
**Institution:** School of Computing and Engineering

## 🔗 References

- Oktay Ördekçi (2025). Heart Disease Dataset. [Kaggle](https://www.kaggle.com/datasets/oktayrdeki/heart-disease/data)
- [Scikit-learn ROC Guide](https://scikit-learn.org/stable/auto_examples/model_selection/plot_roc.html)

---


