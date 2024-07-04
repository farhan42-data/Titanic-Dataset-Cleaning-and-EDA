# Titanic-Dataset-Cleaning-and-EDA

## Introduction
This project involves data cleaning and exploratory data analysis (EDA) on the Titanic dataset. The dataset contains information about passengers on the Titanic, including whether they survived, their age, sex, passenger class, fare, and more. The primary goal is to explore the relationships between variables and identify patterns and trends in the data.

## Dataset
The dataset used in this project is the Titanic dataset, which is publicly available on [Kaggle](https://www.kaggle.com/c/titanic/data). The dataset contains 891 rows and 12 columns.

### Columns
- `Survived`: Survival (0 = No, 1 = Yes)
- `Pclass`: Ticket class (1 = 1st, 2 = 2nd, 3 = 3rd)
- `Name`: Name of the passenger
- `Sex`: Sex of the passenger
- `Age`: Age of the passenger
- `SibSp`: Number of siblings/spouses aboard the Titanic
- `Parch`: Number of parents/children aboard the Titanic
- `Ticket`: Ticket number
- `Fare`: Passenger fare
- `Cabin`: Cabin number
- `Embarked`: Port of Embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)

## Project Structure
- `Titanic_Dataset_Cleaning_and_EDA.ipynb`: Jupyter notebook containing the data cleaning and EDA steps.
- `README.md`: This file, providing an overview of the project.

## Data Cleaning
The data cleaning process involved the following steps:
1. **Handling Missing Values**:
   - Missing values in the `Cabin` column were filled with 'Unknown'.
   - Missing values in the `Age` column were filled with the median age.
   - Missing values in the `Embarked` column were filled with the mode (most common value).
   - Verification ensured no missing values were left.

## Exploratory Data Analysis (EDA)
The EDA process involved both univariate and multivariate analyses to uncover insights from the data.

### Univariate Analysis
- **Age Distribution**: Visualized using a histogram to show the distribution of passenger ages.
- **Survival Count**: Visualized using a bar plot to show the count of survivors and non-survivors.

### Bivariate Analysis
- **Age vs Fare**: Explored using a scatter plot to examine the relationship between age and fare.
- **Correlation Matrix**: Visualized using a heatmap to show correlations between numerical variables.

### Multivariate Analysis
- **Survival Rate by Class and Sex**: Visualized using a bar plot to show survival rates segmented by passenger class and sex.

## Key Findings
1. **Age Distribution**: The age distribution of passengers is skewed towards younger ages, with a median age around 28.
2. **Survival Count**: More passengers did not survive the Titanic disaster than those who did.
3. **Age vs Fare**: There is no strong linear relationship between age and fare.
4. **Correlation Analysis**: 
   - `Pclass` is negatively correlated with `Survived`, indicating that passengers in higher classes had higher survival rates.
   - `Fare` is positively correlated with `Survived`, suggesting that passengers who paid higher fares were more likely to survive.
5. **Survival by Class and Sex**:
   - Women had higher survival rates compared to men across all classes.
   - Passengers in first class had the highest survival rates, followed by second class, with third class having the lowest survival rates.

## Conclusion
The data cleaning and EDA of the Titanic dataset provided valuable insights into the factors affecting passenger survival. Key findings highlight the impact of passenger class and sex on survival rates. These insights could be further explored using machine learning models to predict survival based on passenger characteristics.
