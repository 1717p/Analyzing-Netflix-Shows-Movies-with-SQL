
# 📺 Netflix Shows & Movies Analysis (SQL Project)

This project presents an analysis of Netflix's content library using **Structured Query Language (SQL)**.

The insights are visualized and presented in a PowerPoint presentation (`.pptx`), which includes key metrics, trends, and summaries based on the Netflix dataset.

---
## 🛠️ Tools Used

- SQL – for data cleaning, filtering, grouping, and analytical queries

- SQLite / MySQL – local RDBMS for running queries

- PowerPoint – for visual storytelling and presenting insights

- Excel / CSV – data formatting and pre-processing (if needed)

## 🔍 Key Questions Explored
📝 Overview
The goal of this project is to explore and analyze Netflix's movie and TV show data using SQL queries. The analysis focuses on:

- Content type distribution (Movies vs TV Shows)
- Country-wise content availability
- Yearly release trends
- Top genres and categories
- Most frequent directors and actors
- Duration and rating distributions
---

## 📁 Netflix_SQL_Presentation/
├──Analyzing Netflix Shows & Movies with SQL.pptx - PowerPoint presentation with insights
├── Dataset used: https://www.kaggle.com/datasets/victorsoeiro/netflix-tv-shows-and-movies?select=titles.csv 



## 📊 Sample SQL Queries

-  Count of Movies vs TV Shows
SELECT type, COUNT(*) AS count
FROM titles
GROUP BY type;

-  Top 10 countries by number of titles
SELECT production_countries, COUNT(*) AS total
FROM titles
GROUP BY production_countries
ORDER BY total DESC
LIMIT 10;

-  Year-wise release trend
SELECT release_year, COUNT(*) AS count
FROM titles
GROUP BY release_year
ORDER BY release_year;


## 📈 Output & Visualization
- The PowerPoint presentation includes:

- Pie charts for content type distribution

- Bar graphs for top countries, genres, and directors

- Timeline trends for yearly releases

- Highlighted insights from SQL results

- Presentation file: Analyzing Netflix Shows & Movies with SQL.pptx

## 🚀 How to Use
- Clone or download this repo.

- Load the titles.csv file into your SQL database.

- Use the provided SQL queries to explore and modify analysis.

- Check the .pptx file to review visual insights and trends.



## 📬 Feedback
If you have suggestions or feedback, feel free to raise an issue or connect with me!
