# Movie_Recommender_Engine
## Problem Statement
The project is divided into two parts: 
* **The Story of Film:** This section aims at narrating the history, trivia and facts behind the world of cinema through the lens of data. Extensive Exploratory Data Analysis is performed on Movie Metadata about Movie Revenues, Casts, Crews, Budgets, etc. through the years.
* **Movie Recommender Systems:** This part is focused around building a recommendation engine; namely the Content Based Filter. The performance of the system is evaluated in both a qualitative and quantitative manner.

## Approach 

The problem was divided into several steps:

1. **Data Collection:** Data was collected from the MovieLens website and through a script that queried for data from various TMDB Endpoints.
2. **Data Wrangling:** The datasets were uploaded to a dataframe and explored. Null values were filled in wherever appropriate and polluted values were discarded or wrangled.
3. **EDA:** Extensive data visualisation and summary statistics were used to extract insights and pattern from the various datasets. The history, facts and trivia behind movies were narrated through data.
4. **Machine Learning:** Gradient Boosting Classifer and Regressor were trained on our feature engineered dataset to predict movie success and revenue respectively. Their feature importances were noted to gain insights into what factors influence the revenues of a movie relative to budget.
5. **Recommendation Systems:** A recommendation system was built using various ideas and algorithms also known as Content Based Filtering.

## Final Results 

A Gradient Boosting Regressor and Classifier were built to predict Movie Revenue and Success respectively with a Score of 0.78 and 0.8 respectively.

In addition, a recommendation engine was built based on similar idea and a different algorithm:

* **Content Based Recommender:** I built two content based engines; one that took movie overview and taglines as input and the other which took metadata such as cast, crew, genre and keywords to come up with predictions. I also devised a simple filter to give greater preference to movies with more votes and higher ratings.


## Repository Structure
1. **movies_data_story_telling.ipynb:** The Jupyter notebook that contains the story telling format of Film.
2. **movies_eda.ipynb:** The Jupyter notebook that contains the EDA and narrates the Story of Film.
3. **movies_recommender_engine.ipynb:** The Jupyter notebook containing code for the recommendation engines
4. **movies_recommender_consolidated_report.pdf:** The Final Report
