# Predicting House Prices in King County, WA

Capstone project for *Data Analysis with Python* (IBM Data Science Professional Certificate), by Todd Sakai.

Regression models that estimate home sale prices from 21,613 King County, Washington sales (May 2014 to May 2015). The best model, a Ridge regression with degree-2 polynomial features, explains 70% of price variation on a held-out test set (R² = 0.70).

| Model | R² | Evaluated on |
|---|---|---|
| Linear, longitude only | 0.0005 | In-sample |
| Linear, living area only | 0.493 | In-sample |
| Linear, 11 features | 0.658 | In-sample |
| Scale + polynomial + linear pipeline | 0.751 | In-sample |
| Ridge, 11 features | 0.648 | Held-out test |
| Ridge, 11 features, degree-2 polynomial | 0.700 | Held-out test |

Files: `king_county_house_prices.ipynb` (code and outputs), `King County House Prices - Todd Sakai.pdf` (report without code), `king_county_house_prices_report.html` (the same report as a web page).

Run it with Python 3, pandas, seaborn, matplotlib and scikit-learn. The notebook loads `kc_house_data_NaN.csv` from its own folder if present, and otherwise downloads it from IBM's course server. Data source: [Kaggle house sales dataset](https://www.kaggle.com/harlfoxem/housesalesprediction).
