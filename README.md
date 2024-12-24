# Movie Recommendation System

This project is a **Movie Recommendation System** built using Python, Streamlit, and scikit-learn. The application provides movie recommendations based on user input and displays relevant movie posters by fetching data from the TMDB API.

---

## Features
- **Movie Recommendations**: Suggests five similar movies based on the selected movie.
- **Poster Display**: Fetches and displays posters for the recommended movies.
- **Interactive UI**: Built with Streamlit for a user-friendly interface.

---

## Tech Stack
- **Frontend**: Streamlit
- **Backend**: Python
- **Libraries Used**:
  - `pandas` for data manipulation
  - `scikit-learn` for machine learning and similarity calculations
  - `requests` for API calls
  - `pickle` for saving and loading pre-processed data

---

## Dataset
The system uses a pre-processed dataset that includes:
- Movie titles
- Movie IDs
- Tags for each movie

---

## Installation

### Prerequisites
- Python 3.8+
- pip (Python package manager)

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/Movie-Recommendation-System.git
   cd Movie-Recommendation-System
   ```

2. Install required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Install Git LFS (if handling large files like `similarity.pkl`):
   - [Install Git LFS](https://git-lfs.github.com/)
   - Initialize Git LFS:
     ```bash
     git lfs install
     ```

4. Add your TMDB API key in the `fetch_poster` function in `app.py`:
   ```python
   response = requests.get('https://api.themoviedb.org/3/movie/{movie_id}?api_key=YOUR_API_KEY&language=en-US')
   ```

5. Run the application:
   ```bash
   streamlit run app.py
   ```

---

## Usage
1. Open the Streamlit application in your browser.
2. Select a movie from the dropdown menu.
3. Click the **Show Recommendation** button to view recommended movies and their posters.

---

## File Structure
```
Movie-Recommendation-System/
├── app.py                # Main application file
├── movie_dict.pkl        # Pre-processed movie data
├── similarity.pkl        # Similarity matrix
├── requirements.txt      # Python dependencies
├── .gitattributes        # Git LFS configuration
└── README.md             # Project documentation
```

---

## Issues and Debugging
1. **Large File Issue**:
   - Use Git LFS to handle files larger than 100 MB (e.g., `similarity.pkl`).

2. **API Errors**:
   - Ensure your TMDB API key is valid and has the correct permissions.

3. **Module Errors**:
   - Ensure all dependencies are installed using `pip install -r requirements.txt`.

---

## Future Improvements
- Add a search functionality to find movies not listed in the dropdown.
- Include user ratings to improve recommendation accuracy.
- Use collaborative filtering for better recommendations.

---

## License
This project is licensed under the MIT License. Feel free to use and modify it as needed.

---

## Acknowledgments
- **TMDB API**: For providing movie data and posters.
- **Streamlit**: For the easy-to-use interface.
- **scikit-learn**: For machine learning tools.

---

## Screenshort
![Screenshot 2024-12-24 121819](https://github.com/user-attachments/assets/5d22023f-0657-43f4-acb2-e6865e1f6ff0)


## Contact
For any questions or suggestions, please contact:
- **Name**: Shivam Kumar
- **GitHub**: [https://github.com/shivamkrmnnit]

