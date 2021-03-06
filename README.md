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

 #### Evaluation
Questions to consider:

- How do you interpret the results?

 We have some general knowledge about how to make a profitable and popular movie in terms of genres and directors, writers and actors. I think this is a good first step in analysis.

- How confident are you that your results would generalize beyond the data you have?


  I think these results would generalize beyond this data because there are 16184 movies, which is a quite large number.
  
- How confident are you that this model would benefit the business if put into use?
 
  I think this analysis will be helpful in choosing genres and people to work with.
  
  
#### Conclusions

## Questions to consider:

- What would you recommend the business do as a result of this work?
  
  
    In terms of best movie genres for the highest profit, here are the top 10 genres that I would recommend:
  
  1. Adventure,Drama,Sport
  2. Biography,Documentary,History
  3. Sci-Fi
  4. Documentary,Drama,Sport
  5. Adventure,Drama,Sci-Fi
  6. Comedy,Mystery
  7. Action,Adventure,Sci-Fi
  8. Adventure,Fantasy
  9. Family
  10. Animation,Comedy,Family
  


![df1](png/df1.png)





    One important note about this list is it gives a combination of genres instead of one. That is how the original data was provided, thus the result is recommending a mix of genres for a new movie. 
    
    Also, for the highest profit, the company should consider the top names to work with for a new movie. Some of them are directors, some of them are writers and some of them are actors. Here are the top 10 people that brought in the highest profit:
    
    1. Michael Crichton
    2. Joe Robert Cole
    3. Rafe Spall
    4. Idina Menzel
    5. Shane Morris
    6. Kristen Anderson-Lopez
    7. Peter Del Vecho
    8. Peter Block
    9. Adam Green
    10. Hans Christian Andersen


![df4](png/df4.png)



    In terms of ratings, IMDB and TMBD had different results on the best genres. 
    
    Here are the top 10 movie genres by average votes on TMDB:
    
    1. Documentary,History
    2. Mystery,Thriller
    3. Biography,Drama,Musical
    4. Adventure,Drama,Sci-Fi
    5. Crime,Documentary
    6. Drama,Fantasy,Music
    7. Adventure,Drama,Western
    8. Drama,History,Thriller
    9. Biography,Drama,History
    10. Action,Adventure,Animation
    
    
   ![df2](png/df2.png)
   



    And, here are the top 10 genres according to IMDB ratings:
    
    1. Adventure
    2. Action,Sport
    3. Crime,Documentary
    4. Adventure,Drama,Sci-Fi
    5. Mystery,Thriller
    6. Sport
    7. Adventure,Drama,Mystery
    8. Comedy,Musical
    9. Adventure,Drama,Western
    10. Biography,Drama,Musical
    
    
   
    
    
    
   ![df3](png/df3.png)
  

    Again, in terms of ratings, IMDB and TMBD had different results on the best people to work with. 
    
    Here are the top 10 people by average votes on TMDB:
    1. Ben Sollee
    2. Allison Shearmur
    3. Neal Kingston
    4. Georgina Haig
    5. Miles Heizer
    6. Sebastien Guy
    7. Nina Dior
    8. Ben Evans
    9. Christian Clark
    10. J.R. Sawyers
    
   ![df5](png/df5.png)
   


      Here are the top 10 people by average votes on IMDB:
    1. Tara Fitzgerald
    2. Andrew Swarbrick
    3. Richard Heap
    4. Mark Addy
    5. Scott Nicol
    6. Lee Boardman
    7. Mario Roberto
    8. Mark Thomas
    9. Laura Perez
    10. Phil Wood
    
    
    
   ![df6](png/df6.png)



- What are some reasons why your analysis might not fully solve the business problem?


    I think there are many other factors to consider, such as the time of the year, the economy or any crisis going on, that are not included in this analysis. Therefore, this primary analysis will give a general idea about where to start, but more analysis should be done for better understanding of the industry.
    
    
- What else could you do in the future to improve this project?

   
 I can focus on directors, or actors in specific instead of people in general. I can also seperate genre categories and do a more comprehensive analysis.
    
    



### Repository Structure

    
   dsc-phase1-project-template.ipynb is a Jupyter Notebook containing all analysis and visualizations for the project.

DS_Project_Presentation.pdf contains presentation for the project.

Data folder contains zipped data about movies and provided by Flatiron School for the project. Data comes from IMDB, Rotten Tomatoes, and TMDB and Box Office Monjo.

Images folder contains the visualization created for analysis.






      ????????? README.md                           <- The top-level README for reviewers of this project
      ????????? dsc-phase1-project-template.ipynb   <- Narrative documentation of analysis in Jupyter notebook
      ????????? DS_Project_Presentation.pdf         <- PDF version of project presentation
      ????????? data                                <- Both sourced externally and generated from code
      ????????? images                              <- Both sourced externally and generated from code









  
