# Black Friday Sales Prediction

![Black Friday Sales Prediction](https://searchengineland.com/figz/wp-content/seloads/2014/12/black-friday1-ss-1920.jpg)

## Table Of Contents
- [Project Introduction](#project-introduction)
- [Dataset Description](#dataset-description)
- [Exploratory Data Analysis (EDA)](#eda)
- [Data Preprocessing](#data-preprocessing)
- [Modeling Phase](#modeling-phase)
- [Evaluation Metric](#evaluation-metric)
- [Conclusion](#conclusion)

### Project Introduction
Black Friday, the day after Thanksgiving in the United States, marks the start of the Christmas shopping season. Retailers often offer significant promotions and open early to attract customers. The main challenge for retailers is to set product prices to maximize profits. This project aims to predict product prices using historical sales data, helping retailers optimize their pricing strategy for higher profits.

### Dataset Description
The dataset, sourced from an Analytics Vidhya hackathon, includes features such as age, gender, marital status, product categories, city demographics, and purchase amounts. It contains 12 columns and 537,577 records. Our goal is to predict the purchase amount for products.

### Exploratory Data Analysis (EDA)
Key observations from the data:
- Approximately 75% of purchases are made by male customers, who also tend to spend more on average compared to female customers.
- Single men spend the most during Black Friday, whereas married men spend less, possibly due to increased responsibilities.
- Consumers aged 25-40 are the highest spenders.
- People who have lived in their current city for one year spend the most, likely due to the need to buy more new items.
- City B contributes the most to overall sales, but the specific product analyzed is purchased more in city C.

### Data Preprocessing
- Encoded categorical columns (Age, Gender, City_Category) using LabelEncoder.
- Converted the categorical variable Stay_In_Current_City_Years into dummy variables using pandas' get_dummies.
- Filled missing values in Product_Category_2 and Product_Category_3.

### Modeling Phase
- Split the dataset into train and test subsets with an 80:20 ratio.
- Implemented several supervised models, including Linear Regression, Decision Tree Regressor, Random Forest Regressor, and XGBoost Regressor.

### Evaluation Metric
The Root Mean Square Error (RMSE) is used to measure the model's prediction accuracy. RMSE is the square root of the average squared differences between predicted and actual values.

### Conclusion
Multiple supervised models were tested, including Linear Regression, Decision Tree Regressor, Random Forest Regressor, and XGBoost Regressor. Based on RMSE scores, the XGBoost Regressor performed the best with an RMSE score of 2879.

---

Feel free to contribute to this project by forking the repository and submitting pull requests. For significant changes, please open an issue first to discuss your ideas. If you find this project useful, consider giving it a star!