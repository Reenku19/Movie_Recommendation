Content-Based Movie Recommendation System

This project implements a content-based movie recommendation system that suggests movies to users based on their preferences and the content of the movies themselves. By analyzing movie attributes like genre,title, original_langauage, popularity and potentially plot descriptions (depending on your implementation), the system identifies similar movies and recommends them.

Implementation Details

1. Data Preprocessing: Describe how you clean and prepare the movie data (e.g., handling missing values, converting categorical data).

2. Feature Engineering: Explain any feature extraction or transformation techniques used to represent movies for similarity calculations (e.g., TF-IDF for plot descriptions, one-hot encoding for categorical features).

3. Similarity Measure: Specify the similarity metric used to compare movies (e.g., cosine similarity, Euclidean distance).

4. Recommendation Algorithm: Explain the process of finding similar movies based on user preferences or a reference movie (e.g., neighborhood-based approach, matrix factorization).

5. Evaluation: (Optional) If applicable, describe any evaluation metrics used to assess the recommendation system's performance (e.g., precision, recall, recommendation accuracy).

Software Requirements

Operating System: Windows 10 or higher Programming:
1. Anaconda distribution package (Jupyter Notebook)
2. Anaconda distribution package (PyCharm Editor)
3. Python libraries (NumPy, Pandas, Streamlit, Requests, SKlearn)

Hardware Requirements

1. Minimum 5 GB HDD space
2. Intel Core 2 Duo or above processor
3. 4 GB RAM Required or above
4. x86 64-bit CPU (Intel / AMD architecture)
5. Power Supply for Backup



Architecture of the System

![image](https://github.com/user-attachments/assets/14980f93-0c58-4b18-a694-c546a4c1eac3)

Dataset Details 


The ‘TMDB 10000 Movie Dataset’ is taken into consideration for movie recommendation purposes in this research work. This dataset is available on kaggle.com. These files contain metadata for all 10,000 movies listed in the Dataset. The Data points include id, title, genre, original_language, overview, popularity, release_date, TMDB vote counts, and vote averages. The Movie Details have been collected from the TMDB Open API. Their API also provides access to data on many additional movies, actors and actresses, crew members, and TV shows. 
●	‘id’: It indicates the movie ID 
●	‘title’: It is nothing but the movie title. 
●	‘Genres’: It indicates the genres of the movie like Action, Documentary, etc.  
●	‘Original_language’: It indicates whether the movie is originally created in English or other language. 
●	‘Overview’: It is a short description of the movie. 
●	‘Popularity’: It is a metric which indicates popularity. 
●	‘Release_date’: It consists of the release date of the movie.  
●	‘Vote_average’: It indicates the average of the votes. ● 	‘Vote_count’: It indicates the vote count.


Implementation Of Machine Learning Algorithm

1. Gather the data
   
For this problem, I decided to use the dataset containing 10000 movies from TMDB. This table gathers, in fact, 10000 observations (the movies) and 9 columns. This is what the data frame’s head looks like.
![image](https://github.com/user-attachments/assets/7d380499-f152-4ba6-9c01-d34f6de1d214)

2. Data cleaning

After gathering, to clean the data we check for missing values in the dataset and the new data frame is ready for vectorization.
![image](https://github.com/user-attachments/assets/d4e6a160-124e-488d-8f00-cdcf6e82903f)

3. Modeling

To detect the similarities between movies, I decided to use Count Vectorizer. Once I have the matrix containing the count for each word, we can apply the cosine similarity function.
![image](https://github.com/user-attachments/assets/6ebe7656-529e-47a9-8b47-156cc1f60dcd)

4. Testing the recommender
   
The job is done! Let’s test it by entering Iron Man: these are the top 5 recommended movies (among the 10000 available).
![image](https://github.com/user-attachments/assets/c29ef7e4-b2b6-4db9-83b2-8538d3ae2d0b)



Anaylsis

Graph Plotting 

1. Pair Plot

![image](https://github.com/user-attachments/assets/fdac599c-b367-406a-b2c6-979f559ba3a5)

2. Bar Graph
   
![image](https://github.com/user-attachments/assets/d6ed6714-4a4f-4f13-b7ec-c386a6cfcd3e)


Snapshots


![image](https://github.com/user-attachments/assets/7c9281d6-761d-4815-882e-6295051bf20a)
![image](https://github.com/user-attachments/assets/a8778bf6-aebc-49be-8061-fa11355acdb1)







