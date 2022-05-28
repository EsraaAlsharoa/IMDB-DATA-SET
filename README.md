# IMDB-DATA-SET
This data set contains a mat file for a multi-layer network constructed form IMDB data set. The original data set is puplically available in SQL format in https://relational.fit.cvut.cz/dataset/IMDb.
IMDB data set consists of movies on the IMDB’s top 250 and bottom 100 chart along with their genres and directors with  166 movies, 130 directors and 20 movie and director genres.

* If you are using this data set, please cite the following paper:
Al-Sharoa, Esraa M., and Selin Aviyente. "Community Detection in Fully-Connected Multi-layer Networks Through Joint Nonnegative Matrix Factorization." IEEE Access 10 (2022): 43022-43043.
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
* [The directors-movies inter-layer adjacency](#The-directors-movies-inter-layer-adjacency)

## Author: Esraa Al-sharoa
Last page update: May. 29, 2022


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
IMDB_DataSet.DirectorsIntraLayerNetwork: The directors intra-layer network is constructed by calculating pair-wise Pearson correlation coefficient between
the directors’ genre vectors. The edges with correlation values
greater than 0.5 are kept in the final adjacency.

  
## The movies intra-layer adjacency
IMDB_DataSet.MoviesIntraLayerNetwork: The movies intra-layer network is constructed by calculating pair-wise Pearson correlation coefficient between
the movies’ genre vectors. The edges with correlation values
greater than 0.5 are kept in the final adjacency.



## The directors-movies inter-layer adjacency
IMDB_DataSet.DirectorsMoviesInterLayerNetwork: The directors-movies inter-layer network is constructed
such that a node from the director layer is connected to a
node from the movie layer if the director directed that movie.



