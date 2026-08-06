# __Companies Project - R__

Analyzed a data set with 5012 companies and 14 variables in R. Used basic statistical analysis to figure out if the data was normal and to find outliers. Used principal component analysis to reduce variables and find patterns. Used clusters to create different groups and find out what the companies in every group have in common. Finally, used linear discriminant analysis to find out how distinct each group was from one another. Found that most companies try to grow by either hiring a lot of employees and making risky moves to grow the company fast, or by slowly increasing revenue over time and not taking any super risky moves. 

---

## Table of Contents
- [Introduction](#Introduction)
- [Data Set](Data-Set)
- [Basic Analysis](#Basic-Analysis)
- [Principal Component Analysis](#Principal-Component-Analysis)
- [Clustering](#Clustering)
- [Linear Discriminant Analysis](#Linear-Discriminant-Analysis)
- [Conclusion](#Conclusion)

---

## Introduction



---

## Data Set

### [Data Set](../data/INC+5000+Companies+2019.csv.zip)

For this statistical analysis project using R, I used a data set called INC.5000.Companies.2019. This data set includes 5012 companies and 14 variables recorded in 2019. The most important variables include revenue, growth, workers, previous workers, and what year it was founded. Before starting any statistical analysis, this data set had a couple of problems. It had some columns where there were a bunch of extra characters after the column name, like “growth_...”. To fix this, I had to replace that column name with its normal name growth. Another issue I had was that the revenue column was written out as 40 million. This was an issue because it was a numeric column with the word million or billion in it. As a result, I had to change it so it would be written down in millions but without the wording. For example, 34 million would be 34 or 1.5 billion would be 1500. I also had to exclude all columns that were not numeric. I did this by creating a new data set called companies_numeric. After that I had to make sure there were no Null values, so I made another data set using companies_numeric and made companies_clean. This was the fully cleaned version of the original data set that was used for this statistical analysis. 

---

## Basic Analysis



---

## Principal Component Analysis



---

## Clustering



---

## Linear Discriminant Analysis



---

## Conclusion
