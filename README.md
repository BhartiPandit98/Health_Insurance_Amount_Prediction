# Health Insurance Amount Prediction: Project Overview
- Created a tool that estimates the health insurance amount to person to get an idea about the necessary amount required according to their own health status which they can use while complying with any health insurance company.
- Scarped over 1300 demographics data

# Code and Resources Used
- Python Version: 3.7
- Packages: Numpy, pandas, matplotlib, seaborn
- Scraper data: https://github.com/BhartiPandit98/Health_Insurance_Amount_Prediction/blob/main/insurance.csv

# Dataset Description:
- Age - Age of primary beneficiary
- Sex - Primary beneficiary’s gender
- BMI - Body mass index
- Children - No of dependents
- Smoker - Smoking (yes, no)
- Region - Beneficiary’s residential area in the US (northeast, southeast, southwest, northwest)
- Charges - Individual medical costs billed by health insurance

# Data Cleaning
After scraping the data, I needed to clean it up so that it was usable for our model. I made the following changes:
- Converted the categorical variables to dummy variable
- Normalized the data
- Removed outliers

# EDA
I looked at the distributions of the data and the value counts for the various categorical variables. Below are a few highlights:

![alt](https://github.com/BhartiPandit98/Health_Insurance_Amount_Prediction/blob/main/Box%20Plot.JPG)

![alt](https://github.com/BhartiPandit98/Health_Insurance_Amount_Prediction/blob/main/Scatterplot.JPG)

![alt](https://github.com/BhartiPandit98/Health_Insurance_Amount_Prediction/blob/main/Charge%20Distribution.JPG)

# Model Building
 First I split the data into train and tests sets with a test size of 20%.
 
 I tried two different models and evaluated them using R-Squared:
 
 - Multiple Linear Regression - R2-Score = 0.76
 - Polynomial Regression - R2-Score = 0.85
