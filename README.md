# Formula 1 Race Winner Predictor 🏎️🏁

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![ML](https://img.shields.io/badge/machine%20learning-random%20forest-orange)
![License](https://img.shields.io/badge/license-MIT-green)

A machine learning model that predicts Formula 1 race winners based on historical data (1950-2020).

Usage
Run the Jupyter notebook:

bash
jupyter notebook Formula1prediction-checkpoint.ipynb
Sample Input:

Enter driver name (e.g., hamilton): hamilton
Enter constructor/team (e.g., mercedes): mercedes
Enter starting grid position (e.g., 1): 1
Enter race year (e.g., 2020): 2020
Enter round (e.g., 1): 2
Enter circuit (e.g., silverstone): silverstone
Enter weather (Sunny/Rainy/Cloudy): sunny

Dataset
From Kaggle:
results.csv
races.csv
drivers.csv
constructors.csv
circuits.csv

Model Architecture
python
RandomForestClassifier(
    n_estimators=100,
    random_state=42
)

Dependencies
pandas
scikit-learn
numpy
kagglehub


## Features
- Predicts race winners with ~85% accuracy
- Considers 7 key factors: Driver, Team, Grid Position, Year, Round, Circuit, Weather
- Interactive CLI for predictions
- Uses Random Forest Classifier

## Installation
```bash
git clone https://github.com/yourusername/formula1-prediction.git
cd formula1-prediction
pip install -r requirements.txt
