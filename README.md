## 1. Project Title
**ICU Mortality Prediction**

---

## 2. Problem Statement
Patients admitted to Intensive Care Units (ICUs) generate large amounts of physiological and clinical data. Predicting whether a patient is at risk of in-hospital death at an early stage can help doctors take timely and effective medical decisions. Manual analysis of such large datasets is difficult and time-consuming. Hence, an automated prediction system using machine learning is required.

---

## 3. Objective
The main objectives of this project are:
- To analyze ICU patient physiological data
- To build a machine learning model that predicts in-hospital mortality
- To evaluate the performance of the model using standard metrics
- To visualize results using graphs for better understanding

---

## 4. Dataset Description
The dataset used in this project is the **ICU Mortality Prediction Dataset** obtained from Kaggle.

### Dataset Structure:
- **set-a/**  
  Contains individual patient files with time-series physiological data such as:
  - Heart Rate
  - Blood Pressure
  - Respiratory Rate
  - Temperature
  - Oxygen Saturation, etc.

- **Outcomes-a.txt**  
  Contains the final outcome for each patient:
  - `RecordID`
  - `In-hospital_death`  
    - `0` → Patient survived  
    - `1` → Patient died  

The dataset contains missing values, which are handled during preprocessing.

---

## 5. Methodology
The project follows the steps below:

1. **Data Loading**
   - Load patient time-series data from Set-A
   - Load mortality outcome file

2. **Data Preprocessing**
   - Convert time-series data into patient-level features using mean values
   - Merge features with outcome data
   - Handle missing values using mean imputation
   - Normalize features using StandardScaler

3. **Model Building**
   - Apply Logistic Regression for binary classification

4. **Model Evaluation**
   - Accuracy Score
   - Classification Report
   - Confusion Matrix
   - ROC Curve

5. **Visualization**
   - Feature Importance
   - Class Distribution
   - Performance graphs

---

## 6. Tools and Technologies Used
- **Programming Language:** Python  
- **Platform:** Kaggle Notebook  
- **Libraries:**
  - NumPy
  - Pandas
  - Matplotlib
  - Scikit-learn  

---

## 7. Steps to Run the Project
1. Open Kaggle and create a new notebook
2. Add the ICU Mortality Prediction dataset to the notebook
3. Copy the provided Python code cell by cell into the notebook
4. Run each cell sequentially
5. Observe the output metrics and graphs

No manual extraction of zip files is required.

---

## 8. Results and Output
- The Logistic Regression model achieved an accuracy of approximately **84%**
- The confusion matrix shows high correct prediction for survival cases
- ROC Curve indicates good model performance with AUC around **0.8**
- Feature importance analysis highlights key physiological parameters affecting mortality
- Class distribution shows imbalance between survival and mortality cases

---

## 9. Conclusion
This project demonstrates that machine learning techniques such as Logistic Regression can effectively predict ICU mortality using physiological data. Although mortality prediction is challenging due to class imbalance, the model achieves reliable performance and can assist healthcare professionals in decision-making.

---

## 10. Future Scope
- Apply advanced models such as Random Forest or XGBoost
- Handle class imbalance using resampling techniques
- Use deep learning models for time-series analysis
- Deploy the model as a web-based clinical decision support system

---

## 11. Author
**BTech CSE – 2nd Semester**  
Project on Machine Learning in Healthcare
