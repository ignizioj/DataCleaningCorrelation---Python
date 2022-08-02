# Movie Dataset Cleaned and Examined for Correlation Using Python
### In the dataset were roughly 7600 rows of movies including name, rating, genre, year of release, year of production, score, votes, director, writer, star, country, budget, gross revenue generated, company, and runtime in minutes.

#### Before progressing to my questions and analysis of the data, I had to standardize and clean a few fields.  The first was to check for any missing data. I then dropped nulls based on the percentage calculated as I would be unable to do any prediction analysis with these specifically. The second item I addressed was the date released. I created a separate column for this correction as I only wanted the year of release and essentially had to parse the "released" column for the year portion. 

![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/Movies.png)

![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/newcol.png)

#### I also changed a data type for some numerical values and dropped any duplicates.


#### At this point, I was able to address my questions that I went into this little project with.  I was looking for correlation in the dataset between a movie's budget and the gross revenue from production and release.  Does the budget of a movie production have anything to do with the money earned? Does it potentially mean that movies with higher budgets will bring in more money?

#### I created a scatterplot of the budget and gross earned using Matplotlib and Pyplot. Below is an image of the initial plot.

![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/Scatterplot.png)

#### Next was to display a trendline using Seaborn.  I used a Pearson Regression as this would be the same as the Pearson Heatmaps I used to show the coefficient correlation strength.

![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/ScatterTrend.png)

#### I was able to look at the 'r' value using a table and heatmap. I had to change the value type of the objects to a numeric to display my heatmap properly. The results are below.

![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/CorrelationCoeffcientChart.png)
![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/HeatmapCorrelationMovieFeatures.png)
![ScreenShot](https://github.com/ignizioj/DataCleaningCorrelation-Python/blob/main/HeatmapNumericaFeatures.png)

### My conclusion was that yes, movies with a higher budget do in general earn more.  Is this because the quality is better? This question is left to be answered as the ratings don't seem to be consistently correlated.  However, the votes that a movie gets are correlated at a moderate strength with the budget.  This may be because of the profile or knowledge of the movie prior to release. 

### Feel free to browse any files found in the repository.  I was the only contributer in this project.  Thanks!
