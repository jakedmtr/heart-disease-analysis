# Heart Disease Analysis

The analysis and Excel workbook in this repository are licensed under the MIT License. The underlying dataset is sourced from Kaggle and remains subject to its original license and terms.

## Overview

An analysis using of heart disease patients using Microsoft Excel. Here I investigated which attributes show a correlation with heart disease.

## Dataset

The data set I used is from Kaggle: https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?resource=download

In the original data there were 1025 data points but 723 of them were duplicates, leaving only 302 unique data points.

This data set dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It contains 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 13 of them. The "target" field refers to the presence of heart disease in the patient. I removed the 'ca' attribute (number of major vessels coloured by fluoroscopy) as I didn't use it in my analysis, which brings down the number of columns to 13.

Attribute documentation (13 attributes in total including 'target'):
      
      1 age: age in years
      
      2 sex: sex (1 = male; 0 = female)
      
      3 cp: chest pain type
        -- Value 1: typical angina
        -- Value 2: atypical angina
        -- Value 3: non-anginal pain
        -- Value 4: asymptomatic
        
      4 trestbps: resting blood pressure (in mm Hg on admission to the hospital)
      
      5 chol: serum cholestoral in mg/dl
      
      6 fbs: (fasting blood sugar > 120 mg/dl)  (1 = true; 0 = false)
      
      7 restecg: resting electrocardiographic results
        -- Value 0: normal
        -- Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
        -- Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
        
      8 thalach: maximum heart rate achieved
      
      9 exang: exercise induced angina (1 = yes; 0 = no)
      
     10 oldpeak = ST depression induced by exercise relative to rest
     
     11 slope: the slope of the peak exercise ST segment
        -- Value 1: upsloping
        -- Value 2: flat
        -- Value 3: downsloping
        
     12 thal: 1 = normal; 2 = fixed defect; 3 = reversible defect
     
     13 target: diagnosis of heart disease; 0 = no disease and 1 = disease.

## Objectives

- Investigate demographic patterns in heart disease
- Analyse relationships between clinical variables and heart disease
- Compare patients with and without heart disease
- Identify notable patterns in the dataset

## Data Cleaning

- I checked for missing values; fortunately there were none.
- I checked for duplicate records; as mentioned above there were 723 duplicates recorded and purged.
- Invalid values?
- Data types?
- Categorical consistency?

## Exploratory Data Analysis

### Age

Explain what you found about age and heart disease.

![Age analysis](images/age_analysis.png)

### Sex

Explain what you found about sex and heart disease.

![Sex analysis](images/sex_analysis.png)

### Cholesterol

Explain what you found about cholesterol.

### Chest Pain

Explain what you found about chest-pain categories.

## PivotTable Analysis

Explain how PivotTables were used to investigate relationships between variables.

## Key Findings

1. ...
2. ...
3. ...

## Limitations

- Dataset limitations
- Sample size/composition
- Observational nature of the data
- Association does not imply causation

## Excel Workbook

The complete Excel analysis is available here:

`excel/heart_disease_analysis.xlsx`

## Tools

- Microsoft Excel
- PivotTables
- Excel formulas
- Charts
