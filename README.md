🎬 Movie Revenue Prediction with Random Forest

This project predicts the box office revenue of movies using machine learning. The model is trained on the TMDB 5000 Movie Dataset, and uses features like budget, popularity, runtime, and vote statistics to make predictions.


📌 Problem Statement

Can we predict how much revenue a movie will earn using information available before its release?
This project attempts to answer this using supervised machine learning techniques.


💡 Project Highlights

✅ Used Random Forest Regressor for final model

✅ Tuned model using max_depth=10 for better performance

✅ Compared with Linear Regression for benchmarking

✅ Visualized actual vs predicted revenue


📊 Dataset Used

tmdb_5000_movies.csv
tmdb_5000_credits.csv
Source: Kaggle TMDB Movie Dataset

🧪 Features Used

Feature	Description

budget	Estimated production budget
popularity	Popularity score from TMDB
runtime	Movie duration (minutes)
vote_average	Average user rating
vote_count	Number of user votes
release_year	Year of release


🔧 Model & Evaluation

✅ Final Model: Random Forest Regressor

from sklearn.ensemble import RandomForestRegressor

model = RandomForestRegressor(max_depth=10, random_state=42)
model.fit(X_train, y_train)

📈 Evaluation Metrics:

Mean Absolute Error (MAE): ₹40,102,608

R² Score: 0.73


> These results show the model can predict revenue with reasonable accuracy given limited features.


📉 Visual Output

A plot comparing actual vs predicted revenue:

---

📦 Installation

Install required libraries:

pip install -r requirements.txt


📁 Project Structure

├── movie_revenue_prediction.ipynb
├── requirements.txt
├── README.md
└── data/
    ├── tmdb_5000_movies.csv
    └── tmdb_5000_credits.csv



🚀 Future Improvements

Add NLP analysis from movie overview or genres

Include director or cast popularity

Build a web app using Streamlit


✨ Author

Farid Shaikh,

#An Undergraduate Student
#Passionate about real-world ML projects
