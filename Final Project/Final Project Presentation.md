Final Project Presentation
========================================================
author: Vic Chan
date: 
autosize: true

Introduction
========================================================

- For my final project I created extended Week 2 Assignment with the knowledge that we have gain throughout the semester.
- I will be showing the ratings of all the movies Michael Bay has directed and their ratings from multiple sources and normalizing the ratings to create one final rating for the end user.

OMDB API
========================================================
- Open Source API - Just need to sign up and get a limited amount of calls to the API a day
- Provides a lot of information on the movie including the scores from IMDB, Rotten Tomato, and Metacritics
- Example of a API Call




```
           Length Class      Mode     
Title      1      -none-     character
Year       1      -none-     character
Rated      1      -none-     character
Released   1      -none-     character
Runtime    1      -none-     character
Genre      1      -none-     character
Director   1      -none-     character
Writer     1      -none-     character
Actors     1      -none-     character
Plot       1      -none-     character
Language   1      -none-     character
Country    1      -none-     character
Awards     1      -none-     character
Poster     1      -none-     character
Ratings    2      data.frame list     
Metascore  1      -none-     character
imdbRating 1      -none-     character
imdbVotes  1      -none-     character
imdbID     1      -none-     character
Type       1      -none-     character
DVD        1      -none-     character
BoxOffice  1      -none-     character
Production 1      -none-     character
Website    1      -none-     character
Response   1      -none-     character
```

Ratings
========================================================
- The ratings are from 3 different sources
- Each of the source has a different rating system 
- Need to somehow normalize all the different rates


```r
json_file$Ratings
```

```
                   Source  Value
1 Internet Movie Database 6.9/10
2         Rotten Tomatoes    42%
3              Metacritic 41/100
```

Min Max Normalization
========================================================
- Simple to implement
- Returns a value from 0 to 1
- $1 + 1$

