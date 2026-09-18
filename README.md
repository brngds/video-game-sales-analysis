# 🎮 Video Game Sales Analysis

Exploratory and statistical analysis of global video game sales to identify market trends, regional preferences, and factors associated with commercial success.

## 📌 Context

The online store **Ice** sells video games worldwide and wants to better understand the characteristics associated with successful game releases.

Historical information about game sales, platforms, genres, critic reviews, user reviews, and ESRB ratings is available through 2016.

The objective of this project is to analyze these historical patterns and generate insights that could support the planning of marketing campaigns for 2017.

## 🎯 Business Questions

The analysis focuses on several key questions:

- How has the number of game releases changed over time?
- Which gaming platforms generated the highest historical sales?
- How long do gaming platforms typically remain commercially relevant?
- Which platforms appear most relevant for the upcoming market period?
- How do critic and user reviews relate to game sales?
- Which game genres tend to generate stronger sales?
- How do platform and genre preferences differ across regions?
- Does ESRB rating appear to influence regional sales?
- Are user ratings significantly different across selected platforms and genres?

## 📊 Dataset

The project uses the `games.csv` dataset containing historical information about video game releases and sales.

### Main Variables

- `name` — game title
- `platform` — gaming platform
- `year_of_release` — release year
- `genre` — game genre
- `na_sales` — North American sales
- `eu_sales` — European sales
- `jp_sales` — Japanese sales
- `other_sales` — sales in other regions
- `critic_score` — professional critic score
- `user_score` — user review score
- `rating` — ESRB age/content rating

Regional sales are expressed in millions of units.

## 🔎 Analytical Approach

The project follows the workflow below:

1. Load and inspect the dataset
2. Standardize column names
3. Review data types and missing values
4. Handle `"TBD"` values in user scores
5. Calculate total global sales for each game
6. Analyze game releases over time
7. Examine historical platform sales and platform life cycles
8. Define the most relevant period for forecasting the 2017 market
9. Identify leading and potentially relevant platforms
10. Compare global sales distributions across platforms
11. Analyze the relationship between reviews and sales
12. Compare performance of games across multiple platforms
13. Analyze sales patterns by genre
14. Build regional customer profiles for North America, Europe, and Japan
15. Evaluate the relationship between ESRB ratings and regional sales
16. Perform statistical hypothesis tests
17. Summarize findings and business implications

## 🧹 Data Preparation

The preprocessing stage includes:

- Standardizing column names
- Converting variables to appropriate data types
- Investigating missing values
- Treating `"TBD"` user scores as unavailable ratings
- Reviewing potential data inconsistencies
- Creating a `total_sales` variable from regional sales

These steps create a consistent analytical dataset for the exploratory and statistical analysis.

## 📈 Market & Platform Analysis

Historical sales are analyzed by year and platform to understand how the video game market evolves over time.

The analysis investigates:

- Platform sales trends
- Platform life cycles
- Growing and declining platforms
- Sales distributions
- Potentially relevant platforms for the upcoming period

## ⭐ Reviews & Commercial Performance

Critic and user scores are compared with game sales using:

- Scatter plots
- Correlation analysis
- Cross-platform comparisons

This helps evaluate whether stronger reviews are associated with stronger commercial performance.

## 🎯 Genre Analysis

Game genres are analyzed to understand differences in commercial performance and identify categories associated with stronger or weaker sales patterns.

## 🌎 Regional Market Profiles

Separate market profiles are developed for:

- North America
- Europe
- Japan

For each region, the analysis examines:

- Leading platforms
- Leading genres
- Market share differences
- ESRB rating patterns

This highlights how consumer preferences differ across geographic markets.

## 🧪 Statistical Hypothesis Testing

Two hypotheses are evaluated using statistical tests.

### Xbox One vs. PC

The analysis tests whether the average user ratings for **Xbox One** and **PC** games are statistically different.

### Action vs. Sports

The analysis tests whether the average user ratings for **Action** and **Sports** games are statistically different.

Null and alternative hypotheses are explicitly defined, and conclusions are based on a predefined significance level.

## 💡 Business Applications

The insights from this analysis can support:

- Marketing campaign planning
- Platform prioritization
- Regional marketing strategies
- Genre-focused promotions
- Identification of commercially promising game segments
- Better allocation of advertising resources

## ⚠️ Limitations

The dataset contains historical information only through 2016, and data for 2016 may be incomplete.

Sales patterns in the video game industry can also be influenced by factors not included in the dataset, such as marketing investment, franchise popularity, hardware availability, digital distribution, competition, and broader market conditions.

Therefore, the findings should be interpreted as historical analytical insights rather than precise forecasts of future game sales.

## 🛠️ Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Jupyter Notebook
- Exploratory Data Analysis
- Statistical Hypothesis Testing

## 📁 Repository Structure

```text
video-game-sales-analysis/
│
├── README.md
│
├── data/
│   └── games.csv
│
└── notebook/
    └── video_game_sales_analysis.ipynb
```

## 📌 Project Goal

This project demonstrates an end-to-end analytical workflow combining data preprocessing, exploratory data analysis, visualization, regional market analysis, and statistical hypothesis testing to generate actionable insights from historical video game sales data.
