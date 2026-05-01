**Exploratory Data Analysis (EDA) – Boston Housing Dataset**

**Dataset Overview**
The dataset contains 506 observations and 14 features, representing housing-related attributes and the target variable:
MEDV → Median value of owner-occupied homes (target variable)

**Feature Description**
CRIM: Crime rate per capita
ZN: Proportion of residential land zoned for large lots
INDUS: Proportion of non-retail business acres
CHAS: Charles River dummy variable (1 = near river, 0 = not)
NOX: Nitric oxide concentration (pollution level)
RM: Average number of rooms per dwelling
AGE: Proportion of old houses
DIS: Distance to employment centers
RAD: Accessibility to highways
TAX: Property tax rate
PTRATIO: Pupil-teacher ratio
B: Proportion of Black population (transformed variable)
LSTAT: % of lower-status population
MEDV: Median house price (target)

**Data Information**
Total rows 506 and 14 features and some features are float and integers.
Float64 is majority of features and Int64: RAD, TAX
Dataset contains both continuous and categorical (CHAS) variables
No duplicate data.

**Handle Missing Values**
Missing values were present in the following features:CRIM, ZN, INDUS, CHAS, AGE, LSTAT → each had 20 missing values.
Median imputation was applied to handle missing values because of data distribution is skewed. So median choice is better than mean.

**Skewness Analysis**
Highly positively skewed:
CRIM, ZN, CHAS → presence of extreme values
Moderately skewed:
DIS, RAD, LSTAT, MEDV
Negatively skewed:
AGE, PTRATIO, B

**Outlier Analysis & Removal**
Boxplots show significant outliers in features like CRIM, ZN, and LSTAT due to skewed distributions. These outliers were removed using the IQR method by filtering values outside the 1.5×IQR range.After cleaning, the dataset size reduced from (506, 14) to (217, 14), indicating a large number of extreme values were present.








