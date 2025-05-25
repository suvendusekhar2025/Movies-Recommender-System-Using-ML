# Movies-Recommender-System-Using-ML
The dataset used in this project can be accessed here:  
[📁 Download Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
# What I hane done in this Project!
🎬 Movie Recommender System Using Machine Learning
This project focuses on building a Movie Recommender System that suggests movies to users based on their preferences. In today’s era of information overload, recommender systems play a crucial role in helping users discover content they’re likely to enjoy—making them essential for platforms like Netflix, Amazon Prime, and YouTube.

🔍 Project Overview
The goal is to create a machine learning-based system that recommends movies to users by analyzing patterns in the dataset, such as genres, user ratings, cast, crew, and overviews. The system leverages content-based filtering techniques to generate relevant movie suggestions tailored to user preferences.

🧠 Machine Learning Approach
This project uses a content-based filtering algorithm which works by analyzing the properties (metadata) of the movies—like genres, keywords, cast, and overview text. It creates feature vectors for each movie and calculates cosine similarity to find movies that are similar to a user’s liked movies.

#Key techniques used include:

- Text vectorization using TF-IDF and CountVectorizer

- Natural Language Processing (NLP) for preprocessing descriptions

- Cosine similarity to compute movie-to-movie closeness

🛠 Workflow Summary
1. Data Collection and Understanding
The dataset includes:

- Movie titles, genres, keywords

- Cast and crew details

- Overview and tagline

- Popularity and vote counts

- Two datasets (tmdb_5000_movies.csv and tmdb_5000_credits.csv) are merged and cleaned to extract relevant features.

2. Data Preprocessing
Handling missing values

- Parsing stringified JSON columns (e.g., genres, keywords, cast)

- Combining textual features into a single 'tags' column for each movie

- Removing stopwords and applying stemming to standardize the data

3. Feature Extraction
-> Using CountVectorizer to convert movie tags into vectors

-> Limiting the feature set to top 5000 most frequent terms

-> Creating a similarity matrix using cosine similarity scores

4. Recommendation Engine
-> When a user inputs a movie title, the system:

-> Finds its index in the dataset

-> Calculates similarity scores with all other movies

> Returns the top 5 most similar movies as recommendations

5. Deployment and UI
- The model is deployed using Streamlit to create an interactive web interface

- Users can select a movie and instantly receive recommendations along with poster images fetched via API

🎯 Key Outcomes
-> The recommender system successfully returns relevant movie suggestions based on user input

-> Efficient use of NLP and vector similarity enables fast and meaningful recommendations

-> Integration with Streamlit provides an intuitive user experience

✅ Benefits and Applications:
- Helps users explore new movies based on their preferences

- Can be integrated into larger entertainment platforms for personalized recommendations

- Scalable and extendable for more features (e.g., hybrid filtering, user behavior tracking)

🚀 Potential Future Enhancements:
-> Integrate collaborative filtering to combine user behavior with content metadata

-> Add user authentication and history tracking

-> Incorporate movie ratings into the recommendation logic

-> Use deep learning-based approaches (e.g., embeddings or neural networks)

-> Improve NLP processing by using BERT or other transformers for contextual understanding
