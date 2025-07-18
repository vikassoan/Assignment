# EV Adoption Forecasting

This project forecasts future electric vehicle (EV) adoption using historical registration data from Washington State. The goal is to help urban planners anticipate infrastructure needs, such as charging stations, by predicting EV growth trends.

## Dataset

- **Source:** [Kaggle - Electric Vehicle Population Size 2024](https://www.kaggle.com/datasets/sahirmaharajj/electric-vehicle-population-size-2024/data)
- **File:** `Electric_Vehicle_Population_By_County.csv`
- **Features:**
  - Date (monthly vehicle registration counts)
  - County, State
  - Vehicle Primary Use (Passenger, Truck)
  - Battery Electric Vehicles (BEVs)
  - Plug-In Hybrid Electric Vehicles (PHEVs)
  - Electric Vehicle (EV) Total
  - Non-Electric Vehicle Total
  - Total Vehicles
  - Percent Electric Vehicles

## Workflow

1. **Data Loading:** Loads the dataset using pandas.
2. **Exploration:** Inspects data shape, types, and missing values.
3. **Preprocessing:**
   - Converts date strings to datetime objects.
   - Handles missing values in County and State.
   - Removes rows with invalid dates or missing EV totals.
   - Caps outliers in `Percent Electric Vehicles` using IQR bounds.
4. **Modeling:** (Planned) Build a regression model to forecast future EV adoption.

## Requirements

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- joblib

Install dependencies:
```sh
pip install pandas numpy matplotlib seaborn scikit-learn joblib
```

## Usage

Open and run the notebook [`EV_Adoption_Forecasting.ipynb`](c:/Users/vikas/OneDrive/Desktop/Week_1_Ass/EV_Adoption_Forecasting.ipynb) in Jupyter or Google Colab.

## Output

- Data cleaning and preprocessing steps
- Outlier detection and capping
- Ready-to-use dataset for regression modeling

## License

See dataset source
