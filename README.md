# 📽️ MovieLens Analysis with PySpark

## Overview
This project explores the **MovieLens 20M Dataset** using **Apache Spark** with the **PySpark DataFrame API**. It demonstrates how to perform scalable data analysis on large datasets using Spark in a Jupyter Notebook environment.

## 🔍 Goals
Using PySpark, we analyze movie ratings to answer:
- 🎬 What are the most popular movies?
- 🌟 What are the top-rated movies?
- ⚖️ Which movies are the most polarizing?

## 📁 Dataset
- Source: [MovieLens 20M Dataset](https://grouplens.org/datasets/movielens/20m/)
- Description: Contains 20 million ratings and tag applications across 27,000+ movies.
- Files used:
  - `movies.csv`
  - `ratings.csv`

## 🛠️ Technologies
- Python
- PySpark
- Jupyter Notebook
- Apache Spark
- PyCharm

## 📊 Analysis Highlights
- **Data Loading**: Read CSV files into Spark DataFrames.
- **Aggregations**: Count ratings, compute averages, and standard deviations.
- **Joins**: Merge movie metadata with rating statistics.
- **Filtering**: Focus on movies with a minimum number of ratings.
- **Insights**:
  - Most popular movies by rating count.
  - Top-rated movies with sufficient ratings.
  - Most polarizing movies based on rating variability.

## 📈 Sample Output

### Most Popular Movies (by number of ratings)
| Movie Title               | Number of Ratings |
|---------------------------|-------------------|
| Pulp Fiction (1994)       | 67,310            |
| Forrest Gump (1994)       | 66,172            |
| Shawshank Redemption (1994)| 63,366           |
| Silence of the Lambs (1991)| 63,299           |
| Jurassic Park (1993)      | 59,715            |

### Top Rated Movies (with ≥ 500 ratings)
| Movie Title               | Average Rating | Number of Ratings |
|---------------------------|----------------|-------------------|
| Shawshank Redemption      | 4.45           | 63,366            |
| The Godfather             | 4.36           | 41,355            |
| The Usual Suspects        | 4.33           | 47,006            |
| Schindler’s List          | 4.31           | 50,054            |
| Godfather: Part II        | 4.28           | 27,398            |

### Most Polarizing Movies (highest rating standard deviation)
| Movie Title               | Avg Rating | Num Ratings | Std Dev |
|---------------------------|------------|-------------|---------|
| Dungeons & Dragons        | 2.07       | 2,047       | 1.11    |
| Spawn (1997)              | 2.62       | 5,255       | 1.09    |
| Dirty Dancing (1987)      | 3.21       | 11,013      | 1.13    |
| Hellbound: Hellraiser II | 2.92       | 1,246       | 1.13    |
| Across the Universe       | 3.67       | 1,687       | 1.02    |

---

## 📚 Further Exploration

Here are some ideas to expand the analysis:

- 🎭 **Genre-Based Insights**: Explore how different genres perform in terms of ratings and popularity.
- 📅 **Temporal Trends**: Analyze how movie ratings change over time or by release year.
- 🧠 **Recommender System**: Build a collaborative filtering model to suggest movies to users.
- 🌍 **User Demographics**: If available, analyze rating patterns across different user groups.
- 🧪 **Sentiment Analysis**: Combine with external reviews or tags to assess viewer sentiment.
