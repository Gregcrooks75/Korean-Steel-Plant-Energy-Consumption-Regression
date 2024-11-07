# Korean Steel Plant Energy Consumption Regression



This project provides an in-depth analysis and regression model to predict energy consumption in a Korean steel plant. Using Exploratory Data Analysis (EDA) and regression techniques, the project uncovers patterns in energy use, focusing on optimizing energy management strategies.



---



## Project Overview



The analysis is based on a dataset containing variables related to date, time, and energy usage characteristics. It assumes that energy consumption patterns vary based on time and load type, leading to the following steps:



### Objectives

1. **Identify Key Factors** influencing energy consumption.

2. **Build a Predictive Model** to accurately forecast energy needs.

3. **Generate Insights** for optimizing energy use.



## Workflow



### 1. Data Preprocessing

- **Data Cleaning**: Removal of duplicates and handling of missing values.

- **Feature Engineering**: Creation of new features based on date and time data (e.g., extracting day, month, and year).

- **Outlier Detection**: Identification and removal of outliers to ensure model accuracy.



### 2. Exploratory Data Analysis (EDA)

- **Variable Analysis**: Initial analysis of distributions, relationships, and patterns.

- **Correlation Analysis**: Examination of relationships between variables, focusing on the correlation between power consumption and emissions.

- **Temporal Consumption Patterns**: Analysis of power usage across different times and days.



### 3. Model Training and Evaluation

Three models were trained to predict energy consumption:

- **Linear Regression**: Achieved a high R² score, providing a straightforward and interpretable baseline.

- **Ridge Regression**: Improved robustness against multicollinearity with similar accuracy to Linear Regression.

- **Lasso Regression**: Selected key features by shrinking less important coefficients to zero, providing a simplified model.



#### Model Evaluation Metrics:

- **R² (Coefficient of Determination)**

- **Mean Absolute Error (MAE)**

- **Root Mean Squared Error (RMSE)**



### 4. Key Findings

- **Temporal Variations**: Energy consumption patterns varied significantly by time of day and day of the week.

- **Correlation with CO₂ Emissions**: Strong correlation between energy usage and CO₂ emissions.

- **Load Type Distribution**: The majority of usage came from certain load types, providing insights for targeted energy management.



---



## Results and Conclusions



- **Optimal Model**: Linear and Ridge Regression models were most effective for prediction, achieving similar performance.

- **Predictive Insights**: The analysis highlights key patterns in energy consumption, which can support more efficient and sustainable operations.

- **Business Implications**: By understanding consumption drivers, the plant can make informed decisions to manage peak demand, optimize resource allocation, and reduce costs.



## Files

- `Korean Steel Plant Energy Consumption Regression.ipynb`: Main notebook with code for data processing, analysis, model training, and evaluation.



## Getting Started

1. Clone the repository.

2. Ensure required libraries are installed.

3. Run the Jupyter Notebook to reproduce the analysis and results.



