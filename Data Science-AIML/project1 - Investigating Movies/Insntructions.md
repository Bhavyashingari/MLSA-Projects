Perform exploratory data analysis on the netflix_data.csv data to understand more about movies from the 1990s decade.
What was the most frequent movie duration in the 1990s? Save an approximate answer as an integer called duration (use 1990 as the decade's start year).
A movie is considered short if it is less than 90 minutes. Count the number of short action movies released in the 1990s and save this integer as short_movie_count.
Feel free to experiment after submitting the project!


How to approach the project
1. Filter the data for movies released in the 1990s

2. Find the most frequent movie duration

3. Count the number of short action movies from the 1990s



1. Filter the data for movies released in the 1990s
You'll want to subset the DataFrame to keep only the movies and then filter the years so that you are working with rows where the release year is between 1990 and 1999.

Hint - passing in a condition. For example, if you wanted to subset a music_df DataFrame for rows where the column genre was "pop", you could use the following: 
music_df[music_df["genre"] == "pop"] 

Iterating through a DataFrame
Use a for loop with the .iterrows() method to iterate through the DataFrame's labels and rows. This might look like: 
for label, row in music_df.iterrows():

4. Count the number of short action movies from the 1990s
First, subset the data again to keep only movies with the correct genre. Then, iterate through the data and count the number of movies depending on the condition pf a duration that is less than 90.
