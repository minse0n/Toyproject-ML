# Toyproject-ML


## Notebooks

* **`ml.ipynb`** & **`TabNet_SW.ipynb`**: Machine learning models for ranking and postseason prediction,TabNet, Time Series
* **`Rank_process.ipynb`**: Logic for rank processing and data transformation
* **`test.ipynb`**: data extracting from kbodata library 
## 2. Core Datasets

### Data

* **`kbo_regular_seasons_result.csv`**: Historical team performance (1982–2025) including Win/Loss records, BA, ERA, and WPCT from Kaggle
* **`postseasons_result.csv`**: Yearly postseason placements and rankings by Team ID.
* **`data/raw/`**: Comprehensive historical batting and pitching statistics (1982–2025)

* **`year_data_2025.json`**: Detailed game-level data for 2025 (scoreboards, play-by-play events, umpires, audience metrics)
* **`csv/`**: Sliced 2025 data files categorized by batter, pitcher, and scoreboard records.

* **`data/ranked/`**: Processed datasets containing expanded ranking features.
* **Top-level CSVs**: Refined datasets prepared for immediate modeling.
