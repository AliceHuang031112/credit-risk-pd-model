{\rtf1\ansi\ansicpg1252\cocoartf2761
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx566\tx1133\tx1700\tx2267\tx2834\tx3401\tx3968\tx4535\tx5102\tx5669\tx6236\tx6803\pardirnatural\partightenfactor0

\f0\fs24 \cf0 # Credit Risk Modeling \'96 Probability of Default Framework\
\
## Overview\
This project develops a Probability of Default (PD) model using historical consumer loan data from LendingClub (2007\'962015). The objective is to build a structured risk modeling workflow that demonstrates data cleaning, leakage prevention, probability modeling, and risk segmentation.\
\
## Dataset\
- Original dataset: 2.2M+ consumer loans\
- Filtered to finalized loans only: Fully Paid / Charged Off\
- Modeling sample: 120,000 loans\
- Target variable: binary default indicator\
\
## Methodology\
The project follows a realistic credit risk modeling process:\
- Filtered to loans with known final outcomes\
- Removed post-origination variables to prevent data leakage\
- Selected features based on underwriting logic, including:\
  - loan characteristics\
  - borrower capacity\
  - credit history\
  - stability indicators\
- Built a logistic regression PD model using a preprocessing pipeline with:\
  - imputation\
  - scaling\
  - one-hot encoding\
\
## Model Performance\
- ROC-AUC: 0.70\
- KS Statistic: 0.29\
\
## Risk Segmentation\
Borrowers were grouped into risk deciles using predicted default probability.  \
Observed default rates increased monotonically across deciles:\
\
- Lowest-risk decile: 4.9%\
- Highest-risk decile: 45.4%\
\
This indicates that the model meaningfully separates lower-risk and higher-risk borrowers.\
\
## Key Takeaways\
This project demonstrates:\
- credit risk modeling\
- probability of default estimation\
- model validation using ROC-AUC and KS\
- threshold trade-off analysis\
- risk segmentation\
- data leakage prevention\
\
## Tools\
- Python\
- pandas\
- scikit-learn\
- matplotlib\
\
## Notes\
The raw LendingClub data is not uploaded to this repository due to file size constraints.  \
Please place the downloaded zip file in the working directory before running the notebook.}