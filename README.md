# House Price Prediction

![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0%2B-F7931E?logo=scikitlearn&logoColor=white)

**A course project that predicts house sale prices with three regression models.**

| | |
|---|---|
| **Course** | CSE422: Artificial Intelligence, BRAC University |
| **Semester** | Spring 2024 |
| **Type** | Group project |
| **Made by** | Faiaz Abrar Zaman Pronoy and Md. Jahirul Islam Zishan |
| **Version** | v1.0, the course submission |

---

## What it does

1. Loads 1,460 house sales with 19 columns.
2. Drops `Alley` (mostly empty) and `Id`.
3. Fills missing numbers with the mean and missing categories with the mode.
4. One-hot encodes the categories and scales the numbers.
5. Splits the data 70/30 into training and test sets.
6. Trains three models and compares them.

## Models

| Model | Reported R² |
|---|---|
| Linear Regression | 0.999 |
| Decision Tree | 0.999 |
| SVM (SVR, polynomial kernel) | 0.828 |

The two near perfect scores come from a data leak: the price column was still among the inputs. Version 2.0 fixes this.

## Built with

Python, pandas, NumPy, scikit-learn, Matplotlib, seaborn and Graphviz.

## Run it

```bash
pip install -r requirements.txt
jupyter notebook house_price_prediction.ipynb
```

## Project structure

```
house_price_prediction.ipynb   the notebook
data/house_prices.csv          1,460 house sales
report/                        the course report
requirements.txt               Python packages
```

## Data

The [House Prices](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) competition data on Kaggle.

## Authors

- **Faiaz Abrar Zaman Pronoy** (ফাইয়াজ আবরার জামান প্রনয়), lead developer
- **Md. Jahirul Islam Zishan** (মোঃ জহিরুল ইসলাম জিশান)

## Licence

Copyright 2024-2026 Faiaz Abrar Zaman Pronoy and Md. Jahirul Islam Zishan. All rights reserved.
You may read the code and run it to try it out. You may not copy it, hand it in
as your own work, or publish it. See [LICENSE](LICENSE).
