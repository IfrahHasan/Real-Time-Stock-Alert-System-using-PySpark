# Real-Time Stock Data Pipeline with PySpark

**Overview**  
This project showcases a real-time data streaming pipeline that captures, processes, and analyzes stock market data in near-real-time. By leveraging PySpark’s distributed processing capabilities and integrating a Telegram Bot for instant alerts, this pipeline demonstrates how to efficiently handle financial time-series data at scale.

**Features**  
- **Continuous Data Streaming:** Fetches minute-level stock data from Yahoo Finance for multiple tickers (e.g., AAPL, MSFT, GOOG).  
- **Advanced Analytics:** Computes price spikes, volume surges, volatility shifts, and moving average crossovers.  
- **Anomaly Detection:** Automatically identifies significant market changes and logs them for further analysis.  
- **Instant Alerts via Telegram:** Sends critical alerts directly to a Telegram channel, providing stakeholders with timely market insights.  
- **Daily Summary Reports:** Generates end-of-day reports to review key metrics and anomalies, delivered as a concise PDF.  
- **Scalable and Extensible:** Built on PySpark to handle large datasets, with a modular design to easily integrate additional analytics or data sources.

**Integration with Telegram**  
Using the Telegram Bot API, the pipeline sends alerts directly to a specified Telegram channel. This ensures that analysts, traders, and other stakeholders are promptly informed of important market events. The bot is configured to send messages whenever predefined conditions are met, and the process can be easily customized by adjusting alert thresholds or adding new analytics.

**Project Structure**  

Project Structure:

- real-time-stock-pipeline/
  - README.md: Project overview and setup instructions
  - requirements.txt: Dependencies for running the project
  - LICENSE: Open source license
  - notebooks/: Colab notebook or Jupyter notebooks
    - main_pipeline.ipynb: The primary data pipeline notebook
  - data/: Data and logs
    - logs/: Anomaly logs
    - historical/: Historical data files
  - reports/: Output reports
    - daily_report.pdf: Example end-of-day report



**Getting Started**  
1. **Install Dependencies:**  
   - Ensure you have Python 3.8 or later.  
   - Install the required packages from `requirements.txt`:
     ```bash
     pip install -r requirements.txt
     ```

2. **Configure Telegram Bot:**  
   - Create a Telegram bot using [BotFather](https://core.telegram.org/bots#botfather) and obtain your bot token.  
   - Set up a Telegram channel or chat where the bot will send alerts, and add the bot as a member.  
   - Update the pipeline code with your bot token and channel ID.

3. **Run the Pipeline:**  
   - Open the provided Colab notebook or run the main script locally.  
   - Start streaming data and let the pipeline process incoming stock market data.  
   - Alerts will automatically appear in your Telegram channel when significant conditions are met.

**Contributing**  
Contributions are welcome! If you have ideas for improving the analytics, adding new data sources, or enhancing the Telegram integration, please submit a pull request or open an issue. 

**License**  
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

