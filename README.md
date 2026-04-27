# MA Crossover Backtesting on the S&P 500 (SPY)

**This project investigates whether simple moving average (MA) crossover strategies can outperform a buy-and-hold approach on the S&P 500 (SPY) using daily data from 2013–2018.**

---

## Methodology
- Backtested MA crossover strategies (20/50, 20/100)
- Included transaction costs (2 bps per trade)
- Evaluated performance using:
  - total return
  - annualised volatility
  - Sharpe ratio
  - maximum drawdown
- Performed parameter sweep across a range of MA pairs
- Conducted a train/test split (2013–2016 / 2017–2018) to assess robustness

---

## Key Findings
- Buy-and-hold outperformed the baseline MA strategies over the full sample  
- Parameter sweep showed no broad, stable optimal region  
- Some parameter regions produced stronger Sharpe ratios in both training and test periods  
- Results were sensitive to parameter choice and sample period  

---

## Limitations
- Single asset (SPY) and relatively short time period  
- Use of unadjusted prices excludes dividends  
- Simplified transaction cost assumptions (no slippage or spreads)  
- Limited out-of-sample testing within a single market regime  

---

## Files
- `ma_crossover_spy_backtest.ipynb` – full analysis  
- `spy_data.csv` – dataset used  

---

## Next Steps
- Extend analysis to other assets (e.g. indices, bonds)  
- Test across different market regimes  
- Incorporate adjusted prices and dividend returns  