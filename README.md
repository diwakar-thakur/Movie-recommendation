# Movie Recommendation System

This project is a content-based movie recommendation system that suggests movies to users based on their input. By using a reference movie, the system identifies and recommends movies with similar content. The recommendation engine leverages Natural Language Processing (NLP) techniques to process movie attributes, and machine learning methods to compute similarity scores between films.

## Project Objective

The objective of this project is to create a movie recommendation system that utilizes text processing techniques to provide personalized movie suggestions. The system converts movie descriptions and attributes into tokenized vectors using Scikit-learn's vectorizer and calculates similarity scores with cosine similarity. Based on the user's input of a reference movie, the system generates recommendation scores, sorts the movies accordingly, and prints the top recommended films.

## Features

- **Text Vectorization**: Converts movie descriptions and other attributes into numerical vectors using the Scikit-learn vectorizer.
- **Cosine Similarity**: Measures the similarity between movies based on their vectorized attributes.
- **User Input Validation**: Uses `difflib` to validate and correct minor spelling errors in the reference movie name.
- **Movie Recommendations**: Generates a sorted list of recommended movies based on similarity scores with the user's chosen reference movie.

## Technologies Used

- **Python**
- **Scikit-learn**: For vectorization and cosine similarity.
- **Pandas**: For dataset manipulation.
- **Numpy**: For numerical computations.
- **Difflib**: For input validation and error correction.

## Project Workflow

1. **Dataset Preparation**: A dataset containing various movie attributes such as titles, genres, descriptions, cast, etc., is used to understand the content of each movie.
2. **Text Vectorization**: Movie descriptions are transformed into tokenized vectors using Scikit-learn's `TfidfVectorizer` or `CountVectorizer`.
3. **Cosine Similarity Calculation**: The similarity between movies is calculated using cosine similarity, which measures the angle between vectors representing different movies.
4. **User Input**: The system takes a movie title from the user to serve as the reference for recommendations.
5. **Input Validation**: The `difflib` library is used to correct minor misspellings and ensure that the movie exists in the dataset.
6. **Recommendation Scoring**: A recommendation score is computed for each movie based on its similarity to the reference movie.
7. **Sorting and Output**: Movies are sorted in descending order based on recommendation scores, and the top recommendations are displayed to the user.


## Example Usage

```
Enter a movie name: Inception
Top 5 Recommended Movies:
1. Interstellar
2. The Matrix
3. The Prestige
4. Memento
5. Blade Runner 2049
```

## Future Enhancements

- **Incorporate Collaborative Filtering**: Enhance the system by combining content-based and collaborative filtering techniques.
- **Improve Model Performance**: Experiment with different NLP techniques and feature engineering to improve the recommendation accuracy.
- **Add User Interface**: Develop a graphical or web-based interface to improve user experience.
