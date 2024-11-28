
# Structure
- [ ] Try to implement DS structure (study and implement): https://cookiecutter-data-science.drivendata.org/
	- [x] Initial read

# Datasets

- [x] Research datasets
- [ ] Datasets
	- [x] IMDB Dataset
	- [ ] TMDB 
		- [x] Desired fields: revenue, popularity?
		- [ ] API: https://developer.themoviedb.org/docs/getting-started
		- [ ] TMDB top 5000  https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata?select=tmdb_5000_movies.csv
		- [ ] TMDB Full Dataset (New) ~500 MB https://www.kaggle.com/datasets/asaniczka/tmdb-movies-dataset-2023-930k-movies
			- [ ] Download TMDB_movie_dataset_v11.csv (522.43 MB)
	- [ ] MovieLens
		- [x] Desired fields: Tags

# EDA

- [ ] IMDB EDA
	- [x] name.basics.tsv.gz (80%)
	- [ ] title.ratings.tsv.gz
	- [ ] title.akas.tsv.gz
	- [ ] title.basics.tsv.gz
	- [ ] title.crew.tsv.gz
	- [ ] title.episode.tsv.gz
	- [ ] title.principals.tsv.gz
- [ ] TMDB EDA
	- [ ] TMDB_movie_dataset

# Preprocessing and Feature Engineering

- [ ] Refactor EDA parts for preprocessing and future use
	- [ ] Missing data
	- [ ] Outliers
	- [ ] Handling numerical
	- [ ] Handling categorical
	- [ ] Visualization scripts

- [ ] Filters:
	- [x] Runtime < 150-180 minutes
	- [ ] Possible:
		- [ ] startYear > 2000
		- [ ] 

- [x] Research relevant features
- [ ] Feature Engineering
	- [ ] Target / Directly related
		- [ ] Ratings
		- [ ] Revenue - (TMDB)
	- [ ] Easy to use
		- [ ] Language
		- [ ] Year
		- [ ] Runtime
		- [ ] Country
	- [ ] Complex / High cardinality categories
		- [ ] Production Company
		- [ ] Genres
			- [ ] Word embeddings
				- [ ] https://superlinked.com/vectorhub/articles/movie-recommendation-using-vectordb
			- [ ] Target encoding
				- [ ] Genre - Revenue/Rating
		- [ ] Actors
			- [ ] Target Encoding
				- [ ] Actor - revenue / actor - rating
			- [ ] Target encoding + filter/interaction
				- [ ] Actor - revenue in a specific genre
			- [ ] Entity embeddings
	- [ ] Possibly Target leakage / Future information / Encode to other features
		- [ ] Awards
		- [ ] Reviews / Sentiment

# Model and Training


- [ ] Main Model - XGBoost for tabular data
- [ ] Research creative models
	- [ ] Research
	- [ ] BERT Trained on movies, genre, reviews, etc. - document classification

# Answer Questions

- [ ] Answer Questions:
	- [ ] What is the highest rated movie in 2023? 
		- [ ] EDA - sort
	- [ ] How do we balance ratings and number of votes?
		- [ ] Research
		- [ ] EDA
	- [ ] Who was the most popular actor in 2023?
		- [ ] Research popularity metrics
		- [ ] EDA aggregates
	- [ ] What are the trends in user-movie preferences over the years?
		- [ ] EDA
	- [ ] Define a metric that captures the notion of a ‘hit movie’; justify your metric in the context of a movie studio director looking to invest in building the next AAA title
		- [x] Initial Research
		- [ ] Decide / Combination between revenue and rating

- [ ] Build and Train Model
	- [ ] XGBoost
	- [ ] BERT
	- [ ] Ensemble

- [ ] Recommender
	- [ ] Baseline model
	- [ ] Target model - Collaborative filtering + matrix factorization
	- [ ] Custom Interpretable model
	- [ ] Visualizations and Demo
		- [ ] Possible to visualize and plot latent features?



