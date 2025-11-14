# FIN11: Holiday Effects on Oslo Børs Microstructure

This repository offers a robust Jupyter notebook for analyzing bid-ask spreads and trading volume on the Oslo Stock Exchange with a focus on public holidays and summer vacation periods.

## Main Features

- **Spread estimator selection:** Choose between Corwin-Schultz (CS, 2012) and Abdi-Ranaldo (AR, 2017) methods, settable at the top of the notebook.
- **Event period assignment:** Automatically tags trading dates as holiday or control periods (Christmas, Easter, summer).
- **Multiple testing correction:** All statistical comparisons use Bonferroni-corrected p-values for strict inference.  
  - FDR (Benjamini-Hochberg) is also included in output tables for reference, but **only Bonferroni is used in main results**.
- **Visualizations:** Includes pointplots, barplots, and heatmaps of period/comparison group effects.
- **Regression analysis:** Panel regressions analyze spread determinants, with clear controls for robustness.
- **Robustness checks:** Methods provided to exclude COVID-19 years and compare estimator results.

## Usage

- Automatically downloads data for all Norwegian stocks (2014–2024) from Yahoo Finance (ticker lists grouped by market cap).
- Spread and liquidity metrics, event labeling, and statistical output are fully automated.
- Well-commented code for clarity and extensibility.

## Estimator Options

Corwin-Schultz (CS) and Abdi-Ranaldo (AR) provide alternative, robust ways to estimate bid-ask spreads from daily price data. Select your preferred approach by changing a flag at the start.

## Multiple Testing Correction

All event-based hypothesis tests are corrected for familywise error using Bonferroni.  
- FDR-corrected p-values are shown for reference, but **not used for formal inference**.

## Intended Audience

This code was originally developed for a term paper in the course FIN11.  
It is used to validate the empirical analysis and findings described in the paper, but can also serve as a foundation for further research on Norwegian market microstructure around holidays and event periods.


---
