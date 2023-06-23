---
title: "Report for Data Visualization Mini-Project 01"
author: "Brunda Uppalapati - buppalapati4872@floridaploy.edu"
output: 
  html_document:
    keep_md: true
    toc: true
    toc_float: true
---

# Data Visualization Project 01


**"The Dataset gives data about data science job posts available in glassdoor website to help find interesting aspects around data science field.The dataset includes information about 648 job posts in glassdoor."**

*The link for the chosen Dataset is:
[DS Jobs Data ](https://www.kaggle.com/datasets/rashikrahmanpritom/data-science-job-posting-on-glassdoor?resource=download&select=Cleaned_DS_Jobs.csv)*

***

> All the relevant packages and libraries are installed and the required dataset was loaded into R studio. The columns were reviewed to get a better understanding of the steps needed and to make a visual assessment.

***

The Four Main Graphs which have been visualized are as follows:

* Graph for Top 5 job titles
* Treemap for Data Science Job Sectors
* Distribution of average salaries across different job types
* Average salary versus Company Age

### First Data Visualization Graph

**Finding the Top 5 job titles**

![Graph for Top 5 job titles](C:\Users\bruva\dataviz_final_project\figures\top-5-job titles.png)

The plot shows the top 5 most common job titles in data science based on the provided dataset. By analyzing this chart, we can observe the relative popularity of different job titles and gain insights into the job market for data science professionals. The plot allows us to compare the frequency of different job titles and identify the most prevalent roles which is data scientist in this context.

The original chart planned for this visualization was a bar chart showing the distribution of job titles in the field of data science. The goal was to identify the most common job titles.

***

### Second Data Visualization Graph

**Treemap for Data Science Job Sectors**

![Treemap for Data Science Job Sectors](C:\Users\bruva\dataviz_final_project\figures\DS-Job-Sectors.png)

The plot visually presents the distribution of job sectors within the field of data science using a treemap chart. Each rectangle represents a job sector, and the size of the rectangle corresponds to the frequency of job postings in that sector. By examining the treemap, we can identify the relative prominence of different sectors and gain insights into the areas of specialization and industry focus within data science job opportunities.
`treemapify` package has been used here.

 The original chart planned for this visualization was a pie chart representing the distribution of job sectors in data science but it turned out clumpsy.

***

### Third Data Visualization Graph

**Distribution of average salaries across different job types**

![Avg salary by job type](C:\Users\bruva\dataviz_final_project\figures\avg-salary-by-job-type-1.png)

The plot allows us to compare the salary distributions for different job types within the data science field. By examining the box plot, we can identify the median, quartiles, and any outliers for each job type. The addition of color enhances the visualization, making it easier to differentiate the job types visually. The sorting of job types based on median salary helps us identify the job types with higher or lower salary ranges. This information provides insights into the salary differences based on job roles within the data science field.
`RColorBrewer` package has been used here.

 The original chart planned for this visualization was a box plot showing the distribution of average salaries across different job types. The improvement made was to add color to the box plot to differentiate the job types visually and sort them based on the median salary for better comparison.

***

### Fourth Data Visualization Graph

**Relation between Average salary versus Company Age**

![Avg salary by company age](C:\Users\bruva\dataviz_final_project\figures\avg-salary-by-company-age-1.png)

The plot allows us to explore the relationship between average salary and company age within the dataset. By examining the scatter plot and the added regression line, we can identify any trends or patterns that might exist. If the regression line has a positive slope, it suggests that there is a general trend of higher average salaries for older companies. Conversely, if the regression line has a negative slope or no significant trend, it indicates a less clear relationship between average salary and company age. This information provides insights into how the average salary varies based on the age of the company.
`geom_smooth` method has been used here.

The original chart planned for this visualization was a scatter plot showing the relationship between average salary and company age. The improvement made was to add transparency to the scatter plot points, include a linear regression line to show the overall trend, adjust the font sizes for better readability, and remove the legend since we have only one group represented by the scatter plot points.

***
