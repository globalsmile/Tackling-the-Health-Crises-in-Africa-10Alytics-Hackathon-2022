# Tackling the Health Crises in Africa - 10Alytics Hackathon 2022
<img align="right" alt="Twitter Sentiment Analysis" width="1000" height = "400" src="https://user-images.githubusercontent.com/106287208/187567112-ec593f73-7afe-4ef3-8c80-822591b89038.png">

---


# Table of Contents

- [Problem Statement](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Problem-Statement)
- [Data Sourcing](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Data-Sourcing)
- [Data Preparation](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Data-Preparation)
- [Data Modeling](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Data-Modeling)
- [Data Visualization and Analysis](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Data-Visualization)
- [Recommendations](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Recommendation)
- [Shareable link](https://github.com/globalsmile/Tackling-the-Health-Crises-in-Africa-10Alytics-Hackathon-2022#Shareable-Link)


---

# Problem Statement

The lack of access to adequate medical resources and facilities have led to the significant number of deaths. 
Some of these deaths could have been avoided by timely access to a medical professional or close proximity of hospitals.
Health systems across Africa are underfunded and understaffed. Less than half of African citizens (52%) `about 615 million people`
have access to the health care they need, the quality of health services across the continent is generally poor, and family planning 
needs of half the continent’s women and girls are unmet.

The main focus is on Africa in this dataset and the purpose of this analysis is to provide solutions to the health challenges, especially in Africa. 

---

# Data Sourcing

The Dataset used for this analysis was provided by [10Alytics](https://10alytics.io/) and is available at:

- [10Alytics](https://10alytics.io/)

---

# Data Preparation

Data cleaning and transformation was done in Microsoft Excel and the datasets were loaded into Microsoft Power BI Desktop for modeling and visualization.

There are six datasets for this project.:

- Causes of Deaths: The number of deaths and the causes across different countries from 1990 to 2019
- Number of Deaths by Age Group: Medical Doctors Per 10,000 population: Number of medical doctors per 10,000 medical practitioners in Africa
- ISO 3166_country-and-continent-codes-list-csv: The list of sovereign states and dependent territories by continent describing the list of countries by continent
- World Population: Data from the UN Population Division provides consistent and comparable estimates (and projections) within and across countries over the last century
- Health Expenditure (% of GDP): Countries expenditure on health as a percentage of GDP

The data dictionary containing the features of the data can be found below:

- `Causes of Deaths`

| Fields | Description |
| ----------- | ----------- |
| Entity | Countries |
| Code | ISO-3166 Codes |
| Year | Year |
| Number of executions (Amnesty International) | People that die due to executions |
| Meningitis | People that died due to Meningitis |
| Alzheimer's disease and other dementias | People that died due to Alzheimer's disease and other dementias |
| Parkinson's disease | People that died due to Parkinson's disease |
| Nutritional deficiencies | People that died due to Nutritional deficiencies |
| Malaria | People that died due to Malaria |
| Drowning | People that died due to Drowning |
| Interpersonal violence | People that died due to Interpersonal violence |
| Maternal disorders | People that died due to Maternal disorders |
| HIV/AIDS | People that died due to HIV/AIDS |
| Drug use disorders| People that died due to Drug use disorders |
| Tuberculosis |  People that died due to Tuberculosis |
| Cardiovascular diseases | People that died due to Cardiovascular diseases |
| Lower respiratory infections | People that died due to Lower respiratory infections |
| Neonatal disorders | People that died due to Neonatal disorders |
| Alcohol use disorders| People that died due to Alcohol use disorders |
| Self | People that died due to Self |
| Exposure to forces of nature | People that died due to Exposure to forces of nature |
| Diarrheal diseases | People that died due to Diarrheal diseases |
| Environmental heat and cold exposure | People that died due to Environmental heat and cold exposure |
| Neoplasms | People that died due to Neoplasms |
| Conflict and terrorism | People that died due to Conflict and terrorism |
| Diabetes mellitus | People that died due to Diabetes mellitus |
| Chronic kidney disease | People that died due to Chronic kidney disease |
| Poisonings | People that died due to Poisonings |
| Protein | People that died due to Protein |
| Terrorism (deaths) | People that died due to Terrorism (deaths) |
| Road injuries | People that died due to Road injuries |
| Chronic respiratory diseases | People that died due to Chronic respiratory diseases |
| Cirrhosis and other chronic liver diseases | People that died due to Cirrhosis and other chronic liver diseases |
| Digestive diseases | People that died due to Digestive diseases |
| Fire, heat, and hot substances | People that died due to Fire, heat, and hot substances |
| Acute hepatitis | People that died due to Acute hepatitis |

- `Number of Deaths by Age Group`

| Fields | Description |
| ----------- | ----------- |
| Entity | Countries |
| Code | ISO-3166 Codes
| Year | Year |
| Deaths 70+ years | Population above 70 years old |
| Deaths 50 - 69 years | Population between 50 - 69 years old |
| Deaths 15 - 49 | Population between 15 - 49 years old |
| Deaths 5 - 14 years | Population between 5 - 14 years old |
| Deaths Under 5 | Population under 5 years old |

- `Medical Doctors Per 10,000 population`

| Fields | Description |
| ----------- | ----------- |
| IndicatorCode | Unique Codes for Indicators |
| Indicator | Medical Practitioners Indicators |
| ParentLocationCode | Codes for the Regions |
| ParentLocation | Regions |
| ThreeLocCode | ISO-3166 Codes |
| Location | Countries |
| Period | Year |
| FactValueNumeric | Number of Doctors |
|Value | Number of Doctors |

- `ISO 3166_country-and-continent-codes-list-cs`

| Fields | Description |
| ----------- | ----------- |
| Continent_Name | Name of Countries |
| Continent_Code | ISO-3166 Continent Code |
| Country_Name | ISO-3166 Country Code |
| Two_Letter_Country_Code | ISO-3166 2-letter Country Code |
| Three_Letter_Country_Code | ISO-3166 3-letter Country Code |
| Country_Number | ISO-3166 number Country Code |

- `World Population`

| Fields | Description |
| ----------- | ----------- |
| Entity | Countries |
| Code | ISO-3166 Codes |
| Year | Year |
| Population (historical estimates) | Population Estimate |

- `Health Expenditure (% of GDP)`

| Fields | Description |
| ----------- | ----------- |
| Country Name | Name of the country |
| Country Code | ISO-3166 Country Codes |
| Indicator Name | Name of the Indicator |
| 2000 | % of GDP in 2000 |
| 2001 | % of GDP in 2001 |
| 2002 | % of GDP in 2002 |
| 2003 | % of GDP in 2003 |
| 2004 | % of GDP in 2004 |
| 2005 | % of GDP in 2005 |
| 2006 | % of GDP in 2006 |
| 2007 | % of GDP in 2007 |
| 2008 | % of GDP in 2008 |
|2009 | % of GDP in 2009 |
| 2010 | % of GDP in 2010 |
| 2011 | % of GDP in 2011 |
| 2012 | % of GDP in 2012 |
| 2013 | % of GDP in 2013 |
| 2014 | % of GDP in 2014 |
| 2015 | % of GDP in 2015 |
| 2016 | % of GDP in 2016 |
| 2017 | % of GDP in 2017 |
| 2018 | % of GDP in 2018 |
| 2019 | % of GDP in 2019 |

The `Causes of Deaths` datasets was checked for duplicates, invalid entries, missing values, incorrect data types and issues from data entry.

For numeric columns that had null values, I replaced them with ‘0’. No duplicates were found, and incorrect column data types were 
changed to the appropriate data types, e.g. date column having a number data type was changed to the date data type. 
The same process was repeated for all 5 remaining datasets to ensure accuracy in analysis.

---

# Data Modeling

After the dataset was cleaned and transformed, it was ready to be modeled(using Power BI Desktop).

- A `one-to-many (*:1) relationship` was created between the `Budget` and the `Calender` tables using the `date` column in each of the tables
- A `one-to-many (*:1) relationship` was created between the `Transactions` and the `Calender` tables using the `date` column in each of the tables 
- A `one-to-many (*:1) relationship` was created between the `Transactions` and the `Categories` tables using the `Category` column in each of the tables
- A `one-to-many (*:1) relationship` was created between the `budget` and the `Categories` tables using the `Category` column in each of the tables 
- The realtioships formed in the data model is a `Star Schema` and is shown below:

<img align="right" alt="Data Model" width="1000" height = "400" src="https://user-images.githubusercontent.com/106287208/188418211-26dbee49-71c9-4fef-b767-279d6d4d67cc.png">


---

# Data Visualization and Analysis

Data visualization for the datasets was done in 3 folds using Microsoft Power BI Desktop:

- The `Sales Overview`: Shows the sales vs budget KPI, sales by top 10 customers, sales by top 10 products, e.t.c
-  The `Customer Details`: Shows customer specific information
-  The `Product Details`: Shows product specific information


Figure 1 shows visualizations from `Sales Overview` page

| Figure 1 |
| ----------- |
| ![image](https://user-images.githubusercontent.com/106287208/188423026-e1b4d76d-ffcc-4f8c-a1b7-bd363922f524.png) |

Figure 2 shows visualizations from `Customer Details` page

| Figure 2 |
| ----------- |
| ![image](https://user-images.githubusercontent.com/106287208/188423353-266e6a75-d31a-4f2e-ba1d-30dd1f591050.png) |

Figure 3 shows visualizations from `Product Details` page

| Figure 3 |
| ----------- |
| ![image](https://user-images.githubusercontent.com/106287208/188423526-fe1c6dd3-73da-4f8f-b757-5d585be1eec3.png) |

---

# Recommendations

Measures used in visualization are:

- Budget = `SUM ( FACT_Budget[Budget] )`
- Sales = `SUM ( FACT_InternetSales[SalesAmount] )`
- Sales / Budget = `[Sales] - [Budget]`


As shown from [Data Visualization](https://github.com/globalsmile/Sales-Management-Analysis#Data-Visualization), It can be deducted that for the year ending December 2021:

- Sales is up by `1,051,550`
- The top customer by sales is `Jordan Turner`
- The top product by sales is `Mountain-200 Black,42`
- The top product category by sales is the `Bikes` occupying 93.93% of the total sales
- There is a positive correlation between `Sales` and `Budget`

---

# Shareable Link

You can interact with the report here: 

[View Report](https://app.powerbi.com/view?r=eyJrIjoiNWVmNDRjNjEtNjZjZC00OGE2LTllYjktMDRjMmMyOTE4ZDYxIiwidCI6IjQ5ODY4YWYzLWNjNWYtNDIxNC04YjdmLTQwZjM3NDY0OWEwOSJ9)
