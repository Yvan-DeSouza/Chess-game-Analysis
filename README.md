♟️ Chess Data Analysis

This project performs an exploratory data analysis (EDA) on a chess games dataset to explore how player levels and time controls influence game outcomes, as well as analyzing popular chess openings.

🏆 Project Overview

Goal: Understand how player skill levels (Beginner, Intermediate, Advanced) and game time controls (Blitz, Rapid, Long Rapid) affect chess outcomes (mate, resign, outoftime, draw).

Dataset: games.csv containing player info, ratings, results, number of turns, time controls, and openings.

Tools: Python 3, Pandas, NumPy, Matplotlib

🛠️ Data Processing

⏱️ Time Control Classification

Extracted base time from increment_code.

Categories:

Blitz (≤5 min) ⚡

Rapid (6–29 min) ⏩

Long Rapid (≥30 min) 🐢

🎯 Player Level Classification

Average rating of both players computed.

Categories:

Beginner (≤1400) 🟢

Intermediate (1401–1799) 🟡

Advanced (≥1800) 🔴

➕ Additional Columns

game_type: Time control category.

level: Player skill level.

higher_rating: Player with the higher rating in each game.

📊 Key Visualizations

Game Outcomes 🎨

Bar plot showing distribution of outcomes: mate, resign, outoftime, draw.

Turns by Player Level 🧮

Boxplot showing number of turns played for each skill level.

Outcomes by Time Control ⏳

Stacked bar chart showing outcomes across Blitz, Rapid, and Long Rapid games.

Distribution of Player Levels 📈

Pie chart showing proportion of games played by Beginners, Intermediates, and Advanced players.

Wins by Player Color ⚪⚫

Pie chart showing wins for white, black, and draws.

Correlation of Rating Difference and Outcome 📊

Stacked bar chart showing outcomes based on which player had the higher rating.

Top Chess Openings by Level 📖

Bar charts showing the five most frequently played openings per skill level.

🔍 Insights

Game outcomes are influenced by player rating and time control.

White slightly wins more often than black, while draws are rare.

Certain openings are more popular among specific skill levels.

Blitz games tend to finish faster and have more out-of-time results.

🚀 How to Use

Clone the repository:

git clone <repository-url>


Install dependencies:

pip install -r requirements.txt


Run the notebook:

jupyter notebook Chess_Analysis.ipynb

📦 Requirements

Python 3.8+ 🐍

Pandas 🐼

NumPy 🔢

Matplotlib 📊

Jupyter Notebook (optional) 💻

🌟 Future Work

Fix the heatmap generation issue (convert set to list).

Build ML models to predict game outcomes based on player rating, level, and opening.

Create interactive dashboards using Plotly or Dash.
