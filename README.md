Name: Nidhi Naidu ,
Email: nidhi.naidu@gwu.edu

# Content-Based Movie Recommendation System

## Overview
This project is a **content-based recommendation system** that suggests movies based on user preferences. The system utilizes **TF-IDF vectorization** and **cosine similarity** to compare user input with movie descriptions from a dataset and recommend the most relevant titles.

## Features
- Takes a **short text description** of user preferences.
- Processes and **vectorizes** movie descriptions.
- Computes **cosine similarity** between user input and movie dataset.
- Returns the **top N most similar movies** with their details and similarity scores.

## Dataset
- The dataset used is `imdb_top_250.csv`, containing:
  - `movie_name`: Title of the movie
  - `year_of_release`: Release year
  - `IMDb_score`: IMDb rating
  - `genre`: Movie genre(s)
  - `Plot`: Movie synopsis
  - `directors` and `cast` information
- Ensure `imdb_top_250.csv` is in the same directory as the script.

## Installation & Setup
### Prerequisites
- Python 3.x
- Install required libraries:
  ```bash
  pip install pandas scikit-learn
  ```

## Usage
Run the recommendation script:
```bash
python recommend.py
```
Enter a short description of the type of movies you enjoy, and the system will return top recommendations.

### Example
**User Input:**
```bash
I like action movies set in space
```
**Output:**
```
Top 5 movie recommendations based on your preference ('I like action movies set in space'):

1. Blade Runner (1982) - Action, Drama, Sci-Fi - IMDb: 8.1
2. The Iron Giant (1999) - Animation, Action, Adventure - IMDb: 8.1
3. It's a Wonderful Life (1946) - Drama, Family, Fantasy - IMDb: 8.6
4. Bicycle Thieves (1948) - Drama - IMDb: 8.3
5. The Lord of the Rings: The Fellowship of the Ring (2001) - Adventure, Drama, Fantasy - IMDb: 8.9
```

## Code Structure
- `recommend.py` : Main script for running recommendations
- `imdb_top_250.csv` : Movie dataset
- `README.md` : Project documentation

## Demo Video
[https://www.loom.com/share/2ae742f29dee40b99fadd81eb05746e2?sid=ffe2c932-4875-4cc3-9a2e-e71e7e6f6d1c]

## License
This project is open-source under the MIT License.

