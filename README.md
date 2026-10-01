# YouTube Channel Analysis Dashboard

A Data Analysis Essentials project for exploring and visualizing YouTube channel data. The project includes a Jupyter Notebook for analysis, a cleaned CSV dataset, and an interactive HTML dashboard.

## Project Structure

```text
youtube-channel-analysis/
├── dashboard.html
├── youtube_4k_channels_cleaned.csv
├── youtube_channel_analysis.ipynb
├── README.md
└── .gitignore
```

## Files

### `youtube_channel_analysis.ipynb`

Jupyter Notebook containing the project's data-analysis work.

### `youtube_4k_channels_cleaned.csv`

Cleaned YouTube channel dataset used by the project.

### `dashboard.html`

Interactive browser-based dashboard for exploring the dataset. The dashboard includes sections for:

- Overview
- Top Channels
- ML Insights
- Data Table

It calculates channel-level metrics and provides visual analysis such as distributions, comparisons, correlations, country/tier summaries, top-channel views, growth/trending indicators, and K-Means clustering.

## Dashboard Features

The dashboard processes channel data and derives metrics including:

- Subscribers
- Total views
- Total videos
- Views per video
- Subscribers per video
- Engagement proxy
- Channel-level averages and totals
- Growth score
- Trending index
- K-Means clusters

The dashboard also displays key performance indicators such as total channels, total subscribers, total views, median subscribers, average engagement, and unique countries when those fields are available in the loaded dataset.

## How to Run the Dashboard

### Option 1: Open the HTML file

You can open `dashboard.html` in a modern web browser. If the browser blocks local CSV loading, use a local web server instead.

### Option 2: Run a local server

From the project directory, run:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000/dashboard.html
```

The dashboard can also accept a CSV through its upload/drag-and-drop interface.

## Notebook

To work with the Jupyter Notebook locally, install Jupyter and the required Python packages used by the notebook. Then start Jupyter from the project directory:

```bash
jupyter notebook
```

Open `youtube_channel_analysis.ipynb` and run the cells as required.

## Git Setup

If you are creating the repository locally for the first time:

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/youtube-channel-analysis.git
git push -u origin main
```

Replace `YOUR-USERNAME` with your GitHub username.

## Technologies Used

- Python / Jupyter Notebook
- HTML
- JavaScript
- CSV data
- Papa Parse
- Chart.js
- Chart.js Matrix plugin
- K-Means clustering and standardized numerical features in the dashboard

## Project Purpose

The project demonstrates data cleaning, exploratory data analysis, feature engineering, visualization, and basic machine-learning-oriented analysis using YouTube channel data.

## Notes

The dashboard's growth score and trending index are composite indicators calculated from the available channel metrics. They are intended as project-level analytical indicators rather than official YouTube metrics.
