# 📊 Netflix Data Analysis and Dashboard

This project explores Netflix content data to uncover patterns and trends using data cleaning, transformation, and visualization. The analysis was performed using Python (in Jupyter Notebook) and Tableau Public. Final insights are presented through an interactive dashboard that separates movies and TV shows for clearer analysis.

---

## 🧹 Data Cleaning & Preparation

The original dataset included both movies and TV shows in a single CSV file, with various formatting inconsistencies. The cleaning process involved:

- **Handling Missing Values**: Removed or replaced rows with missing `cast`, `director`, `country`, or `date_added` information where necessary.
- **Date Parsing**: Converted `date_added` into proper datetime format for time-based visualizations.
- **Duration Parsing**: Split the `duration` column into:
  - `duration_value` (e.g., 90, 2, etc.)
  - `duration_unit` (e.g., minutes, seasons)
- **Country Count**: Created a `country_count` column to capture how many countries were listed per record (by splitting comma-separated country values).
- **Filtering Content Types**: Used the `type` column to separate the dataset into two new files:
  - `tv_data.csv` (TV Shows only)
  - `movies_data.csv` (Movies only)
- **Dropped Unnecessary Columns**: The `type` column was dropped after filtering since it was redundant.

---

## 📁 Output Files

- `tv_data.csv`: Cleaned dataset for Netflix TV Shows
- `movies_data.csv`: Cleaned dataset for Netflix Movies

These were loaded into Tableau as **separate data sources** for independent analysis.

---

## 📊 Dashboard Features

The Tableau dashboard displays the following key visuals:

- 🎬 **Top 10 Movie Directors** — Bar chart showing the most frequently appearing movie directors.
- 📺 **Top 10 TV Show Genres** — A breakdown of the most common genres in TV shows using a horizontal bar chart.
- ⏳ **Top 5 Longest Running TV Shows** — Highlights TV shows with the highest number of seasons using a sorted bar chart.
- 📈 **Movie Releases Over Time** — A line chart showing that Netflix has increasingly released newer movies in recent years.
- 🧮 **Movie Ratings Distribution** — A pie chart visualizing the percentage of movies by rating category (e.g., PG, R, TV-MA).
- 🌍 **TV Show Genres by Country** — A chart showing genre preferences across different countries.

Each visualization allows filtering and interaction, offering viewers multiple ways to explore the data.

---

## ⚙️ Tools & Technologies Used

- **Python** (Pandas) — Data cleaning and transformation
- **Jupyter Notebook** — For data preprocessing and exploration
- **Tableau Public** — Dashboard creation and data visualization
- **GitHub** — Project tracking and documentation

---


## ✅ Future Improvements

- Add interactivity across movie and TV data using parameters or blended sources.
- Normalize and analyze overlapping genres or countries more deeply.
- Introduce user-focused metrics like average watch time (if data is available).

---

Feel free to explore, clone, or build on this project for your own data analysis practice!

Source: Kaggle datasets
