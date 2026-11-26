# Movie Similarity - Movie Recommendation System

## About the Project

This project implements a simple movie recommendation system using Python. It finds movies with similar content based on their genres, keywords and descriptions.

The system uses text vectorization and cosine similarity to compare movies and recommend the five most similar titles.

## Dataset

The project uses the **TMDB 5000 Movie Dataset**, available on Kaggle.

The dataset contains information about movies, including:
- Movie titles
- Genres
- Keywords
- Descriptions (overviews)

## Technologies Used

- Python
- Pandas
- Scikit-learn
- Jupyter Notebook

## How It Works

1. Load and explore the movie dataset.
2. Extract genres and keywords from the dataset.
3. Combine genres, keywords and movie descriptions into a single text feature.
4. Convert the text into numerical vectors using `CountVectorizer`.
5. Calculate similarity scores using `cosine_similarity`.
6. Recommend the five most similar movies based on the selected title.

## Example

For the movie **Avatar**, the system recommends titles such as:
- Aliens
- Moonraker
- Starship Troopers
- Mission to Mars
- Alien³

## Limitations

The system compares words rather than understanding their actual meaning. Because of this, some recommendations may not be relevant. The quality of the results also depends on the information available in the dataset.

## How to Run

1. Clone or download this repository.
2. Install the required libraries using:

   `pip install -r requirements.txt`

3. Open `movie_similarity.ipynb` in Jupyter Notebook.
4. Run the notebook cells.

## References

- [TMDB 5000 Movie Dataset - Kaggle](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)
- [CountVectorizer Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.CountVectorizer.html)
- [Cosine Similarity Documentation](https://scikit-learn.org/stable/modules/generated/sklearn.metrics.pairwise.cosine_similarity.html)
