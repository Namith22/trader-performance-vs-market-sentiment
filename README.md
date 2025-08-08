Analysis of Trader Performance vs. Market Sentiment
Project Overview
This project conducts a detailed analysis of the relationship between trader performance, using historical data from Hyperliquid, and market sentiment, as measured by the Bitcoin Fear & Greed Index. The primary objective is to uncover actionable patterns in profitability, trading volume, risk, and strategy (long vs. short) under different market conditions. The insights are intended to help drive the development of smarter, data-driven trading strategies.

Directory Structure
The project is organized into the following structure to ensure clarity and reproducibility:
notebook_1.ipynb: The main Google Colab notebook containing all Python code for data loading, cleaning, analysis, and visualization.
csv_files/: Stores all tabular data outputs.
performance_summary.csv: A summary table of key performance metrics by market sentiment.
outputs/: Stores all visual outputs from the analysis.
README.md: This file, providing a complete overview and setup instructions.


How to Run
Environment: This project is designed to be run in a Google Colab environment.
Data: Upload the fear_greed_index.csv and historical_data.csv files to the root directory of your Colab session.
Execution: Open notebook_1.ipynb and run all the cells sequentially. The script will automatically create the csv_files/ and outputs/ directories and save all the analysis files.
Key Findings & Insights
The analysis revealed several significant patterns connecting trader behavior to market sentiment:

High-Level Trends
"Fear" Drives Profit and Volume: The highest total profit and greatest trading volume are generated during periods of "Fear." This suggests that volatile conditions or contrarian strategies (buying when others are fearful) are highly effective for this cohort of traders.
"Extreme Greed" Has the Highest Win Rate: While "Fear" generates the most absolute profit, trades made during "Extreme Greed" have the highest success rate (46.5% of trades are profitable). This indicates that while traders may be more cautious, their individual bets are more consistently successful when the market is euphoric.
Deeper Insights from Advanced Visualizations
PnL Distribution Reveals Risk: The box plot of PnL shows that while "Fear" has the highest total profit, it also comes with a very wide distribution of outcomes, indicating higher risk. In contrast, "Extreme Greed" shows a tighter, more consistent range of profits.
"Fear" Encourages Larger, Bolder Trades: The trade size distribution shows that the median trade size is largest during periods of "Fear", suggesting traders are more confident and willing to commit more capital during these times, likely to capitalize on perceived market bottoms.
Trade Side Strategy is Key: The analysis of BUY vs. SELL trades reveals a crucial pattern: BUY (long) positions are significantly more profitable across all sentiment types, especially during "Fear" and "Greed." SELL (short) positions, on the other hand, consistently contribute much less to overall profitability.
Coin-Specific Performance: The profitability analysis of the top 5 coins shows that performance is not uniform. Certain coins, like BTC and ETH, are major profit drivers, especially during "Fear" and "Greed," while others may perform differently, highlighting the need for asset-specific strategies.
