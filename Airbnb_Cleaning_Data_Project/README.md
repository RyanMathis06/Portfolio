# __Airbnb Data Cleaning Project__

Cleaned an Airbnb data set containing 102,599 rows and 26 columns using Pandas. The data set includes Nulls, True/False, lowercase and uppercase, columns that were not needed, and symbols. Removed 8 columns and around 3,000 rows after cleaning the data set. 

---

## Table of Contents
- [Introduction](#Introduction)
- [Dropping Columns](#Dropping-Columns)
- [Renaming Columns](#Renaming-Columns)
- [Duplicates](#Duplicates)
- [Nulls](#Nulls)
- [Cleaning Data](#Cleaning-Data)
- [Conclusion](#Conclusion)

---

## Introduction

![Executive Dashboard](../Images/Airbnb_clean_OG.png)
Found this Airbnb data off of Kaggle, wanted to test my ability to clean data properly using pandas. First I imported pandas as pd and then imported my data set as data. After that I did data.head() to ensure it was the correct data and so that I could see exactly what I needed to change. Looking at this image shows me that I need to get rid of $, some columns are all capitalized and others are not, and I see Nulls. 
![Executive Dashboard](../Images/Airbnb_clean1.png)

---

## Dropping Columns

![Executive Dashboard](../Images/Airbnb_clean2.png)
First I looked at all the column names and then I looked to see how many null values each column had. 
![Executive Dashboard](../Images/Airbnb_clean3.png)
I noticed that the column 'License,' only had 2 non-null values and the column 'house_rules' had over 50,000 nulls, therefore I dropped those column as they are basically useless. 
![Executive Dashboard](../Images/Airbnb_clean4.png)
Then I created 2 lists of columns to keep and columns to drop. I dropped the column 'id' because it has no analytical value as it is just an identifier code that distinguishes rows. I dropped 'reviews per month' and 'review rate number' because they are redundant review columns considering I am keeping 'number of reviews' and 'last review.' I dropped 'calculated host listings count' because it is redundant with the other host columns that I kept. And finally I dropped 'availability 365' because it could contain extreme outliers as it could be available 0 days or 365 days. 
![Executive Dashboard](../Images/Airbnb_clean5.png)
Then I made df my data set without the dropped columns. 

---

## Renaming Columns

![Executive Dashboard](../Images/Airbnb_clean6.png)
![Executive Dashboard](../Images/Airbnb_clean7.png)
---

## Duplicates



---

## Nulls



---

## Cleaning Data



---

## Conclusion
