# Movies-ETL
In this repository, we have cleaned and combined large sets of data into one readable database that can now be analyzed. The data comes from both Wikipedia and Kaggle and describes movies.

The Wikipedia data came to us particularly cluttered which is no surprise, as anyone can edit a Wikipedia page. Things like sparsely populated columns, T.V. shows, repeated movies and rows with the same data only different names were all sorted out/combined. Once the Wikipedia data was cleaned up, we turned toward the much cleaner Kaggle data.

With both sets cleaned up, we combined them into one dataframe, “movies_df”. Since the Kaggle data was more complete, we chose to keep it in places where the two shared the same information. Missing data from Kaggle was then filled in using that of Wikipedia. 

A “ratings” dataframe was also created with over 26 million ratings.

![]( https://github.com/thomasstvr/Movies-ETL/blob/main/Resources/ratings_query.png)
A snippet showing the length of the ratings table.

Television shows were filtered out by dropping rows containing any value in the “Original Network” column. This column was chosen over “No. of episodes” and “No. of seasons” because it caught all of that witch could have been filtered with them and more. Shown below is a snippet of the length of the movies table.
	
![]( https://github.com/thomasstvr/Movies-ETL/blob/main/Resources/movies_query.png)

