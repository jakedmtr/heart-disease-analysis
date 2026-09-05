# Heart Disease Analysis

The dataset is sourced from Kaggle here: https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?resource=download which is originally sourced from https://archive.ics.uci.edu/dataset/45/heart+disease.

## Overview

An analysis of heart disease patients using Microsoft Excel. Here I investigated which attributes show a correlation with heart disease.

The initial analysis used a publicly available Kaggle version of the Heart Disease dataset. During data validation, substantial duplication and differences in target encoding were identified. The original UCI Cleveland dataset was subsequently obtained and used to produce a second analysis based on the original source data. Both analyses are retained to demonstrate how dataset quality and preprocessing decisions can affect exploratory analysis.

## Dataset

The original Kaggle dataset contained 1,025 records, but investigation revealed substantial duplication. Duplicate records (723) were removed before analysis. The dataset also used an inverted binary target relative to the original UCI definition, so the target variable was re-encoded such that 0 represents absence of heart disease and 1 represents presence of heart disease. Variable encodings were checked against the original UCI Cleveland Heart Disease dataset. The original data set dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach VA and it contained 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 14 of them. However, only the Cleveland dataset is complete and processed as the other 3 databases contain missing values. The Kaggle data set seems to just use the Cleveland dataset but duplicated to increase the number of data points, which is very bad practice. I noticed during my project that the relationships seemed odd so I investigated and then found out the above information. So now I have instead just used the original processed Cleveland dataset (`/data/cleveland_data.data`) but have left the altered Kaggle version for comparison (`/data/kaggle_data.csv`).

The "target" field refers to the presence of heart disease in the patient. The original data set used the values 0-4 where 0 signified no heart disease and values 1-4 appear to signify different degrees of the possibility of a patient having heart disease, with 4 being the highest. The author of the Kaggle data set re-encoded all rows with values 1-4 to just be 1 and then also (probably by mistake) inverted the target field, such that patients who didn't have heart disease seemingly had it, and vice-versa.

I removed the 'ca' field (number of major vessels coloured by fluoroscopy) and the 'oldpeak' field (ST depression induced by exercise relative to rest) as I didn't use them in my analysis, which brings down the total number of columns to 12.

Attribute documentation (12 attributes in total including 'target'):
      
      1 age: age in years

      2 sex: sex (1 = male; 0 = female)
      
      3 cpt: chest pain type
        -- Value 1: typical angina
        -- Value 2: atypical angina
        -- Value 3: non-anginal pain
        -- Value 4: asymptomatic
        
      4 restbps: resting blood pressure (in mm Hg on admission to the hospital)
      
      5 chol: serum cholesterol in mg/dl
      
      6 fbs: (fasting blood sugar > 120 mg/dl)  (1 = true; 0 = false)
      
      7 restecg: resting electrocardiographic results
        -- Value 0: normal
        -- Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV)
        -- Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
        
      8 maxhr: maximum heart rate achieved (bpm)
      
      9 exang: exercise induced angina (1 = yes; 0 = no)
     
     10 slope: the slope of the peak exercise ST segment
        -- Value 1: up-sloping
        -- Value 2: flat
        -- Value 3: down-sloping
        
     11 thal: 1 = normal; 2 = fixed defect; 3 = reversible defect
     
     12 target: diagnosis of heart disease; 0 = no disease and 1 = disease.

## Objectives

- Investigate demographic patterns in heart disease
- Analyse relationships between clinical variables and heart disease
- Compare patients with and without heart disease
- Identify notable patterns in the dataset

## Excel Workbook

The complete Excel analysis is available here: `/excel/cleveland_heart_disease_analysis.xlsx`.

## Tools

- Microsoft Excel
- PivotTables
- Excel formulas
- Charts
