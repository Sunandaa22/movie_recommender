# Movie Recommender System

## Overview
This project is a content-based movie recommender system that suggests similar movies based on the features of a given movie. The system uses the TMDB 5000 Movies dataset to analyze movie attributes such as genres, keywords, cast, crew, and overview to generate recommendations.

## Features
- **Content-Based Filtering**: Recommends movies based on similarity in content (genres, keywords, cast, crew, and overview).
- **Data Processing**: Cleans and processes movie data to extract relevant features.
- **Cosine Similarity**: Uses cosine similarity to measure the similarity between movies.
- **Stemming**: Applies stemming to reduce words to their root form for better text processing.

## Dataset
The dataset used is the TMDB 5000 Movies dataset, which includes:
- `tmdb_5000_movies.csv`: Contains details about movies such as budget, genres, keywords, overview, etc.
- `tmdb_5000_credits.csv`: Contains information about the cast and crew for each movie.

## Dependencies
- Python 3.x
- Libraries:
  - pandas
  - numpy
  - scikit-learn
  - nltk

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Sunandaa22/movie_recommender.git
   cd movie_recommender
   ```

2. Install the required libraries:
   ```bash

   pip install pandas numpy scikit-learn nltk
   ```

3. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata) and place the CSV files in the project directory.

## Usage
1. Run the Jupyter notebook `movie_recommender.ipynb` to process the data and build the recommender system.
2. Use the `recommend(movie_name)` function to get movie recommendations based on the input movie.

Example:
```python
recommend('Avatar')
```

Output:
```
Titan A.E.
Small Soldiers
Independence Day
Ender's Game
Aliens vs Predator: Requirement
```

## Code Structure
- **Data Loading**: Loads and merges the movies and credits datasets.
- **Data Cleaning**: Processes genres, keywords, cast, and crew data.
- **Feature Engineering**: Combines features into a single 'tags' column for each movie.
- **Vectorization**: Uses CountVectorizer to convert text data into numerical vectors.
- **Similarity Calculation**: Computes cosine similarity between movies.
- **Recommendation Function**: Provides movie recommendations based on similarity scores.

## Future Improvements
- Integrate user preferences for personalized recommendations.
- Deploy the system as a web application using Flask or Django.
- Enhance the recommendation algorithm with collaborative filtering.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## Contact
For any questions or suggestions, feel free to reach out:
- Email: isunandapatra@gmail.com
- GitHub: [Sunandaa22](https://github.com/Sunandaa22)


https://github.com/Sunandaa22