# Data Visualization and Reproducible Research

> Brunda Uppalapati

Learn more about me in my [GitHub profile page](https://github.com/brunda09). 


The following is a sample of products created during the _"Data Visualization and Reproducible Research"_ course.


## Project 01

Here I perform analysis of data science job posts available in glassdoor website to find interesting aspects around data science field.The dataset includes information about 648 job posts in glassdoor. The dataset chosen is: [Glassdoor Job Posts Data](https://www.kaggle.com/datasets/rashikrahmanpritom/data-science-job-posting-on-glassdoor?resource=download&select=Cleaned_DS_Jobs.csv) 

#### Data Analysis

 Performed an analysis to study the trends around:

  1)**Top 5 job titles** to observe the relative popularity of different job titles and gain insights into the job market for data science professionals. The plot allows us to compare the frequency of different job titles and identify the most prevalent roles.
  
  2)**Treemap for identifying level of scope in various Data Science Job Sectors**.Each rectangle represents a job sector, and the size of the rectangle corresponds to the frequency of job postings in that sector
  
  3)**Distribution of average salaries across different job types** using boxplots.
  
  4)**Relationship of Average salary versus Company Age** using scatterplot and regression line.This information provides insights into how the average salary varies based on the age of the company.

Find the code and report in the `project_01/` folder.

**My favorite visualization is :**

![Data Science Job Sectors](https://github.com/brunda09/dataviz_final_project/blob/main/figures/DS-Job-Sectors.png)


## Project 02

**Rape** is the **fourth** most common crime against women in India. Laws against rape come under the Indian Penal Code 376. Incest rape cases are registered under the condition where the offender is known to the victim.I was really much interested in knowing the trend of how the number of rape cases changed over time and also identify the states that are experiencing a high number of rape cases. The dataset chosen for the first, second and third plot is:
[Rape Victims Data](https://www.kaggle.com/code/nehaprabhavalkar/crimes-in-india-analysis/input?select=20_Victims_of_rape.csv)

#### Data Analysis
In this project, I explored :

1)The line plot shows how the **number of rape cases reported changed over time** by increasing from 2002 and peaked in 2005 and started decreasing thereafter.

2)**Displaying the state with largest number of rape cases** by loading the shapefile. `geom_sf()` is used to display spatial information.This plot shows the statewise comparison of the intensity of rape cases reported with Madhya Pradesh reporting the highest number of cases.

3)**Linear Regression Model** 
The dataset is grouped according to year and the number of cases is summed up and stored in a new sub dataset which is used to plot the linear regression graph. The "broom" library is used to tidy up the dataset and the linear regression is viewed with the help of `summary()` and `glance()` functions. I applied `geom_point()` and `geom_smooth()` with method `lm`. Also used `annotate()` to display the outlier in the data.

Find the code and report in the `project_02/` folder.

**My favorite visualization is:** 

![Statewise Rape Cases](https://github.com/brunda09/dataviz_final_project/blob/main/figures/statewise-rape-cases.png)


## Project 03

In this exercise I explored methods to create different types of data visualizations (such as plotting text data, or exploring the distributions of continuous variables) using the dataset obtained from FSU's [Florida Climate Center](https://climatecenter.fsu.edu/climate-data-access-tools/downloadable-data), for a station at Tampa International Airport (TPA) for 2022. The datasets chosen are:

[TPA Weather](https://raw.githubusercontent.com/reisanar/datasets/master/tpa_weather_2022.csv)

[RateMyProfessors comments](https://github.com/reisanar/datasets/blob/master/rmp_wit_comments.csv)

#### Data Analysis

- Part 1 : main task was to create density plots and a histogram using **faceting and ridges**.

- Part 2 : Visualized the text data contained in comments to create a frequency count of **most used bigrams**.


**My favorite visualization is:** 

![Max Temperatures Ridges](https://github.com/brunda09/dataviz_final_project/blob/main/figures/max_temp_ridges_plasma.png)


### Moving Forward

As a beginner studying Data visualization, I learnt a lot regarding the design principles, ggplot, grammar of graphics, spatial visualization, interactive plots, reproducible research etc and it helped me improve my coding skills. I intend to keep learning and practising on different datasets and implement them on other platforms like Tableau moving forward.
