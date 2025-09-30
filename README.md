```markdown
# Heart Disease Analysis and Prediction

### Author  
Anam Jafar  

### Start Date  
December 22, 2024  



## Project Overview  
This project analyzes the UCI Heart Disease dataset to uncover patterns related to cardiovascular risk factors and build supervised learning models to predict the presence or absence of heart disease.
The work involves exploratory data analysis (EDA), data preprocessing, handling class imbalance, and evaluating machine learning models.  



## Dataset  
- **Source:** UCI Machine Learning Repository (Cleveland subset)  
- **Size:** 303 patient records  
- **Attributes:** 13 clinical features and 1 target variable  

### Key Features  
- **Age:** Age in years  
- **Sex:** Gender (1 = Male, 0 = Female)  
- **Chest Pain Type (cp):** Typical angina, atypical angina, non-anginal pain, asymptomatic  
- **Resting Blood Pressure (trestbps):** Measured in mmHg  
- **Serum Cholesterol (chol):** Measured in mg/dL  
- **Fasting Blood Sugar (fbs):** > 120 mg/dL (1 = True, 0 = False)  
- **Resting ECG (restecg):** Normal, ST-T wave abnormality, or left ventricular hypertrophy  
- **Maximum Heart Rate (thalach)**  
- **Exercise-Induced Angina (exang):** 1 = Yes, 0 = No  
- **ST Depression (oldpeak):** Exercise-induced depression relative to rest  
- **Slope of ST Segment (slope):** Upsloping, flat, downsloping  
- **Number of Major Vessels (ca):** 0–3, detected by fluoroscopy  
- **Thalassemia (thal):** Normal, fixed defect, reversible defect  
- **Target:** 1 = Disease present, 0 = No disease  


## Methodology  
### 1. Exploratory Data Analysis (EDA)  
- Analyzed distributions and correlations among clinical features  
- Identified significant class imbalance in the target variable  
- Addressed missing values in `ca` and `thal`  

### 2. Preprocessing  
- One-hot encoded categorical features  
- Standardized numerical features  
- Imputed missing values with the median  

### 3. Handling Class Imbalance  
- Applied SMOTE to balance class distribution  
- Confirmed equal representation of classes after oversampling  

### 4. Modeling and Evaluation  
- Models trained: Logistic Regression, Random Forest, Support Vector Machine  
- Evaluation metrics: Accuracy, Precision, Recall, F1-score  
- Adjusted class weights to improve minority class predictions  



## Results  
- **Best Model:** Random Forest Classifier with class weights  
- **Accuracy:** 66.1%  
- **Performance:**  
  - High precision and recall for class 0 (no disease)  
  - Improved recall for class 1 after balancing  
  - Minority classes (3 and 4) remained difficult to predict due to feature overlap and limited data  



## Challenges  
- **Class Imbalance:** Despite SMOTE, minority classes were poorly represented in predictions  
- **Feature Overlap:** Overlapping attributes limited model differentiation  
- **Dataset Size:** Small dataset reduced the models’ ability to generalize effectively  



## Conclusion  
- Random Forest showed the most robust performance overall  
- SMOTE and class weighting improved recall for some minority classes  
- Precision and recall for minority classes remained low  



## Recommendations  
- **Collect More Data:** Especially for underrepresented classes  
- **Feature Engineering:** Incorporate domain-specific clinical features  
- **Advanced Methods:** Explore ensemble or hybrid models  
- **Binary Classification:** Simplify prediction to presence vs. absence of heart disease for stronger results  



## Tools and Technologies  
- **Programming Language:** Python  
- **Libraries:** pandas, matplotlib, seaborn, scikit-learn  



## Contact  
- **LinkedIn:** [linkedin.com/in/anam-jafar6](https://www.linkedin.com/in/anam-jafar6/)  
- **GitHub:** [github.com/anamjafar6](https://github.com/anamjafar6)  
```
