# Quant Lab

**A live, public, honest scoreboard for AI stock-picking.**
Open it: https://satvikjain2507-star.github.io/quant-lab-site/

Can AI really beat the stock market? Quant Lab tests that question in the open.
Machine-learning models are trained on 20 years of prices, tested without
hindsight, and then run live as paper portfolios. Every portfolio pays real
trading costs and is scored against a fair benchmark, Equal weight, which
simply holds every stock.

## What is on the site

| Page | What it shows |
| --- | --- |
| Portfolios | 17 live paper portfolios in India, the USA and global funds: value, profit and loss, holdings, orders, and why each stock was picked |
| Scoreboard | Every model against Equal weight in its own market: ahead or behind, after costs |
| Check a stock | Type any of 1,000+ stocks and see the model's rank for it today, and the reasons |
| You vs AI | Pick your own stocks and race the models under the same rules |
| How it works | The pipeline, the 20-year backtest, and the bias we found in our own test |

The site installs on a phone like an app (Add to Home screen) and works offline.

## How it works

1. **Collect** daily prices for the Nifty 500, the S&P 500 and 24 global funds.
2. **Clean** splits, demergers, bad ticks and unfinished trading days.
3. **Learn**: models score every stock from 17 signals, retrained monthly on past data only.
4. **Decide** on the last trading day of each month, using that day's closing prices.
5. **Trade** at the next open, paying brokerage, STT, stamp duty, GST and slippage.
6. **Publish**: the ledgers are rebuilt into this page automatically every week.

## What keeps it honest

- A fair yardstick: Equal weight in the same market, not a flattering index.
- Real Indian trading costs on every order.
- No look-ahead: decide on today's close, trade at tomorrow's open.
- A survivorship test that removed most of the backtest edge, published as found.
- Forward results in public. The history is never edited.

## Built with

Python, pandas and NumPy for data, models and the trading engine; plain HTML,
CSS and JavaScript for the site; GitHub Pages for hosting. No servers and no
paid services.

This repository holds only the published page. The research code is private.

Built by Satvik Jain. A research and learning project: nothing here is
investment advice.
