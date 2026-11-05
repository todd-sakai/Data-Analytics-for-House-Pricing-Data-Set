# Predicting House Prices in King County, WA

For this project I built regression models that estimate home sale prices from 21,613 King County, Washington sales (May 2014 to May 2015). The best model, a Ridge regression with degree-2 polynomial features, explains 70% of price variation on a held-out test set (R² = 0.70).

| Model | R² | Evaluated on |
|---|---|---|
| Linear, longitude only | 0.0005 | In-sample |
| Linear, living area only | 0.493 | In-sample |
| Linear, 11 features | 0.658 | In-sample |
| Scale + polynomial + linear pipeline | 0.751 | In-sample |
| Ridge, 11 features | 0.648 | Held-out test |
| Ridge, 11 features, degree-2 polynomial | 0.700 | Held-out test |

Files:
- `king_county_house_prices.ipynb`: Code and outputs
