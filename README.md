# 🎗 Breast Cancer Classifier
A binary classification project that predicts whether a breast tumor is malignant or benign using the Wisconsin Breast Cancer dataset using Logistic Regression.

## 📌 Overview
Early and accurate detection of malignant tumors is critical in breast cancer diagnosis. This project uses Logistic Regression to distinguish between malignant and benign tumors based on cell nuclei measurements, and validates the model's reliability through cross-validation.


## ⚙️ Process
- **Data Preprocessing:** Cleaned data by removing outliers and by checking any NULL values but dataset doesn't contain any NULL values.
- **Exploratory Data Analysis (EDA):** Analyzed tumor characteristics and feature correlations using statistical and visual techniques.
- **Cross-Validation:** 5-fold stratified cross-validation used to evaluate model consistency across different subsets of data.
- **Model Evaluation:** Evaluate model through accuracy, F1 score, precision, recall and confusion matrix.

## 📊 Results
### **Cross-Validation:**
- Mean accuracy: 97.8% (± 0.9% std across 5 folds)
- Test accuracy: 98.25%
- Recall (malignant class): 98%, correctly identified 41/42 malignant cases
- Only 2 total misclassifications out of 114 test samples

## 🔍 Key Findings
- Cross-validation with low standard deviation (±0.9%) confirms the reported accuracy is stable and not the result of a favorable train/test split.
- Recall on the malignant class was prioritized, since false negatives (missed cancer diagnoses) carry the highest clinical cost.
- A linear model achieving ~98% accuracy suggests the relationship between these cell nuclei features and diagnosis is largely linear, supporting the use of a simple model over a more complex one.

## 🌐 Dataset Source
Dataset used in this project is **Wisconsin Diagnostic Breast Cancer dataset**, which is an in-built dataset available in scikit-learn library commonly used for Machine Learning tasks.

## 🛠 Technologies & Tools Used
- Python,
- Scikit-learn
- Pandas
- NumPy
- Matplotlib 
- Seaborn
- TensorFlow
