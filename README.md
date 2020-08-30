# Predicting IMDb Raitngs

To advance my knowldge of machine learning algorithims I dediced to work with [IMDb Datasets](https://www.imdb.com/interfaces/), a collection of seven .tsv files cataloging identifying features of every movie, TV episode, and short film title on IMDB. Of the seven files, I downloaded four that contained information about the director, writer, genre of close to one million titles.

# Data Cleaning and Exploratory Data Analysis

I dediced to keep five features in my data set: year, writer, director, genre, and runtime. I also created a metric called "score" whose formula was:

> score = 5-imdb_rating)*total_votes

I did this to differenciate high rated but small indpendatt films with large blockbusters. I wanted large, high rated blockbusters with lots of votes (ex: Shawshank Redemption, Forrest Gump, Godfather) to be ranked higher than small independant films that are also ranked high. **I only used this 'score' metric for EDA, and discarded it with I started. my ML models.**

Like anyone, I wanted to know what the best movies were, so I ranked every movie by my score metric.

