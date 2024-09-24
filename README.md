# Movie-recommendation-first-ML

This project is a simple movie recommendation system built using Python. It takes your favorite movie as input and recommends similar movies based on various features such as genres, keywords, tagline, cast, and director. The system uses **TF-IDF** (Term Frequency-Inverse Document Frequency) for text vectorization and **cosine similarity** to find movies that are most similar to your input.

## How it Works

1. The dataset is loaded from a CSV file containing information about movies.
2. Several movie features (genres, keywords, tagline, cast, and director) are selected and combined into a single string for each movie.
3. The combined features are converted into numerical vectors using **TF-IDF** vectorization.
4. **Cosine similarity** is used to calculate the similarity between movies.
5. Given a movie title as input, the system suggests a list of similar movies based on the computed similarity.

## Libraries Used

- `numpy` - For numerical operations
- `pandas` - For handling and processing the movie dataset
- `scikit-learn`:
  - `TfidfVectorizer` - For vectorizing text data
  - `cosine_similarity` - For calculating the similarity between feature vectors
- `difflib` - For finding close matches of movie titles

## Installation

To run this project, you'll need to install the required libraries:

```
pip install numpy pandas scikit-learn
```
## Dataset
The project uses a CSV file (`movies.csv`) that contains information about movies. Make sure your dataset has the following columns:

- **index**: Index of the movie
- **title**: Title of the movie
- **genres**: Genres of the movie
- **keywords**: Keywords related to the movie
- **tagline**: Tagline of the movie
- **cast**: Main cast of the movie
- **director**: Director of the movie

## Running the Project
1.Clone this repository.
2.Place your `movies.csv` dataset file in the project directory.
3.Run the script or notebook.
4.Enter your favorite movie name when prompted.
5.The system will suggest similar movies based on the selected features.

## Example
```
Enter your favorite movie name: Inception
Movies suggested for you:
1. Inception
2. Interstellar
3. The Prestige
4. The Dark Knight
5. Memento
6. The Matrix
7. The Dark Knight Rises
8. The Social Network
9. Shutter Island
```
## Future Improvements
- Improve the recommendation by adding more features such as runtime, release year, etc.
- Implement a user-friendly interface for better interaction.
- Explore more sophisticated models to enhance recommendation accuracy.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
