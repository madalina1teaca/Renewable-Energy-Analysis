# Exploratory Data Analysis on Global Renewable Energy and Indicators Dataset

## 1. Introduction

### 1.1 Dataset Description
The **Global Renewable Energy and Indicators dataset** obtained from Kaggle contains comprehensive information on various aspects of renewable energy production and its related indicators globally. It includes data on energy production, installed capacity, economic indicators, environmental factors, and much more, spanning multiple years and covering numerous countries and regions.

#### Key Columns
- **Country**: The country for which the data is reported.
- **Year**: The year of the data entry.
- **Energy Type**: The type of energy (e.g., solar, wind, hydro).
- **Production (GWh)**: The amount of energy produced (in gigawatt hours).
- **Installed Capacity (MW)**: The installed capacity of renewable energy sources (in megawatts).
- **Investments (USD)**: Investments made in renewable energy (in USD).
- **Population**: The population of the country.
- **GDP**: Gross Domestic Product of the country (in USD).
- **Energy Consumption**: Total energy consumption.
- **Energy Exports**: Energy exported by the country.
- **Energy Imports**: Energy imported by the country.
- **CO2 Emissions**: CO2 emissions from the country (in metric tons).
- **Renewable Energy Jobs**: Number of jobs in the renewable energy sector.
- **Government Policies**: Policies promoting renewable energy.
- **R&D Expenditure**: Expenditure on research and development in renewables.
- **Renewable Energy Targets**: National targets for renewable energy adoption.

### 1.2 Objectives of the Analysis
The primary objective of this exploratory data analysis (EDA) is to understand the distribution, relationships, and patterns within the dataset. The analysis aims to:
- Identify trends in renewable energy production, installed capacity, and investments over time and across different regions.
- Investigate relationships between renewable energy production and economic indicators (e.g., GDP, investments).
- Examine the influence of environmental factors on renewable energy production.
- Explore correlations between renewable energy policies, R&D expenditure, and production capacity.
- Analyze the impact of socio-economic factors on renewable energy adoption.
- Identify outliers or anomalies in the data and provide actionable insights based on findings.

### 1.3 Key Questions
During the analysis, we seek to answer critical questions related to:
- Trends in renewable energy production and investments over time.
- The correlation between GDP and renewable energy production.
- Regional differences in renewable energy production and investments.
- The impact of environmental and climatic factors on production.
- The effects of government policies and socio-economic factors on renewable energy adoption.

## 2. Data Loading and Initial Examination

### 2.1 Loading the Data
The dataset is loaded using Pandas for analysis, and basic examination of the structure, data types, and summary statistics is conducted to understand the dataset.

```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

# Loading the dataset
df = pd.read_csv('Data/complete_renewable_energy_dataset.csv')

# Displaying the first few rows
df.head()
```

### 2.2 Initial Examination
- The shape and structure of the dataset are checked.
- Summary statistics for both numerical and categorical columns are computed, providing insights into the data's characteristics.

### 2.3 Initial Visualization
Histograms and count plots are created to visualize the distribution of key numerical and categorical variables.

## 3. Data Cleaning

### 3.1 Handling Missing Values
The dataset is checked for missing values, and appropriate actions are taken (in this case, there are no missing values).

### 3.2 Handling Outliers
Outliers are identified and removed using Z-scores to maintain data integrity.

## 4. Univariate Analysis
Histograms and KDE plots are generated for numerical variables, and bar charts are created for categorical columns to explore their distributions.

## 5. Bivariate and Multivariate Analysis

### 5.1 Relationships Between Two Variables
Scatter plots and box plots are used to explore the relationships between key numerical variables, while also examining the impact of categorical variables.

### 5.2 Multivariate Relationships
Correlation matrices and pair plots provide insights into the relationships between several variables simultaneously.

## 6. Further Look into the Data
Bar plots are generated to visualize the total production, installed capacity, and investments by country.

## 7. Summary of Findings

### 7.1 Trends and Patterns
The analysis identifies increasing trends in renewable energy production and investments, particularly in countries that invest in renewable energy infrastructure.

### 7.2 Relationships and Correlations
- Strong correlations are found between installed capacity and production, as well as between investments and installed capacity.
