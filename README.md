# Amazon Prime Video Data Analysis

![Demo](Res/recording.gif)

## Introduction

This proje involves an exploratory data analysis (EDA) of the Amazon Prime Video content catalog. The primary goal is to uncover insights into the types of content available, popular genres, prolific directors, content ratings, and trends in content release over the years.

## Dataset

The analysis is based on the `amazon_prime_titles.csv` dataset, which contains information about movies and TV shows available on Amazon Prime Video. Each row represents a unique title and includes details such as:

* `show_id`: Unique ID for every show/movie
* `type`: Type of content (Movie or TV Show)
* `title`: Title of the movie or TV show
* `director`: Director(s) of the content
* `cast`: Main actors/cast members
* `country`: Country of production
* `date_added`: Date when the content was added to Prime Video
* `release_year`: The year the content was originally released
* `rating`: Content rating (e.g., 13+, R, TV-MA)
* `duration`: Duration of the movie (in minutes) or TV show (number of seasons)
* `listed_in`: Genres/categories
* `description`: Short description of the content

## Data Analysis & Exploratory Data Analysis (EDA)

The following key insights were derived from the analysis:

### 1. Content Type Distribution

The dataset primarily consists of **Movies**, significantly outnumbering **TV Shows**.

* Movies: 7814 titles
* TV Shows: 1854 titles

### 2. Average Movie Duration

The average duration for movies on Amazon Prime Video is approximately **91.31 minutes**.

### 3. Top Directors

The most prolific directors (those with the highest number of titles) include:

1. **Mark Knight**: 114 titles
2. **Cannis Holder**: 62 titles
3. **Moonbug Entertainment**: 37 titles
4. **Jay Chapman**: 34 titles
5. **Arthur van Merwijk**: 30 titles

### 4. Common Content Ratings

The most frequently occurring content ratings are:

* `13+`
* `16+`
* `ALL`
* `18+`
* `R`

### 5. Top Genres

The most popular genres (categories) for content on the platform are:

1. **Drama**: 3687 titles
2. **Comedy**: 2099 titles
3. **Action**: 1657 titles
4. **Suspense**: 1501 titles
5. **Kids**: 1085 titles

### 6. Release Year Distribution

The analysis of `release_year` indicates a strong trend towards more recent content being added. There has been a significant increase in the number of titles released, particularly from **2019 to 2021**.

### 7. Missing Values

During the EDA, missing values were identified in several key columns:

* `director`: 2082 missing values
* `cast`: 1233 missing values
* `country`: 8996 missing values (very high)
* `date_added`: 9513 missing values (very high)
* `rating`: 337 missing values

The high number of missing values in `country` and `date_added` suggests these columns might require significant imputation or external data for meaningful analysis, or may be excluded from analyses where their completeness is critical.
