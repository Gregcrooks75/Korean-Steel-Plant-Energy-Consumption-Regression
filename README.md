# Energy Storage Analysis

## Project Overview

This project involves analyzing energy storage data to classify fuel types in residential storages using logistic regression. The analysis process included several key steps:

- **Data Cleaning:** The dataset was initially explored to identify and remove redundant or irrelevant columns. The 'CAISO Flag' column, which was dominated by the 'OTHER' category, was removed. Location-based columns like 'Facility Zip' and 'Facility City' were also dropped due to high cardinality.

- **Target Variable Focus:** The analysis focused on the 'Customer Sector' column, filtering it to retain only 'Residential' entries. A new categorical variable, 'Fuel_Type_v2', was created to simplify the classification into 'Nonsolar' and 'Solar' categories.

- **Data Transformation:** The 'Nameplate Capacity' was log-transformed to address skewness in the data, and the dataset was further filtered to remove any 'Other' categories in 'Fuel_Type_v2'.

- **Model Training:** Logistic regression with Lasso regularization was employed to classify the fuel types. The model was evaluated using a confusion matrix and classification metrics, achieving an accuracy of 84%.

- **Visualization:** The results are visualized through a confusion matrix and a line chart showing the median nameplate capacity by year, providing insights into the trends and model performance.

## Visualizations

- **Data Cleaning Process:** A visual representation of the data cleaning steps is provided to illustrate the transformation from raw to cleaned data.

- **Median Name Plate Capacity by Year:** A line chart visualizes the trend in median nameplate capacity over the years.

- **Confusion Matrix:** A confusion matrix is used to evaluate the model's performance, accompanied by a table of classification metrics for interpretability.

## Conclusion

This analysis provides a comprehensive approach to understanding and classifying fuel types in residential energy storage systems. The use of logistic regression with Lasso regularization helps in focusing on significant features, leading to a robust model with high accuracy.
