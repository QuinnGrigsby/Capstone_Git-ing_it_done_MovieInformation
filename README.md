# Git-ing it done
# Computing Vision Film Creation

## Overview

Git-ing it done was hired to assist Computing Vision in creating a successful movie studio. 

In our report we will cover:

* [***Business Understanding:***](#business-understanding) Our understanding of the goal, key questions, and stakeholders
* [***Data Understanding and Analysis:***](#data-understanding-and-analysis) Our data sources, descriptions, and visualizations
* [***Statistical Communication:***](#statistical-communicaiton) Our statistical analysis and interpretation
* [***Conclusion:***](#Conclusion) Our relevant findings and recommendations

Related PowerPoint and Jupyter notebook are linked below

[PowerPoint Presentation](Capstone_Pod4_Presentation.pdf)

![Jupyter Notebook](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/cristian/Data%20Understanding.ipynb)

## Business Understanding

Computing vision is looking to create a new movie studio, our goal was to help analyze what genre movie to create based on rating and profitablity. Additionally, which well-known studio would be a profitable partner and should Computing Vision launch domestically or internationally.  

### Key Business Question

* **What is the relationship between production budgets vs income by genre?** Establishing a relationship between budget and income by genre will help understanding if a big budget produces higher income, and if there are any genres that have particularly high profits.

### Stakeholders 

In our analysis we considered a few key stakeholders including:

* **Computing Vision**
* **Git-ing it done**
* **Movie Goers and Critics**
* **Directors and Studios**

## Data Understanding and Analysis

To make actionable insights for Computing Vision we examined data from multiple different sources. 

### Sources of Data

In the folder [zippedData](zippedData) are movie datasets from:

* [Box Office Mojo](https://www.boxofficemojo.com/)
* [IMBD](https://www.imdb.com/)
* [Rotten Tomatoes](https://www.rottentomatoes.com/)
* [TheMovieDB](https://www.themoviedb.com/)
* [The Numbers](https://www.the-numbers.com/)

Our Main focus was the data sources from Box Office Mojo, and IMDB. 

### Descriptions of Data

Our first step was to implement some data cleaning in the Box Office Mojo dataset. This includes

* **Replacing null values in foreign and domestic gross income with "0".** This enables to be able to convert data types to float

* **Removing rows that contained a null value in Studio, this was a removal of only 5 rows.** As there was only 5 rows containing a missing studio we felt it was appropriate to drop those five rows.

* **Removing any commas in the foreign and domestic gross columns to treat them equally as floats.** Removing commas was required to treat the columns as floats instead of strings.

* **Creating a column that represents the total gross income.** A total gross income column will help identify which movies had the highest sales whether they were released internationally or not. 

Our second step was to clean The Number data set. We followed the same cleaning steps as we did with the Box Office Mojo dataset.

Finally, we utilized the IMDB database. Data cleaning was performed in the queries and in the dataframes following similar steps as the Box Office Mojo dataset. 

### Visualizations

Git-ing it Done created a few visualization to help support our questions and analysis.

* **Profit and Budget** This visualization shows the relationship between budget and profit. It appears that a high budget could be related to a higher profit, we examine this further in the statistical analysis.

![Profit and Budget](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/visualizations/Income_and_budget.png)

More to be found within the main and branch notebook.
    
## Statistical Communication

Git-ing it done decided the best question to pursue a statistical analysis on is budget vs profit.

We wanted to know if having a higher budget resulted in a larger profit.

* **H0** Having a larger budget will not increase the profit of a movie by genre

* **H1** Having a larger budget will increase the profit of a movie by genre

We calculated and used the following statistic for our analysis

* **Sample Mean** = 2.4923 [Percentage (x100)]

* **Sample STDEV** = 2.558 [Percentage (x100)]

* **Sample Size** = 100 (genres)

* **Z-score** = -1.0691

* **P-value** = 0.1425

* **Alpha** = 0.05

### Results of statistical inference

Based on this data, with our pvalue being larger than our alpha we can significantly fail to reject the null hypothesis.

### Interpretation and context

This means that, having a larger budget does not necessarily mean larger profits. This is understandable because there are movie that have a high budget but poor performance at the box office. While some high profit earning movies have a high budget; we have high confidense that producing a movie with a high budget is not guaranteed to increase sales. 

## Conclusion and Recommendation

On one side, some graphs showed that despite the budget assign to a movie porject, often the result tend to show huge incomes; but in the other, and with other data, the same graph showed that we can also deal with losses.

Due to this uncertantity of knowing how much budget to assign to a project to see if it was profitable or not, we continued with a statistical analysis using the data that made up the "Percentage of Profit" and "Percentage of Losses"; where we find out that there is actually no relation between high budgets and low budgets and the income of a movie.

We could recommend though, to produce a movie among the top 10 most profitable genres and assign it a moderate budget, so in the case that it results that we could not retrieve the investment back, it would not be that much of a loss.