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

![Jupyter Notebook](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/Data%20Understanding.ipynb)

## Business Understanding

Computing vision is looking to create a new movie studio, our goal was to help analyze what genre movie to create based on rating and profitablity. Additionally, which well-known studio would be a profitable partner and should Computing Vision launch domestically or internationally.  

### Key Business Questions

* **What movies are doing well at the box office by genre and popularity ratings?** This will help establish if there is a genre that is exceedingly popular

* **What is the relationship between production budgets vs income by genre?** Establishing a relationship between budget and income by genre will help understanding if a big budget produces higher income, and if there are any genres that have particularly high profits.

* **What studio or director could Computing Vision work with to increase sales?** If there is a high correlation between a particular studio or director and high sales it would be beneficial to work with them.

* **Is there a benefit to producing a film domestic vs foreign?** This will help understand if there is a significant advantage to releasing the film internationally or domestically. 

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

### Three visualizations

Git-ing it Done created a few visualization to help support our questions and analysis.

* **Genre and Ratings** This visualization shows the genres with the highest ratings. Comedy and Action appear repeatedly are among the highest

![Genre and Ratings](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/visualizations/Genres_with_highest_rating.png)

* **Total Gross** This visualization shows the genres with the highest gross income. Actioc, adventure, as well as comedy appear frequently. This supports the genres with high ratings. An Action and comedy movie would be good for Computing Vision to create

![Total Gross](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/visualizations/Total_gross.png)

* **Domesting and Foreign Gross** This visualiztion shows the split between foreign and domestic gross. Foreign gross is often a larger percentage of the total gross. Computing vision should release internationally not strictly domestically.

![Domesting and Foreign Gross](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/visualizations/Domestic_and_foreign_gross.png)

* **Profit and Budget** This visualization shows the relationship between budget and profit. It appears that a high budget could be related to a higher profit, we examine this further in the statistical analysis.

![Profit and Budget](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/visualizations/Income_and_budget.png)

* **Studio with Highest Profit** This visualizaiton shows the studios that have the highest profit. Buena Vista (Disney) and Warner Bros are the top two. We would recommend that Computing Visions chooses to work with either Disney or Warner Bros in their creation of an action/comedy movie. 

![Studio with Highest Profit](https://github.com/QuinnGrigsby/Capstone_Git-ing_it_done_MovieInformation/blob/main/visualizations/Studio_with_high_profit.png)
    
## Statistical Communication

Git-ing it done decided the best question to pursue a statistical analysis on is budget vs profit.

We wanted to know if having a higher budget resulted in a larger profit.

* **H0** Having a larger budget will not increase the profit of a movie by genre

* **H1** Having a larger budget will increase the profit of a movie by genre

We calculated and used the following statistic for our analysis

* **Sample Mean** = 2.4923 (Percentage (x100))

* **Sample STDEV** = 2558 (Percentage (x100))

* **Sample Size** = 100 (genres)

* **Z-score** = -1.0691

* **P-value** = 0.1425

* **Alpha** = 0.05

### Results of statistical inference

Based on this data, with our pvalue being larger than our alpha we can significantly fail to reject the null hypothesis.

### Interpretation and context

This means that, having a larger budget does not necessarily mean larger profits. This is understandable because there are movie that have a high budget but poor performance at the box office. While some high profit earning movies have a high budget; we have high confidense that producing a movie with a high budget is not guaranteed to increase sales. 

## Conclusion

Git-ing it done is making the recommendation for Computing vision to partner with Buena Vista (Disney) or Warner Bros to make an action/comedy movie and to launch internationally with a modest budget for the film.

An Action/Comedy movie would likely produce significant profit, and attain a high popularity rating. This is supported by the graphs we made visualizing a high popularity and income related to action/comedy genres. Buena Vista (Disney) and Warner Brother are studios that produce a lot of profit. A partnership with them could prove valuable to Computing vision for producing a succesful movie. This is supported by the visualization showing the profit made by Buena Vista and Warner Bros. It is important for Computing Vision to launch internationally. Foreign releases can make up half or more of total income, supported by our visualization. 

If Computing Vision follows our recommendations they would produce a movie that is not only profitable, but popular. This will help them achieve their goal of creating a name for themselves in the movie industry. 
