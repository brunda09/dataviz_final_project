---
title: "Data Visualization for Exploratory Data Analysis Project-03"
author: "Brunda Uppalapati4872@floridapoly.edu"
output: 
  html_document:
    keep_md: true
    toc: true
    toc_float: true
---

# Data Visualization Project 03


In this exercise you will explore methods to create different types of data visualizations (such as plotting text data, or exploring the distributions of continuous variables).


***
#### The libraries installed in the project and loaded are as follows:

1. Tidyverse
2. ggplot
3. viridis
4. dplyr
5. ggridges
6. tidytext
7. RColorBrewer
8. lubridate
9. viridisLite

***

**"The Dataset used for the project is obtained from FSU for a station at Tampa International Airport (TPA) for the year 2022"**

[Florida Climate Center](https://climatecenter.fsu.edu/climate-data-access-tools/downloadable-data)


*The link for the Dataset chosen for recreating the graphs:
[Tampa Weather Data](https://raw.githubusercontent.com/reisanar/datasets/master/tpa_weather_2022.csv)*


> The main task of Part 1 was to recreate six graphs which makes use of faceting and ridges:

#### Question (a)

The initial step is to convert the numeric columns of "month" into written characters, the function **as.factor** is made use of  whose main function is to return the original object of a class with the requested column specified as a factor rather than numeric.

To obtain the actual graph according to the image given, the function of **facet_wrap** is performed on the column month and the months are divided into different grids and the data is displayed in the form of a histogram. 

![Maximum Temp vs. Days](https://github.com/brunda09/dataviz_final_project/blob/main/figures/max-temp-facet.png)


***

#### Question (b)

The second plot is the density plot which is evaluated using the kernel **epanechnikov** and the parameters of bw and lwd which set the bandwidth and line width respectively are also used to plot the graph.

![Density Plot](https://github.com/brunda09/dataviz_final_project/blob/main/figures/max-temp-density.png)

***

#### Question (c)

The third plot is the density plot along with facet_wrap which is evaluated using the default kernel **gaussian** is used to plot the graph.The legend is omitted from being displayed by using the function *legend.position = "none"*

![Default Density Plot](https://github.com/brunda09/dataviz_final_project/blob/main/figures/density-facet.png)

***

#### Question (d)

Density ridges is plotted with quantile lines and the plot showcases the second quantile. The plot below uses the `plasma` option (color scale) for the _viridis_ palette

![Density Plot Plasma](https://github.com/brunda09/dataviz_final_project/blob/main/figures/max_temp_ridges_plasma.png)

***

#### Question (e)

The bar plot shows average precipitation for each month. It shows that the precipitation is high in the months of June, July, August indicating heavy rainfall in those 3 months.Also we can see sharp tranisitional periods May to June and then August to September indicating the transition from a wet season to a dry season or vice versa.

![Average Precipitation](https://github.com/brunda09/dataviz_final_project/blob/main/figures/avg-precipitation.png)

***

#### Part 2 - Option (a)

Here I picked up the dataset: [RateMyProfessors comments](https://github.com/reisanar/datasets/blob/master/rmp_wit_comments.csv) and visualized the text data contained in "comments" column to create a frequency count `geom_bar()` of **most used bigrams** ignoring the stopwords.

![Bigram](https://github.com/brunda09/dataviz_final_project/blob/main/figures/bigram.png)

***
