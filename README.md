# Python_Coding
Python Coding related resources

Python vs. SAS
https://github.com/asnr/sas-to-python

Python version: python -V

Xgboost install: pip3 install xgboost

Pip update: pip install --upgrade pip

Pip on Jupyter Note Book:
## Install a pip package in the current Jupyter kernel
import sys
!{sys.executable} -m pip install xyz
  - xyz could be "numpy" or "shap"
  
# Missing Value Treatments

## Treating the missing values of education as a separate category
data['education'] = data['education'].replace(np.NaN, 'NA')
## Treating the missing values of previous year rating as 0
data['previous_year_rating'] = data['previous_year_rating'].fillna(0)
## Replace missings by median
dataMasterX = dataMasterX.fillna(dataMasterX.median())

# Convert Object Vars to Numeric Type
dataMasterX = dataMasterX.astype(float)


