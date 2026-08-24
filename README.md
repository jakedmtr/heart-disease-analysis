# heart-disease-analysis
An analysis using Excel of heart disease patients from the https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset?resource=download dataset.

The analysis and Excel workbook in this repository are licensed under the MIT License. The underlying dataset is sourced from Kaggle and remains subject to its original license and terms.

--------------------------------------------------------------------------------------------------------------

File breakdown:

* heart_disease.csv - The original data
* heart_disease.xlsx - My edited Excel spreadsheet

--------------------------------------------------------------------------------------------------------------
This data set dates from 1988 and consists of four databases: Cleveland, Hungary, Switzerland, and Long Beach V. It contains 76 attributes, including the predicted attribute, but all published experiments refer to using a subset of 13 of them. The "target" field refers to the presence of heart disease in the patient. I removed the 'ca' attribute (number of major vessels coloured by fluoroscopy) as I didn't use it in my analysis, which brings down the number of columns to 13.

Attribute documentation (12 attributes in total):
      
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
