
# Data Quality Analysis – UCI Adult Income Dataset
# Overview:

This project explores real-world data quality issues using the UCI Adult Income Dataset, a well-known dataset used to predict whether a person earns more than $50,000 per year. The purpose of this project is to apply data quality concepts from Week 10 (Data Warehousing & ETL) and Week 11 (Data Mining & Bias) from COMP 331 and demonstrate how poor data quality can affect machine learning results.

The analysis focuses on three major data quality dimensions:

1. Completeness (Missing Data)

2. Consistency (Formatting & Value Issues)

3. Bias & Fairness (Sensitive Attributes)

All of the analysis was performed using Microsoft Excel, focusing on manual inspection and real data examples.

# Objectives:

The main goals of this project are to:

- Identify real data quality problems in a commonly used machine learning dataset

- Apply ETL standardization rules and CRISP-DM data preparation concepts

- Analyze bias and fairness risks in training data

- Propose practical and realistic data cleaning recommendations

# Dataset Information: 

Source: UCI Machine Learning Repository

Dataset Name: Adult Income Dataset

File Used: adult.data

Number of Records: ~32,000

Number of Attributes: 14 + 1 target label

Target Variable:

<=50K

>50K

This dataset represents census data and is commonly used in data mining and machine learning research.

# Tools:

Microsoft Excel (data inspection, filtering, and searching)

# Data Quality Dimension Analysis: 

1. Completeness (Missing Values)

   Missing values in the dataset are represented as "?"

   The most affected columns were:

   workclass
   
   occupation
   
   native-country
   
   A decent portion (between 7–10%) of the dataset contains missing values
   
   These missing values affect model accuracy and can introduce bias if not handled properly
   
2. Consistency (Formatting & Value Issues)
   
   Some categories are very similar but treated as separate values, such as:

   Self-emp-inc vs Self-emp-not-inc
   
   The education column mixes labels like:

   Bachelors, Masters, and also 11th, 9th

   capital-gain and capital-loss fields show:
   
   Many zero values
   
   A few extremely large outliers
   
   these issues violate ETL standardization rules from Week 10 and make preprocessing more difficult

3. Bias & Fairness
   
   The high-income class (>50K) is dominated by male records
   
   The dataset is heavily skewed toward individuals labeled as White
   
   Sensitive attributes such as sex and race introduce:
   
   Historical bias
   
   Sampling bias
   
   These issues relate directly to Week 11 topics on fairness and ethical data mining 

# Real Data Examples

Actual records from the dataset were used in the project to provide clear, real examples of:

Inconsistencies in workclass and education

Skewed demographic representation

Zero-heavy numerical fields like capital-gain and capital-loss


# Project Files Included

adult.data – Original raw dataset

Adult_Data_Quality_Presentation_Updated.pptx – Final presentation

Project Report (PDF submission)

README.md – Project documentation

# Author: 
Fuzail Chaugle-300196602



