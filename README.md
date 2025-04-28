# Multi-Exchange-Stock-Quote-Classifier

## Overview
This project is part of the Applied Machine Learning course and aims to analyze and predict the optimal currency/exchange for executing stock price quotes. The provided dataset contains a time series of bid and ask prices for a given stock traded multiple times per day in different currencies. The goal is to develop and compare several classification models to determine which currency offers the best price at each time point.

## Project Name Suggestion
**Multi-Exchange Stock Quote Classifier**

## Dataset
- **File:** `price_data_multicurrency.csv`
- **Format:** CSV
- **Contents:** Time-stamped bid and ask prices of a stock in multiple currencies/exchanges.

## Prerequisites
- Python 3.8+
- A virtual environment (venv or Conda) activated

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Menashe-Lorenzi/tomato-yields-analysis.git
   cd tomato-yields-analysis
   ```
2. Create and activate a virtual environment (if not already done):
   ```bash
   python -m venv .venv
   source .venv/bin/activate        # macOS/Linux
   .\.venv\Scripts\activate      # Windows
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Load the dataset and preprocess:
   ```python
   import pandas as pd
   df = pd.read_csv('price_data_multicurrency.csv')
   ```
2. Train classification models to predict the best currency/exchange:
   ```bash
   python train_model.py --data price_data_multicurrency.csv
   ```
3. Evaluate and compare model performance:
   ```bash
   python evaluate.py --model output/my_model.pkl
   ```

## Project Structure
```
├── .venv/                        # Virtual environment
├── data/
│   └── price_data_multicurrency.csv
├── notebooks/
│   └── analysis.ipynb           # Exploratory data analysis
├── src/
│   ├── train_model.py
│   ├── evaluate.py
│   └── utils.py
├── requirements.txt
└── README.md
```

## Contributing
Feel free to submit issues or pull requests for improvements.

## License
This project is licensed under the MIT License.")}

