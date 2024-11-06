# Energy Consumption Prediction Project



## Aim

The objective of this project is to predict **Active Power Consumption (kWh)** in an industrial setting using historical data from the steel industry. Active Power, measured in kWh, represents the usable energy in an AC circuit. Given the importance of `Usage_kWh` as a measure of real power consumption, our analysis focuses primarily on this field.



### Key Assumptions

- Time-related variables (e.g., weekday, time of day) affect power consumption patterns.

- Power factor fields are useful indicators of energy efficiency, as they highlight the ratio of active power to apparent power in a circuit.



## Data Preparation

To begin the analysis, data was loaded, cleaned, and formatted:

- **Column Renaming**: Original column names were standardized for readability.

- **Datetime Processing**: The date field was converted to datetime format, and separate columns for day, month, and year were created.

- **Handling Duplicates and Missing Values**: The dataset was checked for duplicates and missing values, with none found.



## Outlier Detection and Transformation

- **Outlier Detection**: Strong skewness and outliers were observed in power factor and reactive power fields.

- **Data Transformation**: Right-skewed variables were transformed using the Interquartile Range (IQR) method to reduce outlier impact, especially for non-normal distributions.



## Feature Engineering

Additional features were created to enhance predictive power:

- **Holiday Identification**: A dataset of holidays was integrated to analyze consumption patterns on holidays vs. non-holidays.

- **Daily and Previous Day Usage**: Summarized daily usage of active power and created a lag feature to represent previous day’s consumption.



## Exploratory Data Analysis (EDA)

- **Correlation Analysis**: A heatmap revealed strong collinearity between CO2 and Active Power.

- **Consumption Patterns**: Analyzed consumption by day of the week, week status (weekday vs. weekend), and load type to uncover patterns:

- **Highest Consumption**: Tuesday has the highest average active power consumption, while Sunday has the lowest.

- **Load Types**: Distribution of load types (e.g., light, medium, maximum) was examined to understand energy demand variation.



## Predictive Modeling

- **Data Splitting**: The dataset was split into training and testing sets.

- **Preprocessing and Scaling**: Numerical features were scaled, and categorical features were encoded.

- **Model Selection**: Various machine learning models, including Linear Regression, were evaluated based on accuracy.



## Key Findings

- **Day and Time Impact**: Energy consumption varies significantly by day of the week and load type, with higher consumption observed on weekdays.

- **Seasonal Trends**: Winter months, especially January, show higher average power consumption, particularly for light loads.



This project provides valuable insights into industrial energy usage patterns, paving the way for more efficient energy management and targeted predictions of power needs.
