# 📺 Netflix Content Analysis (EDA with Python)

## 🔍 Overview

This project explores Netflix’s content library using real-world data. It dives into trends related to **movies and TV shows**, analyzing genres, top actors/directors, and optimal content release timing. The analysis also examines how long it typically takes for movies to be added to Netflix after their original release.

---

## 🎯 Objectives

- Clean and structure the Netflix dataset
- Analyze TV shows vs movies by region and type
- Identify top contributing countries, directors, and actors
- Uncover genre and category trends using word clouds
- Detect best months/weeks for releasing content
- Study the average delay between theatrical release and Netflix addition

---

## 📦 Dataset

- Source: Netflix content dataset (CSV)
- Total entries: ~8,800 raw → exploded to ~200,000 after unnesting
- Fields used: title, type, director, cast, country, date_added, release_year, rating, listed_in, duration

---

## 🔧 Tools & Libraries

- Python (`pandas`, `numpy`, `matplotlib`, `seaborn`)
- Word cloud (`wordcloud`)
- Jupyter Notebook / Google Colab

---

## 🔍 Key Steps & Features

### 📊 Data Cleaning & Preprocessing
- Converted `date_added` to datetime
- Split and exploded multivalued fields like `cast`, `country`, `director`, and `listed_in`
- Derived fields: `movie_minutes`, `show_seasons`, `week_added`, `month_added`, and `days_to_add`

### 📈 Exploratory Data Analysis

- **Type distribution**: Movies vs TV Shows
- **Top countries** by number of titles
- **Top actors** in movies & TV shows
- **Top directors** by unique works
- **Best week/month** to release content
- **Days between theatrical release and Netflix addition** (histogram & boxplot)
- **Genre analysis** using word cloud
- **Annual content trends** (TV vs Movie growth over years)

---

## 📊 Visualizations Included

- Bar plots for:
  - Top countries, actors, and directors
  - Content additions per year
- Word cloud for genre distribution
- Line chart: Weekly and monthly content additions
- Histogram and boxplot: Delay in movie release vs Netflix availability

---

## 📌 Key Insights

- 📅 **Best week for movies**: Week 1 (316 releases)
- 📅 **Best week for TV shows**: Week 27 (85 releases)
- 📅 **Best month overall**: July for both movies & shows
- 🎬 **Top Movie Actor**: Vatsal Dubey (13 unique movies)
- 📺 **Top TV Actor**: David Attenborough (14 shows)
- 🎥 **Top Director (Movies)**: Rajiv Chilaka (19 titles)
- 🌍 **Top content-producing countries**: US, India, UK, Canada, France

---

## 📘 Lessons Learned

- Multivalue columns (like `cast`, `listed_in`) require unnesting for proper insights
- Dates can be mined deeply for release strategies
- Real-world EDA benefits from blending visual storytelling with domain knowledge

---


