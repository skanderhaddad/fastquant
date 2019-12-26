# psequant
Framework for applying quantitative finance on PSE data with the goal of promoting data driven investments in the Philippines

# Getting started
```
from pse_pipeline import get_pse_data
df = get_pse_data("JFC", "2018-01-01", "2019-01-01")
print(df.head())
```
# Setup
```
git clone https://github.com/enzoampil/psequant.git
cd psequant
virtualenv env
source env/bin/activate
pip install -r requirements.txt
```
# Run tests
```
pytest test_pse_pipeline.py
```
# Current features:
## Easy access to stock related data (OHLCV)
1. Basic daily price features
    - Date
    - Open
    - High
    - Low
    - Close
    - Value
 2. Company disclosures (WIP)
 3. Company related tweets (WIP)

 # Future features
## Processed text information with NLP
1. Disclosure reports summarized in structured tabular form
2. Summary statistics from tweets

## Easy to use API for back testing trading strategies
1. Example scripts for backtesting on different companies with different trading strategies
2. High level functions for simple backtesting
