# NAFLD Risk Prediction System

The **NAFLD Risk Prediction System** is a machine learning-based project designed to predict the likelihood of Non-Alcoholic Fatty Liver Disease (NAFLD) progression. This system leverages data preprocessing, feature engineering, and predictive modeling to provide healthcare insights for early diagnosis and improved treatment outcomes.

## Features
- Comprehensive data cleaning and preprocessing to improve data quality
- Exploratory Data Analysis (EDA) to identify trends and insights
- Feature engineering for better model performance
- Machine learning models such as Logistic Regression, Random Forest, and XGBoost
- Techniques to handle class imbalance, including SMOTE and class weighting
- Visualizations for performance metrics like confusion matrix, classification report, and ROC curve
- Clear code structure with documentation for easy understanding

## Dataset
The dataset contains data from a population study on Non-Alcoholic Fatty Liver Disease (NAFLD). It includes subjects diagnosed with NAFLD and a set of matched control subjects followed for metabolic conditions, cardiac endpoints, and mortality.

### Key Features
- `age`: Age of the subject
- `male`: Gender indicator (1 = Male, 0 = Female)
- `height`: Height in cm
- `bmi`: Body Mass Index
- `futime`: Follow-up time in days
- `status`: Target variable (0 = No NAFLD progression, 1 = NAFLD progression)

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/NAFLD-Risk-Prediction-System.git
   cd NAFLD-Risk-Prediction-System




---

### **Detailed Project Explanation**
Here’s a breakdown of key parts of your project to help you understand the process:

### **1. Data Preprocessing**
- **Missing Values Handling:** Filling missing data with appropriate methods (mean, median, or mode) based on feature distribution.  
- **Outlier Removal:** Identified and removed extreme values using IQR for cleaner data.  
- **Feature Engineering:** Created the `age_bmi_interaction` feature to capture combined effects on NAFLD risk.  
- **Encoding Categorical Variables:** Applied one-hot encoding or label encoding where necessary.  
- **Data Scaling:** Used `StandardScaler` to ensure numerical features are on the same scale.  

---

### **2. Exploratory Data Analysis (EDA)**
- **Distribution Analysis:** Histograms, boxplots, and violin plots to understand feature distributions.  
- **Correlation Analysis:** Heatmaps to detect highly correlated features.  
- **Feature Interaction Analysis:** Identified patterns between BMI, age, and NAFLD progression.

---

### **3. Model Building**
- **Logistic Regression:** Baseline model for binary classification.  
- **Random Forest:** Added to capture non-linear patterns and improve recall.  
- **XGBoost:** Used for optimizing prediction performance and minimizing false negatives.  
- **SMOTE (Synthetic Minority Over-sampling Technique):** Applied to handle class imbalance by oversampling minority class data.  

---

### **4. Model Evaluation**
- **Confusion Matrix:** Visualized true positives, true negatives, false positives, and false negatives.  
- **Classification Report:** Evaluated precision, recall, and F1-score.  
- **ROC Curve:** Used for adjusting model decision thresholds for optimal balance between precision and recall.  

---

### **5. Prediction Pipeline**
- Prepared new data by ensuring feature consistency.  
- Applied the same data preprocessing steps (e.g., scaling, feature engineering).  
- Output includes both **class predictions** and **probability scores** for better decision-making.  

---

### **6. Future Improvements**
- Tuning hyperparameters for improved model performance.  
- Exploring ensemble methods for stronger prediction stability.  
- Integrating deep learning models like **ANNs** or **LSTMs** for improved recall on minority class.

---

This README provides everything you need to structure your project effectively on GitHub. If you'd like to expand specific sections or add visual examples, let me know! 🚀

