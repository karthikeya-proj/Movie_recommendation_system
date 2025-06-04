#  Movie Recommendation System

A Python-based Movie Recommendation System that suggests movies similar to a user's favorite selection. This project utilizes content-based filtering techniques and provides an interactive interface for users to explore movie recommendations.

---

## Features

- **Content-Based Filtering**: Recommends movies based on similarity in genres, keywords, and other metadata.
- **User-Friendly Interface**: Interactive prompts for user input and displaying recommendations.
- **Data Visualization**: Presents recommendations in a readable format.
- **Extensible Codebase**: Modular design allows for easy enhancements and integration with other systems.

---

## Tools & Technologies

- **Programming Language**: Python 3.x
- **Libraries & Packages**:
  - `pandas`: Data manipulation and analysis.
  - `numpy`: Numerical operations.
  - `scikit-learn`: Machine learning algorithms for computing similarities.
  - `nltk`: Natural language processing for text preprocessing.
  - `pickle`: Object serialization for saving and loading models.
  - `os`: Interacting with the operating system.
  - `warnings`: Handling warning messages.

---

## 📁 Project Structure

```
├── movie_recommendation (1).py       # Main Python script containing the recommendation logic
├── README.md                         # Project documentation
├── Screenshot 2024-07-27 114206.png  # Screenshot of the application
```

---

## Dataset

The project uses a dataset named `movies.csv`, which includes the following columns:

- `title`: Title of the movie.
- `genres`: Genres associated with the movie.
- `keywords`: Keywords describing the movie.
- `overview`: Brief summary of the movie.
- `cast`: Main cast members.
- `crew`: Crew members, including directors and writers.
  
  ####
   [Download Dataset. ](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)


---

## How It Works

1. **Data Preprocessing**:
   - Combines relevant features (`genres`, `keywords`, `cast`, `crew`) into a single string.
   - Converts text to lowercase and removes spaces for uniformity.

2. **Vectorization**:
   - Uses `CountVectorizer` from `scikit-learn` to convert text data into numerical vectors.

3. **Similarity Computation**:
   - Calculates cosine similarity between movie vectors to determine similarity scores.

4. **Recommendation Generation**:
   - Based on the user's favorite movie, retrieves the top 5 most similar movies.

---

## Getting Started

### Prerequisites

Ensure you have Python 3.x installed. Install the required packages using pip:

```bash
pip install pandas numpy scikit-learn nltk
```

### Running the Application

1. Clone the repository:

```bash
git clone https://github.com/karthikeya-proj/Movie_recommendation_system.git
cd Movie_recommendation_system
```

2. Run the Python script:

```bash
python "movie_recommendation (1).py"
```

3. Follow the on-screen prompts to enter your favorite movie and view recommendations.

#

## Future Enhancements

- **Web Interface**: Integrate with web frameworks like Flask or Django for a web-based UI.
- **Collaborative Filtering**: Incorporate user-based recommendations using collaborative filtering techniques.
- **Enhanced NLP**: Utilize advanced NLP models for better understanding of movie descriptions.
- **Real-Time Data**: Fetch and update movie data in real-time from external APIs like TMDB.

---

## 🤝 Contributing

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

---


---

## Contact

For any queries or suggestions, please contact [karthikeya-proj](https://github.com/karthikeya-proj).
