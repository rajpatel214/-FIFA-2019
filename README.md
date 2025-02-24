**Project Title: FIFA 2019 Player Analysis and Performance Prediction**

**Objective:**  
The objective of this project is to analyze the FIFA 2019 player dataset and develop a predictive model to estimate a player's overall rating based on key performance indicators. The analysis helps in understanding player characteristics, market value, and performance trends.

**Dataset Overview:**  
The dataset consists of FIFA 2019 player statistics, including attributes like age, nationality, club, position, skills, physical attributes, and financial data (market value, wage, release clause). The dataset also includes performance-related metrics like passing accuracy, dribbling, finishing, and defensive abilities.

**Data Preprocessing:**  
- Unnecessary columns such as images and logos were removed to avoid redundant data.
- Missing values were handled using appropriate imputation techniques:
  - Numerical attributes were filled using median values.
  - Categorical attributes were filled using the mode.
  - Some text-based columns were assigned default values.
- Currency symbols and units (like €M, €K) were converted into numerical format for proper analysis.

**Feature Selection:**  
A subset of important features was selected, including player attributes, performance indicators, and physical attributes. This selection helps in improving the accuracy of predictive models by removing irrelevant variables.

**Exploratory Data Analysis (EDA) Summary:**  
The analysis provided insights into player distribution based on age, position, preferred foot, international reputation, and weight distribution across different nationalities. Visualizations such as histograms, scatter plots, and violin plots helped understand trends in player characteristics and their impact on performance.

**Predictive Modeling:**  
To predict the overall rating of a player, multiple regression models were implemented and compared:

1. **Linear Regression:** Achieved an accuracy score of **91%**.
2. **Ridge Regression:** Also resulted in an accuracy of **91%**, reducing overfitting compared to linear regression.
3. **Lasso Regression:** Showed a slightly lower accuracy of **90%**, indicating feature selection was necessary.
4. **ElasticNet:** Combined Ridge and Lasso regression techniques but had a performance of **90%**.
5. **Support Vector Regression (SVR):** Outperformed linear models with an accuracy of **97%**.
6. **Decision Tree Regression:** Used to visualize decision splits but was less interpretable.
7. **Random Forest Regression:** Provided the best accuracy of **97%**, showing high predictive power for estimating player performance.

**Final Conclusion:**  
The FIFA 2019 player dataset provides valuable insights into player attributes and their influence on performance. Among various regression models tested, **Random Forest Regressor and Support Vector Regression (SVR) performed the best with an accuracy of 97%**, making them the most reliable choices for predicting a player's overall rating. This analysis can assist football clubs and analysts in scouting and evaluating players based on data-driven insights.

