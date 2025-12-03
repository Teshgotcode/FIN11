# FIN11: Holiday Effects on Oslo Børs Microstructure

This repository contains a sophisticated Jupyter notebook for empirical research on the Oslo Stock Exchange. It focuses on analyzing bid-ask spreads and trading volumes with respect to calendar-driven events, such as Christmas, Easter, and the summer holiday period. The notebook automates all data processing and statistical inference, supporting rigorous academic or practitioner analysis.

## Key Features

*   **Spread Estimator Options:** Choose between Corwin-Schultz (2012) and Abdi-Ranaldo (2017) spread estimators using an intuitive notebook flag.[1]
*   **Automated Holiday/Event Tagging:** Trading days are strictly classified as control or event periods (Christmas, Easter, summer) using Norwegian holiday calendars and well-documented calendar logic.[1]
*   **Advanced Hypothesis Testing:** All statistical comparisons use a Bonferroni correction for familywise error rate (FWER). FDR (Benjamini-Hochberg) values are also reported for transparency, but only Bonferroni governs the main conclusions.[1]
*   **Visualizations:** High-quality plots and heatmaps summarize the effect sizes and statistical significance for all periods, groups, and main estimates.[1]
*   **Panel Regression and Robustness:** Fixed-effects panel regressions investigate determinants of spread, controlling for volatility and volume. Robustness checks enable you to exclude COVID-19 years or compare estimator choices.[1]
*   **Execution/Backtesting Component:** For recent years, the notebook simulates market-order versus limit-order strategies to quantify the liquidity premium and actual cost savings of trading during the summer period.[1]

## How to Use

*   The notebook downloads and processes all Norwegian equity data (2014–2024) directly from Yahoo Finance.[1]
*   Spread estimation, event tagging, output generation, and summary visualizations are fully automated.[1]
*   All code cells are thoroughly commented for clarity and extension.

## Intended Audience

This tool is designed for students, researchers, and practitioners interested in market microstructure, transaction costs, and calendar effects in Norwegian equity markets.[1]

**For details on figures, regression outputs, and code usage, see the Code and Output in this repository.**
