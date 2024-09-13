# Tech Stock Analysis: Impact of Interest Rates on Higher Moments

## Introduction

This project investigates the impact of interest rate changes on the risk profiles of major tech stocks, focusing on higher moments (skewness and kurtosis) . By examining these often-overlooked statistical measures, we aim to provide a more comprehensive understanding of stock behavior during periods of changing interest rates.

## Methodology

Our analysis follows these key steps:
1. Data collection for tech stocks and interest rates (2018-2024)
2. Calculation of returns and higher moments (mean, standard deviation, skewness, kurtosis)
3. Identification of periods with decreasing interest rates
4. Comparison of stock behavior during normal periods vs. periods of decreasing rates
5. Analysis of correlations and tail risks

We use Python for data processing and analysis, leveraging libraries such as pandas, numpy, and scipy for statistical calculations, and plotly for visualization.

## Data

- **Stock Data**: Daily adjusted closing prices for AAPL, AMZN, GOOGL, MSFT, NVDA, and TSLA (2018-2023)
- **Interest Rate Data**: Daily Federal Funds Rate (2018-2023)

Data sources: Yahoo Finance (stocks) and FRED (Federal Reserve Economic Data) for interest rates.

## Key Findings

1. **Asymmetry Shifts**: During rate decreases, AMZN and TSLA show increased positive skewness (0.85 and 0.34), while MSFT and GOOGL become more negatively skewed (-1.64 and -1.49).

2. **Increased Tail Risks**: Kurtosis spikes for most stocks during rate cuts (e.g., MSFT: 6.63 to 14.85), indicating higher probability of extreme events.

3. **Volatility Changes**: AAPL and MSFT show 33.9% and 32.2% volatility increases respectively during rate decreases.

4. **Correlation Dynamics**: Significant shifts in stock correlations, affecting diversification strategies.

5. **Tail Risk Metrics**: Conditional Value at Risk (CVaR) worsens for most stocks during rate decreases, with AAPL's CVaR rising from -4.47% to -7.27%.

## Implications for Investors

- Reassess risk models to account for changing higher moments during interest rate fluctuations.
- Adjust portfolio weights based on new risk-reward profiles revealed by skewness and kurtosis changes.
- Prepare for potentially larger drawdowns, even in a decreasing rate environment.
- Regularly review diversification strategies as correlations shift during different rate regimes.

## Limitations

1. **Time Period Specificity**: The 2018-2023 period may not represent all economic cycles or interest rate regimes.
2. **Sample Size**: Focusing on six tech stocks limits the generalizability of findings.
3. **Assumption of Stationarity**: The analysis assumes relationships between interest rates and stock behavior remain constant, which may not hold over longer periods.
4. **Omitted Variables**: Other factors (e.g., company-specific news, broader market trends) that could influence stock behavior are not accounted for.
5. **Lag Effects**: The analysis doesn't consider potential delayed impacts of interest rate changes on stock behavior.


## Future Work

- Extend the analysis to a broader range of stocks and sectors.
- Incorporate machine learning models to predict changes in higher moments based on interest rate movements.
- Develop a real-time dashboard for monitoring these metrics.
- Investigate the impact of other macroeconomic factors on higher moments.

## Contributing

Contributions to this project are welcome! Please fork the repository and submit a pull request with your proposed changes.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.

---

