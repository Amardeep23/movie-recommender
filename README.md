# Movie Recommender System

## Overview
This project implements a Movie Recommender System using a content-based approach. The system suggests movies similar to a user-selected movie based on textual data such as movie descriptions, genres, and cast information.

## Table of Contents
- [Dependencies](#dependencies)
- [Installation](#installation)
- [Usage](#usage)
- [Data](#data)
- [Methodology](#methodology)
- [Recommendation](#recommendation)
- [Files](#files)
- [Contributing](#contributing)
- [License](#license)

## Dependencies
- Python 3.x
- Streamlit
- Pandas
- NumPy
- Requests
- Scikit-Learn
- NLTK (Natural Language Toolkit)

You can install the required packages using pip:
```bash
pip install streamlit pandas numpy requests scikit-learn nltk
Installation
Clone the repository to your local machine:
bash
Copy code
git clone https://github.com/yourusername/movie-recommender.git
Change the directory to the project folder:
bash
Copy code
cd movie-recommender
Run the Streamlit app:
bash
Copy code
streamlit run movie_recommender.py
Visit the local URL provided by Streamlit in your web browser.
Usage
Select a movie from the dropdown menu.
Click the "Recommend" button to view the top 5 recommended movies based on similarity to the selected movie.
Data
The project uses movie data from the TMDb 5000 Movie Dataset available on Kaggle. It consists of movie details, cast, and crew information.

Methodology
Data Preprocessing: Data was cleaned, missing values were handled, and relevant features were selected.
Text Processing: Movie descriptions, genres, and cast information were processed to create tags for each movie.
Text Vectorization: Bag of Words (BoW) was used to convert text data into numerical features.
Similarity Calculation: Cosine similarity was used to calculate the similarity between movies.
Recommendation Generation: A function was created to recommend similar movies based on user input.
Recommendation
The system recommends movies based on content similarity. For a given movie, it suggests movies with similar textual content, such as plot descriptions, genres, and cast.

Files
movie_recommender.py: The main Python script that contains the Streamlit app and recommendation logic.
tmdb_5000_movies.csv: Dataset containing movie details.
tmdb_5000_credits.csv: Dataset containing cast and crew information.
movies_dict.pkl: Pickled file containing movie data.
similarity.pkl: Pickled file containing the similarity matrix.
Contributing
Contributions are welcome! If you have any improvements or suggestions, please open an issue or create a pull request.

License
This project is licensed under the MIT License - see the LICENSE file for details.
