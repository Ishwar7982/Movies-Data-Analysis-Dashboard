# Movies-Data-Analysis-Dashboard
This repository contains a Power BI Dashboard built using a dataset of movies with details such as titles, release years, runtime, genres, awards, and nominations.  The aim of this project is to analyze movies across different dimensions like genres, runtime, awards, and highlight patterns that could provide insights into the film industry.

# Dataset Description

The dataset includes metadata about movies, covering essential attributes.

Columns:

-- tconst – Unique identifier for each movie (IMDb-like format).

-- titleType – Type of title (e.g., movie).

--  primaryTitle – Official movie title.

-- originalTitle – Original release title.

-- startYear – Release year.

-- endYear – End year (if applicable, otherwise \N).

-- runtimeMinutes – Runtime duration in minutes.

-- genres – Movie genres (comma-separated).

-- awards – Number of awards won.

-- nominations – Number of award nominations.

-- best picture – Indicator if nominated/won Best Picture (1 = Yes, 0 = No).


# Dashboard Features

The Power BI dashboard provides the following insights:

🎥 Movie Trends – Number of movies released per year.

⏳ Runtime Analysis – Distribution of movie lengths.

🎭 Genre Popularity – Breakdown of most common genres.

🏆 Awards & Nominations – Analysis of award-winning films.

⭐ Best Picture Highlights – Movies nominated/won in the Best Picture category.

# Visual Insights

Bar Chart – Total Movies by Year:
Shows yearly movie releases from 2014–2018, with 2016 & 2017 as peak years (~14K movies each).

Line Chart – Avg Duration by Year:
Runtime fluctuates, with the highest average runtime in 2015 (84.9 minutes) and lowest in 2017 (82.6 minutes).

Clustered Bar – Awards by Year & Genre:
Comedy & Biography genres dominate awards across multiple years.

Bar Chart – Best Movies & Duration:
Highlights top award-winning movies such as Green Book (130 mins), Spotlight (129 mins), and The Shape of Water (123 mins).

Interactive Filters:
Slicers allow users to filter by Year, Genre, Awards, and Best Picture categories for deeper insights.

# DAX Measures

Some sample DAX calculations used in the dashboard:

-- Total_Movies = COUNTA(Data[tconst])

-- Total_Awards = SUM(Data[awards])

-- Total_Nominations = SUM(Data[nominations])

-- Avg_Duration = AVERAGE(Data[runtimeMinutes])

-- Best_Picture = SUM(Data[best picture])


# BUttons
-- Menu - Show All 4 Butoons

-- Fev Genre - Show Resent 3 year Data with Selected Category.

-- WF Data - Convert  Clustered Bar Chart in a WaterFall Chart.

-- Bar Chart - Convert WaterFall Chart in a Clusteret Bar Chart.

-- Reset - Show the default view.



