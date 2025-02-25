# Understanding-Breast-Cancer-Data-
Software Design For Responsible Intelligent Systems-- Project 1

## Project Description
This project aims to predict the recurrence of breast cancer in patients using a dataset obtained from the class Git repository. The dataset consists of 9 independent features and 1 dependent target variable, which represents whether a patient experiences recurrence or not. The goal is to explore the dataset through Exploratory Data Analysis (EDA) and build classification models to predict recurrence effectively.
## Dataset Details
The dataset includes various attributes related to patient demographics, tumor characteristics, and treatment details.
Features of the Dataset:
- Independent Features
  - Age
  - Menopause status
  - Tumor size
  - Number of involved lymph nodes (inv-nodes)
  - Presence of node caps (node-caps)
  - Degree of malignancy (deg-malig)
  - Breast affected (left or right)
  - Tumor quadrant location (breast-quad)
  - Radiation therapy history (irradiat)
- Target Variable
  - Class (Recurrence or No Recurrence)
## Exploratory Data Analysis
In this part of the Jupyter Notebook, the data was first investigated for any missing values and inconsistencies. Once the data was cleaned and remedied for any null and invalid values, each column of the data frame was investigated for data type conversion. It was found that all of the columns needed to be converted over to categorical besides `deg-malig`. One-hot endcoding and mapping was utilized to convert the data types. 
## Univariate and Multivariate
The data was then visualized in differnt ways to show patterns, correlation, and frequency. Histograms, boxplots, and heatmaps were the main ways to show the data set.
## Classification Models
In the last part of the notebook, the code implemented K-Nearest Neighbors and Logistic Regression moddels. GridSearchCV was also utilized to find the optimal K value for KNN. Through these models, the project compares the calssification reports for the different models and observed class imbalance issues leading to poor recal for recurrence cases.
## Key Findings
Some key findings from this project that I found interesting includes:
- The age groups 40-49 and 50-59 has the highest occurrences of breast cancer.
- Tumors were more commonly found in the left lower quadrant of the left breast.
- Higher malignancy degrees were more prevalent in the dataset
- Class imballance significantly impacted the model performance, particularly for recurrence cases.
- KNN and GridSearchCV improved accuracy but still ignored the recurrence class.
- Logistic Regression performed better but still under preformed.
