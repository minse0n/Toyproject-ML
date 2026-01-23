# Toyproject-ML

## 1. Predict KBO games using mlp

**Dataset:**
* Merged 3 seasons (2023–2025) of KBO data (~2,135 games)
* Merged 2 seasons (2024.June–2025) of KBO data (~1000 games)
* **`csv/`**: Sliced 2025 data files categorized by batter, pitcher, and scoreboard records from library `kbodata`
  
**Features (12 inputs):** 
* Home/Away team’s last 30-game avg runs scored/allowed.
* Home/Away team’s last 30-game batting average.
* Starting pitcher's season avg runs allowed.
* Team's total win % and Home/Away win %.


**Model**

* **Algorithms:** Tested **SGD, ADAM, and L-BFGS** using Scikit-learn and PyTorch.
* **Architecture:** Settled on a Multilayer Perceptron (MLP) with **3 to 12 hidden nodes** and **Tanh/ReLU** activation.
* **Scaling:** Applied `StandardScaler`
* **Overfitting Management:** Used **Dropout** and **Weight Decay** in PyTorch


## 2. others
#### Data

* **`kbo_regular_seasons_result.csv`**: Historical team performance (1982–2025) including Win/Loss records, BA, ERA, and WPCT from Kaggle
* **`postseasons_result.csv`**: Yearly postseason placements and rankings by Team ID.
* **`data/raw/`**: Comprehensive historical batting and pitching statistics (1982–2025)

* **`year_data_2025.json`**: Detailed game-level data for 2025 (scoreboards, play-by-play events, umpires, audience metrics)

* **`data/ranked/`**: Processed datasets containing expanded ranking features.
* **Top-level CSVs**: Refined datasets prepared for immediate modeling.


#### Other Notebooks

* **`ml.ipynb`** & **`TabNet_SW.ipynb`**: Machine learning models for ranking and postseason prediction,TabNet, Time Series
* **`Rank_process.ipynb`**: Logic for rank processing and data transformation
* **`test.ipynb`**: data extracting from kbodata library 
