# University Admission Prediction  

## Project Overview  
This project predicts students' chances of admission to a university using various regression models based on academic and extracurricular criteria. The dataset contains features such as GRE scores, TOEFL scores, CGPA, university ratings, and research experience.  

---

## Table of Contents  
- [Dataset Details](#dataset-details)  
- [Project Steps](#project-steps)  
- [Technologies Used](#technologies-used)  
- [Results](#results)  
- [Installation](#installation)  

---

## Dataset Details  
The dataset includes the following columns:  
- **GRE Score**: Graduate Record Exam score  
- **TOEFL Score**: Test of English as a Foreign Language score  
- **University Rating**: University ranking (1 to 5)  
- **SOP**: Statement of Purpose quality (1 to 5)  
- **LOR**: Letter of Recommendation quality (1 to 5)  
- **CGPA**: Cumulative GPA on a scale of 10  
- **Research**: Research experience (1 = Yes, 0 = No)  
- **Chance of Admit**: Admission probability (target variable)  

---

## Project Steps  
1. **Data Exploration**  
   - Visualized feature distributions (GRE, TOEFL, CGPA, etc.).  
   - Generated a correlation matrix to examine relationships between features and the target.  

2. **Data Preprocessing**  
   - Standardized numerical features to improve model performance.  
   - Split data into training (80%) and test (20%) sets.  

3. **Model Training and Evaluation**  
   - Implemented and evaluated the following models:  
     - **Linear Regression**  
     - **Ridge Regression**  
     - **Lasso Regression**  
     - **Random Forest Regressor**  
   - Used **RMSE** and **R²** for model evaluation.  

4. **Hyperparameter Optimization**  
   - Applied **GridSearchCV** to optimize hyperparameters for Random Forest.  

5. **Results Visualization**  
   - Plotted a bar chart comparing model RMSEs.  

---

## Technologies Used  
- **Python 3.x**  
- Libraries:  
  - `pandas`  
  - `numpy`  
  - `matplotlib`  
  - `seaborn`  
  - `scikit-learn`  

---

## Results  
### Model Performance Comparison:  
| Model                  | RMSE      | R²         |  
|------------------------|-----------|------------|  
| Linear Regression      | 0.0609    | 0.8188     |  
| Ridge Regression       | 0.0609    | 0.8188     |  
| Lasso Regression       | 0.1435    | -0.0072    |  
| Random Forest          | 0.0654    | 0.7908     |  
| Optimized Random Forest| 0.0640    | 0.7999     |  

- The **Linear Regression** and **Ridge Regression** models performed best, achieving the lowest RMSE and highest R².  
- Lasso Regression underperformed due to its sensitivity to feature selection.  

---

## Installation  
1. Clone this repository:  
   ```bash  
   git clone https://github.com/niamat-sirrou/University_Admission_Prediction.git  
   cd University_Admission_Prediction  
