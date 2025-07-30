---

# NHL Salary Predictor Model

This project uses machine learning to predict NHL player salaries based on their performance statistics and team salary cap data. The model scrapes live contract data from `capwages.com` and merges it with a provided set of player performance ratings.

The primary goal is to determine which statistical features are most indicative of a player's salary in the league.

***
## 📊 Data Sources

* **Live Salary Data:** Pulled dynamically from [capwages.com](https://capwages.com/) for all 32 NHL teams.
* **Player Ratings Data:** Sourced from the included `PlayerRatings.xlsx` file. This data includes advanced metrics for skaters who have played a minimum of 20 games in the 2024 season (even strength only).

***
## 🚀 Model Performance

A multiple linear regression model was trained using the combined data. The performance of this initial model is as follows:

* **Mean Absolute Error (MAE):** **$1,460,923**
    * This means, on average, the model's salary prediction is off by approximately $1.46 million.
* **R-squared (R²):** **0.576**
    * This indicates that the model's features explain about 57.6% of the variance in player salaries.

***
## 🛠️ How to Run

The entire process, from data scraping to model training and evaluation, is contained within the Jupyter Notebook.

1.  Ensure both `Wage_Predictor_NHL.ipynb` and `PlayerRatings.xlsx` are in the same directory.
2.  Open the notebook in an environment like Google Colab or a local Jupyter instance.
3.  Click **"Run all"** (`Runtime` -> `Run all` in Google Colab).
4.  Scroll to the bottom of the notebook to see the final merged DataFrame and the model performance summary.

***
## 🔮 Future Improvements

This project serves as a solid baseline. Potential next steps include:
* Adding more features like player age and contract term.
* Exploring more complex models (e.g., Random Forest, Gradient Boosting) to capture non-linear relationships.
* Performing hyperparameter tuning to further optimize model performance.
