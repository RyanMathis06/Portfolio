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

For this statistical analysis on companies, I wanted to find what made these companies different
from each other. I wanted to find separate groups of companies and figure out why they were
grouped, what made them similar or different. I also wanted to figure out if there were any
outliers and why there were outliers.

---

## Data Set

### [Data](../data/INC+5000+Companies+2019.csv.zip)

Before I started, I had to analyze and clean up the data. I used a data set called INC.5000.Companies.2019. This data set includes 5012 companies and 14 variables recorded in 2019. The most important variables include revenue, growth, workers, previous workers, and what year it was founded. Before starting any statistical analysis, this data set had a couple of problems. It had some columns where there were a bunch of extra characters after the column name, like “growth_...”. To fix this, I had to replace that column name with its normal name growth. Another issue I had was that the revenue column was written out as 40 million. This was an issue because it was a numeric column with the word million or billion in it. As a result, I had to change it so it would be written down in millions but without the wording. For example, 34 million would be 34 or 1.5 billion would be 1500. I also had to exclude all columns that were not numeric. I did this by creating a new data set called companies_numeric. After that I had to make sure there were no Null values, so I made another data set using companies_numeric and made companies_clean. This was the fully cleaned version of the original data set that was used for this statistical analysis. 

---

## Basic Analysis

The first thing I did after cleaning my data was to figure out the sample mean vector of each variable. This helped me see how big or small the numbers were compared to one another. I then found the sample covariance matrix and the sample correlation matrix. I found the sample covariance matrix to see if it would be viable or not to use non-standardized data. I decided to use standardized data by figuring out the correlation matrix. 

![Executive Dashboard](../Images/Basic%20Analysis%20Graph.png)

This plot shows that the data I will be analyzing is not normal and is skewed to the right. I know this because if it was normal, it would follow the line, but at around the 20th chi-square quantile, the data points shoot vertically away from the line. It is skewed to the right because most of the points are clumped up in the bottom left, and only a few points are far in the upper right-hand corner. I can also tell that the data has a heavy tail since the points in the upper right corner reach 4000 ordered distances. As a result, they are enormous and far away from normal. 

---

## Principal Component Analysis

I will be performing Principal Component Analysis to find the components that capture the most variance from those extreme outliers since the data is heavily skewed. First, I created a Scree plot to decide how many principal components I should use. 

![Executive Dashboard](../Images/PCA%20PIC.png)

From this, I can see that the elbow is at Component 3 because it is where the graph flattens out.

![Executive Dashboard](../Images/Loadings%20PIC.png)

These Loadings show me that comp 1 must be the size of the company (workers and previous workers), comp 2 must be the maturity of the company (revenue and years on list), and comp 3 must be the growth of the company. This data set has now gone from 6 to 3 variables based on size, maturity, and growth of a company. 

![Executive Dashboard](../Images/PCA%20Scores%20PIC.png)

This PCA score plot shows that most of the companies are grouped around the (0,0) point, the average. However, there are two outliers in the bottom right of the plot with an enormous amount of size, but not a lot of time on the companies list. Around point (0,0) I realized that the points either go vertically or horizontally. This is because the companies are taking two different paths, one focusing on hiring and gaining employees, while the other focuses on increasing their revenue over time.

---

## Clustering



---

## Linear Discriminant Analysis



---

## Conclusion
