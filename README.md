Chess Data Analysis

This project performs an exploratory data analysis (EDA) on a dataset of chess games to investigate how player levels and time controls influence game outcomes. The analysis also explores popular chess openings and their distribution among different skill levels.

Project Overview

Goal: To understand how different player levels (Beginner, Intermediate, Advanced) and game time controls (Blitz, Rapid, Long Rapid) affect chess outcomes (mate, resign, outoftime, draw).

Dataset: Chess games dataset (games.csv) containing information about players, ratings, game results, number of turns, time control, and openings.

Tools: Python 3, Pandas, NumPy, Matplotlib

Data Processing

Time Control Classification:

Extracted the base time from increment_code.

Categorized games into:

Blitz (≤5 min)

Rapid (6–29 min)

Long Rapid (≥30 min)

Player Level Classification:

Computed the average rating of both players.

Categorized into:

Beginner (≤1400)

Intermediate (1401–1799)

Advanced (≥1800)

Additional Columns:

game_type: Stores the time control category.

level: Stores the player skill level.

higher_rating: Indicates which player had a higher rating in each game.

Key Visualizations

Game Outcomes:

Bar plot showing distribution of outcomes (mate, resign, outoftime, draw) across all games.

Turns by Player Level:

Boxplot showing the number of turns played for each skill level.

Outcomes by Time Control:

Stacked bar chart showing outcomes across Blitz, Rapid, and Long Rapid games.

Distribution of Player Levels:

Pie chart showing proportion of games played by Beginners, Intermediates, and Advanced players.

Wins by Player Color:

Pie chart showing win distribution for white, black, and draw outcomes.

Correlation of Rating Difference and Outcome:

Stacked bar chart showing outcomes based on which player had the higher rating.

Top Chess Openings by Level:

Bar charts showing the five most frequently played openings per skill level.

Insights

Outcomes are influenced by both player rating and time control.

White slightly wins more often than black, with draws being relatively rare.

Certain openings are more popular among specific skill levels.

Blitz games tend to finish faster and have more out-of-time results.

How to Use

Clone the repository:

git clone <repository-url>


Install dependencies:

pip install -r requirements.txt


Run the analysis notebook to generate plots:

jupyter notebook Chess_Analysis.ipynb

Requirements

Python 3.8+

Pandas

NumPy

Matplotlib

Jupyter Notebook (optional, for running the notebook)

Future Work

Fix the heatmap generation for opening differences by converting the index set to a list.

Explore machine learning models to predict game outcomes based on player rating, level, and opening.

Interactive dashboards using Plotly or Dash for better visualization.
