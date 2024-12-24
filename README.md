
# Recommendation Systems

This repository contains an implementation of a hybrid recommendation system combining collaborative filtering and content-based filtering. It recommends movies to users based on their past ratings and movie tags.

## Features

- **Collaborative Filtering**: Recommends movies based on user similarity using cosine similarity.
- **Content-Based Filtering**: Recommends movies similar to a given movie based on movie tags using TF-IDF and cosine similarity.
- **Hybrid Approach**: Combines collaborative and content-based filtering for enhanced recommendations.

## Dataset

The recommendation system uses the following datasets:
1. **movies.csv**: Contains movie metadata (e.g., title, genres).
2. **ratings.csv**: Contains user ratings for movies.
3. **tags.csv**: Contains user-assigned tags for movies.

You can use the sample data from the data folder or use any other dataset from different sources

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/recommendation-systems.git
   cd recommendation-systems
   ```

2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Place the dataset files (`movies.csv`, `ratings.csv`, `tags.csv`) in the appropriate directory.

## Usage

Run the script to generate movie recommendations:
```bash
python recommendation_system_with_tags.py
```

### Example Output
```text
Movies recommended for User 2 based on hybrid approach: ['Movie 1', 'Movie 2', 'Movie 3', 'Movie 4', 'Movie 5']
```

### Customization
- To provide a specific movie for content-based filtering, set the `movie_title` parameter in the `hybrid_recommend_movies` function.
- Adjust the number of recommendations (`n`) as needed.


## Requirements

See [requirements.txt](requirements.txt) for a list of dependencies.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
