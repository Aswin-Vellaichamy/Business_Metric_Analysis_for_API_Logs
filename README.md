# Business_Metric_Analysis_for_API_Logs

Python-based performance analysis dashboard using provided app logs data. The goal is to extract meaningful insights and create visualizations that could help monitor app health.

**Business Metrics Analysis**

This repository contains a Python script for analyzing API log data to compute key business metrics and visualize patterns. The analysis includes insights such as response time trends, error rates, peak usage periods, and endpoint performance. Below are the detailed steps, functionalities, and instructions for setting up and running the code.

# Features

**Response Time Metrics**

- Calculates average and P95 (95th percentile) response times for each endpoint.

- Detects unusual spikes in response times using a boxplot method.

**Error Metrics**

 - Computes error rates and categorizes errors (Client Errors vs. Server Errors).

- Detects hourly error rate anomalies.

**Usage Metrics**

- Identifies peak usage periods by hour.

- Analyzes endpoint availability and identifies issues.

- User Experience Metrics

- Calculates the percentage of requests taking more than 1 second.

**Visualizations**

- Bar charts for response times, error rates, and requests per endpoint.

- Line plots for response time trends and error rate patterns.

- Scatter plots and boxplots for response time anomalies.

**Requirements**

- Python 3.7 or higher

**Required Python libraries**:

- pandas

- matplotlib

- You can install the required libraries using pip:

```
pip install pandas matplotlib
```

**Input Data**

The script expects a CSV file with the following columns:

- endpoint: The API endpoint hit.

- response_time: The response time in seconds.

- status_code: The HTTP status code returned.

- timestamp: The timestamp of the request (in ISO 8601 format).

**How to Run**

- Place your log data in a CSV file, e.g., app_logs.csv.

- Update the file path in the script:
```
file_path = '/path/to/your/app_logs.csv'
```

**Run the script**:
```
python script.py
```
The results will be printed to the console and saved as CSV files in the output directory.

**Visualizations**

- response_times_plot.png: Bar chart of average and P95 response times.

- error_rates_plot.png: Bar chart of error rates by type.

- peak_usage_plot.png: Line chart of peak usage periods.

- requests_per_endpoint_plot.png: Bar chart of total requests per endpoint.

- response_time_trends_plot.png: Line chart of response time trends over time.

- error_rate_patterns_plot.png: Line chart of error rate patterns over time.

- endpoint_performance_plot.png: Line chart comparing endpoint performance.

- peak_usage_analysis_plot.png: Bar chart of hourly usage.

- response_time_boxplot.png: Boxplot of response times.

- response_time_spikes_scatter.png: Scatter plot of unusual spikes in response times.

