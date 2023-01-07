# Tackling the Health Crises in Africa - 10Alytics Hackathon 2022
<img align="right" alt="Tackling the Health Crises in Africa - 10Alytics Hackathon 2022" width="1000" height = "500" src="https://miro.medium.com/max/720/0*yq9oNi9a9MpDRqNi.webp">

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

- [10Alytics hackathon 2022 datasets](https://drive.google.com/drive/folders/1_pPCjVLhIA8_pn5LFSIzMcvjFXT15oM7?usp=share_link)

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

- A `one-to-many (*:1) relationship` was created between the `Causes of Deaths` and the `Country` tables using the `CountryID` column in each of the tables
- A `one-to-many (*:1) relationship` was created between the `Number of Deaths by Age Group` and the `Country` tables using the `CountryID` column in each of the tables 
- A `one-to-many (*:1) relationship` was created between the `Medical Doctors` and the `Country` tables using the `CountryID` column in each of the tables
- A `one-to-many (*:1) relationship` was created between the `Country GDP` and the `Country` tables using the `CountryID` column in each of the tables 
- A `one-to-many (*:1) relationship` was created between the `World Population` and the `Country` tables using the `CountryID` column in each of the tables 

The realtioships formed in the data model is a `Star Schema` and is shown below:

<img align="right" alt="Data Model" width="1000" height = "400" src="https://user-images.githubusercontent.com/106287208/211148517-aa46241c-140e-41e3-a64b-ae6d01c30f2f.png">



---

# Data Visualization and Analysis

- The analysis aimed to determine the factors contributing to the health crisis being experienced in Africa which has sadly led to the death of millions of people (both young and old).

To achieve this set goal:-

I created a visualization showing the trend of deaths in Africa from 1990 to 2019 (the year range provided in the datasets). The visual showed that The total number of deaths increase annually. However more people died in 2004(over 9M deaths or 3.64% of total deaths) than in any other year.

![image](https://user-images.githubusercontent.com/106287208/211149892-465fc0b1-e2cf-43a8-bd03-1e4f2960a052.png)


- To determine the African countries with the highest number of deaths resulting from health crises, I used a column chart to show top 10 African countries with the highest deaths record. From this Analysis, Nigeria has the highest prevalence of health crisis in Africa with over 49M death cases which contributes 9.80% to the total # of deaths (app. 259M) in Africa.

![image](https://user-images.githubusercontent.com/106287208/211150389-df6b6a7d-5d52-4e94-ab19-0008888f08e5.png)



- A bar chart representation showed the diseases leading to the most deaths in Africa. With over 33 factors responsible for the death of Africans annually, cardiovascular diseases are the leading cause. Contributing over 33M deaths to the total number of deaths in Africa.

![image](https://user-images.githubusercontent.com/106287208/211150214-c13700a7-3be7-4b49-a69a-76cff35d614f.png)


- Further analysis of 5 different age grades showed that children under 5 have suffered the most significant number of deaths (about 42.9% of total death)
due to the lack of access to adequate medical resources and facilities.

![image](https://user-images.githubusercontent.com/106287208/211150138-6edc20f2-fe4d-4121-bb5f-7d8e38028c1f.png)


- The health expenditures of different African countries were compared and the analysis showed that Sierra Leone had the highest health expenditure, whereas Nigeria with the highest number of deaths was missing in the top 10 countries with the highest health expenditures.

![image](https://user-images.githubusercontent.com/106287208/211150436-406280c8-2a77-4eb6-bfbb-e09808fdcd30.png)


- Nigeria and Algeria topped the list of countries with the highest number of medical doctors in the timeframe used in this analysis.

![image](https://user-images.githubusercontent.com/106287208/211150513-41883d06-ae1e-4121-b995-6ca40e019c73.png)



---

# Recommendations

Africa is the second most populated continent in the world and this puts it on the verge of losing more of its citizens if adequate infrastructures are not immediately put into place in its health sector. For countries like Nigeria with an increasing population, the budget in the health sector should be increased and medical facilities fully funded to enable access to medical resources by patients.

Much attention should be given to pregnant women to eliminate the chances of their newborns suffering from neonatal disorders and diarrhoea, which are among the leading causes of death in Africa.

Overall, brain drain and emigration of medical doctors should be minimized by offering them competitive salaries and ensuring that the working condition(hospitals) is adequately equipped, safe and conducive for both patients and doctors.

---

# Shareable Link

You can interact with the report here: 

[View Report](https://app.powerbi.com/view?r=eyJrIjoiMWI3MzYzMmQtNDBkMC00MWRhLTlmNjYtYTQ5MWYwOWFiNWVlIiwidCI6IjQ5ODY4YWYzLWNjNWYtNDIxNC04YjdmLTQwZjM3NDY0OWEwOSJ9)
