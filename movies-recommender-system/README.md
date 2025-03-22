# Movie Recommender System

This is a simple movie recommender system built using Python and Streamlit. It recommends movies based on a selected movie and displays their posters using data from The Movie Database (TMDb) API.

## Features

- Recommends 5 movies similar to the selected movie.
- Displays movie posters fetched from TMDb API.
- Interactive UI built with Streamlit.

## Project Structure
movies-recommender-system/ ├── app.py # Main application file ├── movie_dict.pkl # Pickle file containing movie data ├── movies.pkl # (Optional) Additional movie data ├── similarity.pkl # Pickle file containing similarity matrix ├── MRS.ipynb # Jupyter notebook for experimentation └── .idea/ # IDE configuration files

## Requirements

- Python 3.7 or higher
- Streamlit
- Pandas
- Requests

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movies-recommender-system.git
   cd movies-recommender-system
   ```
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Add your TMDb API key in the fetch_poster function in app.py:
   To fetch movie details from TMDb API, use the following  code:
   ```python
   response = requests.get('https://api.themoviedb.org/3/movie/{}?api_key=YOUR_API_KEY&language=en-US'.format(movie_id))
   ```
4. Run the application:
   ```bash
   streamlit run app.py
   ```
5. Open the application in your browser at http://localhost:8501.

## Usage
1. Select a movie from the dropdown menu.
2. Click the "Recommend" button to get 5 similar movies along with their posters

## Screenshots
<img alt="Screenshot 1" src="C:\Users\91798\OneDrive\Pictures\Screenshots\Screenshot 2025-03-22 134510.png">

<img alt="Screenshot 2" src="C:\Users\91798\OneDrive\Pictures\Screenshots\Screenshot 2025-03-22 134536.png">

<img alt="Screenshot 3" src="C:\Users\91798\OneDrive\Pictures\Screenshots\Screenshot 2025-03-22 134558.png">

Example of the application interface.

## License
This project is licensed under the [MIT License](LICENSE). See the LICENSE file for details.

## Acknowledgments
- [The Movie Database (TMDb)](https://www.themoviedb.org/) for providing the movie data and API.
- Streamlit for the interactive UI framework.