# Movie Recommendation System

This project is a movie recommender that uses Singular Value Decomposition (SVD) to extract latent features from movie ratings. It computes similarity scores by comparing a user's average latent vector with all movie embeddings to provide personalized film recommendations. The system is integrated into a Django web application, allowing users to input movie titles and receive recommendations.

## Features

- **Data Processing:** Loads and cleans movie metadata and user ratings.
- **Latent Feature Extraction:** Uses TruncatedSVD to reduce dimensionality and obtain latent vectors.
- **Similarity Computation:** Calculates dot product similarity between a user's average vector and movie embeddings.
- **Web Interface:** A Django-based front-end for inputting movie titles and displaying recommendations.

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/movie-recommender.git
   cd movie-recommender
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare Data:**
   - Place `movies_metadata.csv` and `ratings_small.csv` in the appropriate directory.
   - Run the training script to generate `svd_model.pkl`.

4. **Run the Django server:**
   ```bash
   python manage.py runserver
   ```

## Usage

- Open your browser and go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/).
- Enter movie titles into the provided form to receive personalized recommendations.

## Technologies

- **Python**
- **Pandas & NumPy**
- **Scikit-Learn (TruncatedSVD)**
- **Django**
- **SciPy**

## License

This project is licensed under the MIT License.
