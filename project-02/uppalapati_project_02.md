---
title: "Report for Data Visualization Mini-Project 02"
author: "Brunda Uppalapati - buppalapati4872@floridapoly.edu"
output: 
  html_document:
    keep_md: true
    toc: true
    toc_float: true
---

# Data Visualization Project 02


**"The Dataset that has been used for the Interactive plot and Linear Regression plot is that of the Indian Crime Analysis"**

*The link for the Dataset chose for the first and third plot is:
[Indian Rape Data](https://www.kaggle.com/code/nehaprabhavalkar/crimes-in-india-analysis/input?select=20_Victims_of_rape.csv)*


**"The Shapefile that has been used for the Spatial Visualization is that of Indian States"**

*The link for the Shapefiles can be obtained from:
[Indian States Shapefile](https://www.kaggle.com/code/nehaprabhavalkar/crimes-in-india-analysis/input?select=India+States)*

***

#### The packages and libraries installed in the project and loaded are:

1. Tidyverse
2. ggplot
3. plotly
4. dplyr
5. RColorBrewer
6. htmlwidgets
7. sf
8. broom
9. scales

***

### Interactive Plot

**Displaying the change in the total number of rape cases reported throughout the years**

The original dataset is grouped by with the help of the group_by() function and the number of rape cases are summed up and a new sub-dataset is created.

The library of `plotly` is used to create an interactive graph which is much more visually appealing. The original graph that was intended to be plotted was a barplot which displayed the total rape cases that were reported each year.

The plot basically enables the user to observe the total no. of rape cases that have occurred in each year.

A scatter plot is plotted which is displayed with the help of "markers+lines" which makes it easier to get the total cases that have been recorded in a particular year. The layout function helps in labelling the axes and title of the plot.

The interactive plot is then saved as a standalone **HTML File** which can be accessed via:

[Rape Cases Data](file:///C:/Users/bruva/dataviz_final_project/project-02/reported_cases_figure.html)

***

### Spatial Visualization

**Displaying the intensity of rape cases reported in Indian States**


In the initial step the shapefile of the data being used is loaded. The shapefile format is a geospatial vector data format for geographic information system (GIS) software.

Then merge operation is performed using `join()` to relate shapefile with our dataset of rape victims.geom_sf() is used to display spatial information and mercator projection is used .


![Graph for Areawise Rape Cases](C:\Users\bruva\dataviz_final_project\figures\statewise-rape-cases.png)

***

### Linear Regression Model 


The dataset is grouped according to year and the number of rape cases reported are summed up and stored in a new sub dataset which is used to plot the linear regression graph. The `broom` library is used to tidy up the dataset and the linear regression is viewed with the help of `summary()` and `glance()` functions. 


![Model for Rape Cases](C:\Users\bruva\dataviz_final_project\figures\linear-regression.png)

***
