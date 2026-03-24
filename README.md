# Credit Risk Modeling – Probability of Default (PD) Framework

## Overview
This project develops a Probability of Default (PD) model using historical consumer loan data from LendingClub (2007–2015). The objective is to build a structured risk modeling workflow that demonstrates data cleaning, leakage prevention, probability modeling, and risk segmentation.

## Dataset
- Original dataset: 2.2M+ consumer loans  
- Filtered to finalized loans only: Fully Paid / Charged Off  
- Modeling sample: 120,000 loans  
- Target variable: binary default indicator  

## Methodology
The project follows a realistic credit risk modeling process:

- Filtered to loans with known final outcomes  
- Removed post-origination variables to prevent data leakage  
- Selected features based on underwriting logic:  
  - loan characteristics  
  - borrower capacity  
  - credit history  
  - stability indicators  
- Built a logistic regression PD model using a preprocessing pipeline  

## Model Performance
- ROC-AUC: 0.70  
- KS Statistic: 0.29  

## Risk Segmentation
Borrowers were grouped into risk deciles using predicted default probability.  

Default rates increase monotonically:

- Lowest-risk decile: 4.9%  
- Highest-risk decile: 45.4%  

This confirms strong risk separation.

## Skills Demonstrated
- Credit risk modeling  
- Logistic regression  
- Model validation (ROC, KS)  
- Risk segmentation  
- Threshold optimization  
- Data leakage prevention  

## Tools
- Python  
- pandas  
- scikit-learn  
- matplotlib  

## Note
The raw dataset is not uploaded due to file size.  
Please download the LendingClub dataset and place the zip file in the working directory before running the notebook.
