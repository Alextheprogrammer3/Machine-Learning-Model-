# Machine-Learning-Model-
# T20 Cricket Batting Performance Analysis and Prediction

## Project Overview

This project aims to analyze and predict batting performance in T20 cricket using machine learning techniques. The dataset used is `batting_stats_for_icc_mens_t20_world_cup_2024.csv`, which includes various metrics such as matches played (`Mat`), innings (`Inns`), runs scored (`Runs`), batting average (`Ave`), strike rate (`SR`), centuries (`100`), half-centuries (`50`), and number of ducks (`0`).

## Methodology

1. **Data Loading and Exploration**:
   - Loaded the dataset using Pandas and explored its structure to understand available features and target variables.
   - Conducted initial data cleaning by handling missing values and converting necessary columns to appropriate data types.

2. **Feature Engineering**:
   - Engineered new features like `Experience_Factor`, `Impact_Ratio`, and `Performance_Index` to capture player performance comprehensively.
   - Transformed non-numeric features like `HS` (highest score) into numeric form for modeling purposes.

3. **Model Development**:
   - Utilized various machine learning models such as Linear Regression, Random Forest Regression, and Neural Networks to predict strike rate (`SR`).
   - Employed techniques like feature scaling and polynomial features to enhance model performance and capture non-linear relationships.

4. **Model Evaluation**:
   - Evaluated models using metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and R-squared (`R2`) to assess predictive accuracy.
   - Visualized feature importances using plots to understand which factors contribute most to batting performance prediction.

5. **Model Optimization and Fine-tuning**:
   - Employed Grid Search Cross-Validation to optimize the hyperparameters of the Random Forest Regressor.
   - Tuned parameters such as the number of estimators (`n_estimators`), maximum depth (`max_depth`), and minimum samples split (`min_samples_split`) to improve model performance.

6. **Deployment and Persistence**:
   - Saved the trained Random Forest model using joblib for future deployment and reuse.
   - Demonstrated how to load the model from disk and make predictions.

## Results

- **Random Forest Model Performance**:
  - Mean Squared Error (MSE): 0.0751
  - Mean Absolute Error (MAE): 0.2382
  - Root Mean Squared Error (RMSE): 0.2740
  - R-squared (`R2`): -0.1054

## Conclusion

This project demonstrates the effective application of machine learning in analyzing and predicting batting performance in T20 cricket. By leveraging data-driven insights, teams and players can optimize strategies and improve their performance on the field.

---

**Repository Directory Structure:**

- `README.md`: Project overview, methodology, results, and conclusions.
- `batting_stats_analysis.ipynb`: Jupyter notebook containing detailed code implementation.
- `batting_stats_for_icc_mens_t20_world_cup_2024.csv`: Dataset used for analysis and modeling.
- `rf_model.pkl`: Saved Random Forest model for strike rate prediction.
