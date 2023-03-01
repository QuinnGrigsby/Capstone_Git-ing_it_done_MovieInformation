# Git-ing it done
# Computing Vision Film Creation

## Overview

Git-ing it done was hired to assist Computing Vision in creating a successful movie studio. 

In our report we will cover:

* [***Business Understanding:***](#business-understanding) Our understanding of the goal, key questions, and stakeholders
* [***Data Understanding and Analysis:***](#data-understanding-and-analysis) Our data sources, descriptions, and visualizations
* [***Statistical Communication:***](#statistical-communicaiton) Our statistical analysis and interpretation
* [***Conclusion:***](#Conclusion) Our relevant findings and recommendations

## Business Understanding

Computing Vision looking to create a movie studio, our goal was to help analyze what genre movie would be the most successful.
Git-ing it done formed a few key questions to answer in order to provide the stakeholders our best recommendations. 

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

To make actionable insights to Computing Vision we examined data from multiple different sources. 

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

### Three visualizations

Add three visualizations
    

## Statistical Communication

Git-ing it done decided the best question to pursue a statistical analysis on is budget vs profit

### Results of statistical inference

### Interpretation and context

## Conclusion

Git-ing it done is making the recommendation to 