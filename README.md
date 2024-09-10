# Dengue Fever Prediction using Machine Learning

This repository contains a comprehensive analysis of dengue fever prediction using advanced machine learning models. The project focuses on predicting dengue fever outbreaks in the tropical cities of San Juan (Puerto Rico) and Iquitos (Peru) based on historical data involving climate factors, population demographics, and previous disease occurrences.

## Dataset

The dataset contains:
- **Training Data**: 1456 records with 25 features
- **Test Data**: 416 records
- Features include city, year, week of the year, climate-related information, and total dengue cases.
- Data was merged and preprocessed for model training, including missing values handling and categorical encoding.

## Analysis Workflow

1. **Exploratory Data Analysis (EDA)**: 
   - Performed to understand dataset characteristics, detect trends, and identify outliers.
   - Visualizations included line graphs showing spikes in dengue cases and histograms indicating seasonal patterns.

2. **Data Preprocessing and Feature Engineering**:
   - Missing values were handled using median imputation.
   - Temporal variables were transformed, and categorical variables were encoded for model input.
   - Features were scaled using StandardScaler for improved model performance.

3. **Model Building**:
   - Various machine learning models were implemented:
     - **Decision Trees**
     - **Random Forest**
     - **Gradient Boosting**
     - **XGBoost**
   - Performance metrics included **Mean Squared Error (MSE)**, **Mean Absolute Error (MAE)**, and **R-squared**.

4. **Hyperparameter Tuning**:
   - **GridSearchCV**, **Optuna**, and **TPOT** were applied to optimize model parameters and improve performance.

## Key Findings

- **EDA Results**: 
  - A notable surge in dengue cases between 1997-1999, particularly during weeks 35-49, suggesting seasonal factors.
  - San Juan consistently reported more cases than Iquitos, emphasizing geographical differences in disease burden.
  
- **Model Performance**: 
  - **XGBoost** emerged as the top-performing model with an R² score of 0.774 and the lowest MSE of 0.364.
  - After hyperparameter tuning with **Optuna**, **Gradient Boosting** achieved the best performance with an R² of 0.815 and an MSE of 0.297.

## Conclusion

This research demonstrates the potential of machine learning models, especially ensemble methods like Gradient Boosting and XGBoost, to predict dengue fever outbreaks with high accuracy. The integration of automated hyperparameter tuning techniques, such as Optuna and TPOT, further enhanced model performance.
