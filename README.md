# 🎧 Beyond the Beat
### Understanding Music Through Data

**Beyond the Beat** is a data analysis project focused on exploring Spotify tracks and understanding how musical characteristics relate to track popularity.

Using R, statistical analysis and data visualization, this project aims to discover patterns, identify relationships between audio features and popularity, and explore differences across music genres.

---

## 📌 Table of Contents

- [Project Overview](#-project-overview)
- [Research Questions](#-research-questions)
- [Dataset](#-dataset)
- [Methodology](#-methodology)
- [Technologies](#-technologies)
- [Repository Structure](#-repository-structure)
- [Visualizations](#-visualizations)
- [Interactive Dashboard](#-interactive-dashboard)
- [Installation and Usage](#-installation-and-usage)
- [Expected Outcomes](#-expected-outcomes)
- [Authors](#-authors)

---

## 🔎 Project Overview

Music is more than just sound. Every Spotify track contains measurable characteristics that can help us understand musical patterns and listener preferences.

The main objective of this project is to investigate the relationship between Spotify track popularity and different audio features, such as:

- **Danceability:** How suitable a track is for dancing.
- **Energy:** The intensity and activity of a track.
- **Valence:** The musical positiveness conveyed by a track.
- **Tempo:** The estimated speed of a track in beats per minute.
- **Acousticness:** The likelihood that a track is acoustic.
- **Instrumentalness:** The likelihood that a track contains no vocals.
- **Loudness:** The overall loudness of a track.

Our goal is to use data analysis to identify interesting trends and communicate our findings through clear visualizations.

## ❓ Research Questions

The project will focus on answering the following questions:

1. Is there a relationship between track popularity and energy?
2. Do more danceable tracks tend to have higher popularity?
3. Which music genres have the highest average popularity?
4. Are certain audio features correlated with each other?
5. Does tempo influence the danceability of a track?
6. How do musical characteristics differ across genres?

These questions may be refined as the analysis progresses.

## 📊 Dataset

The project uses a Spotify tracks dataset obtained from Kaggle.

**Dataset source:** [Spotify Tracks Dataset – Kaggle](https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset)

The dataset contains information about tracks, artists, genres, popularity and several audio features.

### Main variables

| Variable | Description |
|---|---|
| `track_name` | Name of the track |
| `artists` | Artist or artists |
| `track_genre` | Music genre |
| `popularity` | Track popularity score |
| `danceability` | Danceability score |
| `energy` | Energy score |
| `valence` | Musical positiveness |
| `tempo` | Tempo in BPM |
| `acousticness` | Acousticness score |
| `instrumentalness` | Instrumentalness score |
| `loudness` | Loudness in dB |
| `duration_ms` | Track duration in milliseconds |

*Note: The final list of variables will be confirmed against the downloaded dataset.*

## ⚙️ Methodology

The project is divided into several stages:

### 1. Data Loading
- Import the original Spotify dataset.
- Inspect its dimensions and structure.
- Identify variable types.

### 2. Data Quality Analysis
- Detect missing values.
- Identify duplicated records.
- Examine potential outliers.
- Evaluate data consistency.

### 3. Data Cleaning
- Handle missing values where appropriate.
- Remove or correct invalid records when justified.
- Prepare the dataset for analysis.

### 4. Data Transformation
Using `dplyr` to:
- Select relevant variables.
- Create new variables.
- Group tracks by genre.
- Calculate descriptive statistics.
- Summarize popularity and audio features.

### 5. Exploratory Data Analysis
- Calculate descriptive statistics.
- Examine variable distributions.
- Explore relationships between numerical variables.
- Investigate differences across genres.

### 6. Data Visualization
Use `ggplot2` to create visualizations that communicate the main findings.

### 7. Interactive Dashboard
Develop a Shiny application to explore the dataset through interactive charts and filters.

## 🛠️ Technologies

The project uses the following tools and technologies:

| Technology | Purpose |
|---|---|
| R | Main programming language |
| DataSpell | Development environment |
| tidyverse | Data manipulation and analysis |
| dplyr | Data transformation |
| ggplot2 | Data visualization |
| Shiny | Interactive dashboard |
| Git | Version control |
| GitHub | Repository and collaboration |

## 📁 Repository Structure

```text
beyond-the-beat/
│
├── README.md
├── .gitignore
│
├── data/
│   ├── raw/
│   ├── processed/
│   └── README.md
│
├── R/
│   ├── 01_load_data.R
│   ├── 02_data_quality.R
│   ├── 03_data_cleaning.R
│   ├── 04_data_transformation.R
│   ├── 05_exploratory_analysis.R
│   ├── 06_correlation_analysis.R
│   └── 07_visualizations.R
│
├── app/
│   └── app.R
│
├── outputs/
│   ├── figures/
│   └── tables/
│
└── docs/
    └── screenshots/
```

## 📈 Visualizations

The following visualizations are planned:

- **Popularity vs. Energy:** Explore the relationship between energy and popularity.
- **Popularity by Genre:** Compare average popularity across music genres.
- **Danceability by Genre:** Investigate differences in danceability.
- **Correlation Heatmap:** Identify relationships between audio features.
- **Tempo vs. Danceability:** Explore the relationship between track tempo and danceability.
- **Audio Feature Distributions:** Examine the distributions of the main musical characteristics.

The final visualizations and their interpretations will be added as the analysis progresses.

## 💻 Interactive Dashboard

An interactive dashboard will be developed using **Shiny**.

It will allow users to:

- Filter tracks by music genre.
- Explore popularity ranges.
- Compare different audio features.
- Visualize relationships between variables.
- Explore the dataset through interactive charts and tables.

More information and screenshots will be added once the application is developed.

## 🚀 Installation and Usage

### Requirements

- R installed on your computer.
- DataSpell or another R-compatible IDE.
- The Spotify dataset downloaded from Kaggle.

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/beyond-the-beat.git
```

### 2. Open the project

Open the cloned repository in DataSpell.

### 3. Install the required packages

```r
install.packages(c(
  "tidyverse",
  "dplyr",
  "ggplot2",
  "shiny"
))
```

### 4. Download the dataset

Download the Spotify dataset from Kaggle and place the original CSV file inside:

```text
data/raw/
```

Follow the dataset's license and usage conditions when downloading or redistributing it.

### 5. Run the analysis

Execute the R scripts in numerical order, starting with:

```text
R/01_load_data.R
```

### 6. Run the Shiny application

Once developed, launch the dashboard using:

```r
shiny::runApp("04-app")
```

## 🎯 Expected Outcomes

By the end of the project, we aim to:

- Understand the relationship between musical characteristics and popularity.
- Identify patterns across different music genres.
- Apply data cleaning and transformation techniques.
- Perform exploratory and statistical analysis.
- Develop meaningful visualizations using ggplot2.
- Build an interactive dashboard with Shiny.
- Present the results in a clear and reproducible way.

**Important:** The analysis will identify associations and patterns, not necessarily causal relationships. Popularity should not be interpreted as a direct measure of musical quality.

## 👥 Authors

**Beyond the Beat** is an academic project developed as part of the Technical and Scientific Programming coursework at the University of Deusto.

---

*Beyond the Beat – Understanding Music Through Data.*
