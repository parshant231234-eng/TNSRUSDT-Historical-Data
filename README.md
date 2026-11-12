# TNSRUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **TNSRUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `TNSRUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `32` months
- **Total Candles:** `1,364,190` 1-minute candles
- **Historical Range:** `2024-04-08 15:30:00` to `2026-11-11 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
TNSRUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── TNSRUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/TNSRUSDT-Historical-Data/main/1m/2026/11/TNSRUSDT_1m_2026-11.csv"
df = pd.read_csv(url)
print(df.head())
```
