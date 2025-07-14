# Movie Recommender System 🎬

A content-based movie recommendation system built with Python, Streamlit, and machine learning.

## Features

- **Interactive Web Interface**: Built with Streamlit for easy movie selection
- **Content-Based Filtering**: Uses movie features like genres, cast, crew, and overview
- **Real-time Poster Fetching**: Fetches movie posters from TMDB API
- **5000+ Movies**: Trained on TMDB dataset with extensive movie information
- **Cosine Similarity**: Uses advanced similarity metrics for accurate recommendations

## How it Works

1. **Data Processing**: Processes movie data including genres, cast, crew, and overview
2. **Feature Engineering**: Creates combined text features from all movie attributes
3. **Vectorization**: Uses CountVectorizer to convert text to numerical vectors
4. **Similarity Calculation**: Computes cosine similarity between movies
5. **Recommendation**: Returns top 5 most similar movies with posters

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/AbdulAhad365/movie-recommender-system.git
   cd movie-recommender-system
   ```

2. **Install dependencies**:
   ```bash
   pip install streamlit pandas numpy scikit-learn requests
   ```

3. **Run the notebook** to generate model files:
   - Open `notebook86c26b4f17.ipynb`
   - Run all cells to generate `movie_list.pkl` and `similarity.pkl`
   - Move these files to the `model/` directory

4. **Run the Streamlit app**:
   ```bash
   streamlit run app.py
   ```

## File Structure

```
movie-recommender-system/
├── app.py                      # Main Streamlit application
├── notebook86c26b4f17.ipynb    # Jupyter notebook with ML pipeline
├── model/
│   ├── movie_list.pkl          # Processed movie data
│   └── similarity.pkl          # Similarity matrix (large file)
├── tmdb_5000_movies.csv        # Original movie dataset
├── tmdb_5000_credits.csv       # Original credits dataset
└── README.md                   # This file
```

## Technologies Used

- **Python**: Core programming language
- **Streamlit**: Web framework for the user interface
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning library
- **TMDB API**: Movie poster and metadata

## Dataset

The system uses the TMDB 5000 Movie Dataset containing:
- 4,803 movies with detailed information
- Movie metadata: genres, keywords, cast, crew
- Movie financials: budget, revenue, ratings

## API Key

The app uses TMDB API for fetching movie posters. The API key is included in the code for demonstration purposes.

## Future Enhancements

- Add collaborative filtering
- Implement user ratings
- Add movie search functionality
- Deploy on cloud platforms
- Add more recommendation algorithms

## License

This project is open source and available under the MIT License.

## Contributing

Feel free to fork this repository and submit pull requests for any improvements.

---

**Made with ❤️ by AbdulAhad365**
