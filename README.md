# Cryptocurrency Correlation Analysis Dashboard 📊💰

This repository contains a Power BI dashboard project that provides an in-depth analysis of cryptocurrency correlation patterns across 1000+ digital assets. The dashboard helps investors and analysts make data-driven portfolio decisions by identifying correlation relationships, volatility patterns, and diversification opportunities in the crypto market.

## Table of Contents
- [Introduction](#introduction)
- [Data Preparation](#data-preparation)
- [Key Performance Indicators (KPIs)](#key-performance-indicators-kpis)
- [Dashboard Features](#dashboard-features)
- [Advanced DAX Calculations](#advanced-dax-calculations)
- [Insights and Analysis](#insights-and-analysis)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)

## Introduction
Cryptocurrency portfolio diversification is often misunderstood, with many investors believing their assets are uncorrelated when they actually move together during market stress. This dashboard addresses this critical gap by providing real-time correlation analysis and statistical insights to help build truly diversified crypto portfolios.

## Data Preparation
The dataset includes:
- **1000+ cryptocurrency assets** with daily price data
- **OHLCV data** (Open, High, Low, Close, Volume)
- **Time series analysis** spanning multiple market cycles
- **Custom date tables** for advanced time-based calculations

Data was cleaned and processed using Power Query, with relationships established between date tables and crypto data for optimal performance.

## Key Performance Indicators (KPIs)
- **Correlation Coefficient**: Real-time correlation between any two crypto assets
- **Daily Return %**: Percentage change in asset prices
- **Volatility %**: Market volatility calculations using high-low spreads
- **Price Change**: Absolute difference between open and close prices
- **Volume Analysis**: Trading volume patterns and top performers

## Dashboard Features
✅ **Interactive Correlation Matrix**: Select any two cryptocurrencies to see their correlation coefficient
✅ **Volatility Tracking**: Real-time volatility measurements across all assets
✅ **Time-Based Analysis**: Filter by date ranges to see how correlations change over time
✅ **Top Volume Insights**: Identify highest trading volume assets
✅ **Portfolio Diversification Tools**: Visual indicators for portfolio risk assessment

## Advanced DAX Calculations
The dashboard features sophisticated DAX measures including:
- Custom correlation coefficient formulas
- Statistical variance calculations (X², Y², XY)
- Dynamic date table relationships
- Complex filtering for multi-asset analysis

```dax
Correlation Coeff = 
DIVIDE(
    [n]*[XY] - [X]*[Y],
    SQRT(
        ([n]*[X^2] - [X]^2) * ([n]*[Y^2] - [Y]^2)
    )
)
```

## Insights and Analysis
Key findings from the analysis:
- **Correlation Clusters**: Identification of highly correlated asset groups
- **Market Stress Patterns**: How correlations spike during volatility
- **Diversification Opportunities**: Assets with low or negative correlations
- **Volume-Correlation Relationships**: Trading activity impact on price relationships

## Recommendations
To further enhance portfolio management using this dashboard:

**Incorporate Predictive Analytics**: Integrate machine learning models to forecast correlation changes during market events.

**Enhance Real-Time Monitoring**: Connect to live crypto APIs for continuous correlation tracking.

**Add Risk Metrics**: Include Value at Risk (VaR) calculations and portfolio optimization suggestions.

**Expand Asset Coverage**: Include DeFi tokens, NFTs, and traditional assets for cross-market correlation analysis.

**Mobile Optimization**: Ensure dashboard accessibility across devices for on-the-go portfolio monitoring.

## Conclusion
The Cryptocurrency Correlation Analysis Dashboard provides comprehensive insights into crypto market relationships, enabling data-driven investment decisions. The advanced statistical calculations and interactive visualizations offer actionable intelligence for building truly diversified crypto portfolios.

---

This project was completed by Dasola Olanrewaju. Feel free to connect with me on [[[LinkedIn](https://www.linkedin.com/in/olanrewaju-dasola-697a70253/)] for any questions or discussions related to this project or cryptocurrency analytics in general.

Happy analyzing, and may your crypto investments be truly diversified! 🚀📈💎
