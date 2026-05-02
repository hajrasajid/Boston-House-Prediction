
**Boston Housing Price Prediction (Linear Regression)**

This project applies Linear Regression to predict housing prices using the Boston Housing dataset. The workflow includes data cleaning, scaling, model training, evaluation, and interpretability analysis.

**Feature	Description**

CRIM	Crime rate,
ZN	Residential land zoning,
INDUS Non-retail business acres,
CHAS Charles River dummy variable,
NOX	Nitric oxides concentration,
RM	Average number of rooms,
AGE	Proportion of old houses,
DIS	Distance to employment centers,
RAD	Accessibility to highways,
TAX	Property tax rate,
PTRATIO	Pupil-teacher ratio,
B	Proportion of Black population,
LSTAT	% lower status population,
MEDV	Median house price (Target).

**Data Preprocessing**
Median imputation (skewed distributions)
Outlier removal using IQR method
Feature-target split
Train-test split (75% / 25%)
Feature scaling using StandardScaler

**Model Used**

Linear Regression (Scikit-learn)

**Model Performance**

Train RMSE (scaled): 0.548
Test RMSE (scaled): 0.666

**Residual Analysis**

✔ Residuals are normally distributed
✔ Indicates assumptions of Linear Regression are satisfied
✔ No major bias in predictions

**Feature Importance (Coefficients)**

**Positive Impact Features:**
RM (Rooms per house),
RAD,
CRIM.

**Negative Impact Features:**
LSTAT,
DIS,
TAX,
AGE,
PTRATIO,
NOX,
INDUS,
B.

**Interpretation**

More rooms → higher price
Higher poverty / tax / pollution → lower price

**Visualizations**

Actual vs Predicted Plot
Residual Plot
Feature Importance Plot

**Key Insights**

Housing price strongly depends on RM (rooms) and LSTAT (lower status population %).
Negative socio-economic factors reduce price significantly.
Linear model provides a strong baseline but may underfit complex relationships.

**Requirements**

numpy
pandas
scikit-learn
matplotlib
seaborn

**Author** 

Hajira Sajid  
Data Scientist | Building Real-World Machine Learning Solutions  

