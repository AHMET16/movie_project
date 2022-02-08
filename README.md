# best_movie_imdb_tmdb
#### Microsoft Movie Analysis
### Author: A KARAOGLAN
## Overview
This project represents a preliminary study of the entry into the microsoft film industry. The company, which is very new in this sector, made front studies by making use of the large database containing the data of movies such as IMDB, TMDB, ROTTEN TOMATOES. We decided to examine the director, genre and movie profit. We determined which film genres had a more successful effect on the directors' profit. Using this data, Microsoft can decide which movies it would be right to start with in its new project.

### Business Problem
Microsoft is the world leader in its field, but the film industry is also very new in terms of know-how, the company should decide how much budget it has outside of this project and decide on the film it will shoot. The results of the data and analyzes I have collected show the following. Genre and runtime data of the directors have determined the genre that provides the least risk for companies that have just started in the film industry.

### Data Understanding
## Questions to consider:

### Question Where did the data come from, and how do they relate to the data analysis questions?

The data is provided by Flatiron school and collected from the respective websites.

The data is collected from Box Office Mojo, IMDB, Rotten Tomatoes, and TheMovieDB.org. The data has information about movie titles, genres, directors, actors, profits, release year.


### Methods
### Data Preparation
## Questions to consider:

- How did you prepare the data ?

Here are the datasets that I used for analysis:

imdb datasets: imdb_title_basics, imdb_title_crew, imdb_title_principals, imdb_title_ratings, imdb_name_basics

tmdb dataset: tmdb_movies

bom dataset: bom_movie_gross

tn dataset: tn_movie_budgets

- Were there variables you dropped?

I dropped the following columns from the data:

  original_title, primary_title, Unnamed: 0, genre_ids, id, nconst, tconst,
  original_language, release_date, start_year, birth_year, death_year, 
  known_for_titles,  'category', 'job', 'characters', 
  'vote_count', 'runtime_minutes', 'ordering'
- Were there variables you created?
 I created a value 'profit', which is simply the worldwide_gross minus production_cost.
 
- How did you address missing values or outliers?

  I dropped rows with missing worldwide_gross or production_cost values.

- Why are these choices appropriate given the data and the business problem?

  Dropping the nan values, rather than replacing them is an appropriate choice, since I want to provide        accurate information.
   
- Why are these choices appropriate given the data and the business problem?
   
   Dropping the nan values, rather than replacing them is an appropriate choice, since I want to provide accurate information.


- Were there variables you dropped?

   I later dropped studio, year, domestic_gross, foreign_gross, worldwide_gross columns, since they are not necessary for further analysis.

 
  
