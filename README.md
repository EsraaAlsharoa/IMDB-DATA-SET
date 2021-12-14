# IMDB-DATA-SET
This data set contains a mat file for a multi-layer network constructed form IMDB data set. The original data set is puplically available in SQL format in https://relational.fit.cvut.cz/dataset/IMDb.
IMDB data set consists of movies on the IMDB’s top 250 and bottom 100 chart along with their genres and directors with  166 movies, 130 directors and 20 movie and director genres.
The mat file contains the following:
-----------------------------------------------------------------
## Table of contents
* [The Directors Full Names](#The-Directors-Full-Names) 

* [The Movies Full Names](#The-Movies-Full-Names)

* [The genres of the directors](#The-genres-of-the-directors)
* [The genres of the movies](#The-genres-of-the-movies)
* [IDs of all movies and directors](#IDs-of-all-movies-and-directors)
* [The genres](#The-genres)
* [The movies's genres matrix ](#The-movies's-genres-matrix) 
* [The directors's genres matrix](#The-directors's-genres-matrix)
* [The directors intra-layer adjacency](#The-directors-intra-layer-adjacency)
* [The movies intra-layer adjacency](#The-movies-intra-layer-adjacency)


## The Directors Full Names
IMDB_DataSet.DirectorsFullnames

## The Movies Full Names
IMDB_DataSet.MoviesFullnames

## The genres of the directors
IMDB_DataSet.AllDirectorsGenres

## The genres of the movies
IMDB_DataSet.AllMoviesGenres

## IDs of all movies and directors
IMDB_DataSet.DirectorsMoviesIDs. The matrix is organized as follows:

Director's original ID ,    Movie's original ID  , Director's new ID ,  Movie's new ID
----------------------     -------------------   -----------------   --------------

## The genres
IMDB_DataSet.Genres


## The movies's genres matrix 
IMDB_DataSet.MoviesGenresMatrix. The matrix is organized as follows:

Movie's original ID , Movie's new ID  , Genres vector
-------------------  --------------  -------------
For every movie, a binary-valued genre vector is generated where the entries of the vector are 1 if the movie is in that genre and 0 otherwise.


## The directors's genres matrix
IMDB_DataSet.DirectorsGenresMatrix. The matrix is organized as follows:
director's original ID ,  Director's new ID  , Genres vector
----------------------   -----------------   -------------
For every director, a binary-valued genre vector is generated where the entries of the vector are 1 if the director directed a movie in that genre and 0 otherwise.


## The directors intra-layer adjacency
IMDB_DataSet.DirectorsIntraLayerNetwork 


  
## The movies intra-layer adjacency
IMDB_DataSet.MoviesIntraLayerNetwork


11- The directors-movies inter-layer adjacency: IMDB_DataSet.DirectorsMoviesInterLayerNetwork
-----------------------------------------------------------------

Author: Esraa Alsharoa
------------------------
Last page update: Dec. 14, 2021
