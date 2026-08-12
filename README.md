# spx-tail-risk-volatility
Empirical analysis of S&amp;P 500 tail risk, GARCH volatility, VaR and SPX implied volatility.
# SPX Tail Risk and Volatility Modelling

Empirical analysis of S&P 500 return distributions, conditional volatility,
Value-at-Risk and the SPX implied-volatility surface.

## Overview

This repository contains the Python analysis developed for my bachelor's
thesis in International Economics and Finance at Bocconi University.

The project investigates whether heavy-tailed return distributions and
GARCH models improve the measurement of S&P 500 tail risk and examines how
downside risk is reflected in SPX option-implied volatility.

## Methodology

- Analysed 8,817 daily S&P 500 Total Return Index observations
- Tested return normality and examined crisis-period effects
- Estimated Normal, Student-t and Lévy-stable distributions
- Compared GARCH(1,1) models under Normal and Student-t innovations
- Backtested dynamic 99% Value-at-Risk forecasts
- Analysed the SPX implied-volatility surface across maturities

## Key Results

- Student-t improved AIC by 2,264 relative to the Normal distribution
- GARCH-t reduced the 99% VaR violation rate from 2.27% to 1.10%
- SPX 25-delta risk reversals ranged from -4.76% to -6.71%

## Repository Structure

- `notebooks/`: Python notebooks used for the empirical analysis
- `figures/`: selected graphical results
- `thesis.pdf`: complete thesis
- `requirements.txt`: Python dependencies

## Data Availability

The analysis uses S&P 500 Total Return Index data obtained through CRSP/WRDS
and SPX option data obtained from OptionMetrics IvyDB via WRDS.

The source datasets are proprietary and are therefore not included in this
public repository. The notebooks retain selected outputs so that the
methodology and results can be reviewed without access to the underlying data.

Users with appropriate data licences can reproduce the analysis by placing
the required files in a local `data/` directory adjacent to the `notebooks/`
directory.

## Tools

Python, NumPy, pandas, SciPy, Matplotlib and Excel.

## Author

Francesca Giosa  
BSc International Economics and Finance, Bocconi University
