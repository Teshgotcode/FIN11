# FIN11: Holiday Effects on Oslo Exchange Microstructure

This repository contains an advanced Jupyter notebook for empirical analysis of bid-ask spreads and trading volume on the Oslo Stock Exchange, with particular emphasis on effects around public holidays and the summer vacation period. The code was developed for a FIN11 term paper and features fully automated data processing and robust statistical inference.

## Main Features

- **Spread estimator selection:** Use either Corwin-Schultz (CS, 2012) or Abdi-Ranaldo (AR, 2017). Select your method at the top of the notebook.
- **Automatic period tagging:** Trading days are labeled as either control or event periods (Christmas, Easter, summer) using strict calendrical logic.
- **Stringent hypothesis testing:** All comparisons implement Bonferroni correction for familywise error. FDR (Benjamini-Hochberg) is also reported for reference, but only Bonferroni governs main results.
- **Visualizations:** Includes point plots, bar plots, and heatmaps summarizing effect sizes for each period or group.
- **Panel regression:** Fixed-effects panel regressions analyze the determinants of spreads, with thorough controls for volatility and trading volume patterns.
- **Robustness checks:** Options to exclude COVID-19 years and compare results across spread estimators are included.

## Usage

- Downloads data automatically for all Norwegian stocks (2014–2024) from Yahoo Finance, grouped by market capitalization.
- Spread and liquidity metrics, event assignment, and full statistical output are streamlined and thoroughly commented for easy extension.
- Output includes exported tables as well as figures from regression and hypothesis test analyses.

## Estimator Options

Corwin-Schultz (CS) and Abdi-Ranaldo (AR) offer complementary approaches for estimating bid-ask spreads from daily price data. Method selection is made via a simple flag.

## Multiple Testing Correction

All event-driven hypothesis tests employ strict Bonferroni correction—FDR is reported for transparency only. Tables include both sets of p-values.

## Robustness and Extensibility

- Option to exclude COVID-19 years and validate sensitivity to estimator choice or input series.
- Panel regression outputs are formatted for further academic analysis or publication.

## Intended Audience

The notebook is suited for students and researchers in finance, quantitative analysis, or market microstructure, as well as practitioners interested in event-driven transaction cost analysis on the Oslo Stock Exchange.
