# CS-GY-6513: Big Data Project - Analysis and Prediction of Stock Prices Using Yahoo Finance Dataset


## Abstract
Stock price prediction is crucial for financial analysis, helping investors and institutions make informed decisions. The vast and constantly evolving nature of stock market data makes prediction challenging. Stock prices change rapidly, generating massive amounts of real-time data, while historical records spanning years or decades contribute millions of data points per stock.

Traditional forecasting methods struggle with the market's complexity and volatility. They are computationally slow, inefficient with large datasets, and often fail to capture the non-linear patterns that drive stock price movements. With data covering thousands of stocks over long periods, traditional approaches also face scalability issues and miss critical indicators, reducing accuracy and increasing prediction errors.

This project aims to develop a machine learning-based predictive model for stock price forecasting, leveraging historical stock data from Yahoo Finance. By utilizing advanced data analytics and machine learning techniques, the project seeks to improve stock price prediction’s accuracy and provide investors with valuable insights.

---

## Setup Instructions

### Prerequisites
1. **Python Environment**:
   - Use version 3.12.9
   - Create a virtual environment:  
     ```bash
     python -m venv venv
     source venv/bin/activate  # On Windows: venv\\Scripts\\activate
     ```
   - Install dependencies:  
     ```bash
     pip install -r requirements.txt
     ``` 
2. **Java Installation**:
   - Install Java 8 (required for Apache Spark).

3. **Apache Spark**:
   - Install Apache Spark 3.5.5. Ensure it's added to your system PATH.
4. **Update JAVA_HOME and SPARK_HOME**: 
   - Update paths in every notebook to prevent dependency conflicts 
---

## Running the Project

### Step 1: Data Preprocessing
Run the preprocessing pipeline available in the notebook:
- **File**: `BigDataPreProcessing&DataUnpacking.ipynb`
- **Output**: Preprocessed datasets for analysis and model training.

### Step 2: Exploratory Data Analysis (EDA)
Conduct EDA and visualize patterns in the data:
- **File**: `BigDataProjectDataVisualisations&EDA.ipynb`
- **Output**: Key insights and visualizations of historical trends.

### Step 3: Anomaly Detection
Identify anomalies in stock price data:
- **File**: `BigDataAnomalyDetection.ipynb`
- **Output**: Anomalies in stock prices and trading volumes using ZScores.

### Step 4: Machine Learning Model Experiments
Build and evaluate machine learning models for stock price prediction:
- **File**: `BigDataMLPredictionModelExperiments.ipynb`
- **Output**: Prediction models like LSTM, Random Forests and performance metrics (e.g., RMSE, R-squared).

---

## Future Work
- Implement real-time recommendation updates using streaming data pipelines.
- Develop a web-based user interface for system interaction.
- Create user-specific dashboards for personalized recommendations and history visualization.
- Incorporate sentiment analysis of user reviews to enhance recommendation accuracy.

---

## Acknowledgments
This project leverages stock market data from FNSPID
@misc{dong2024fnspid,
      title={FNSPID: A Comprehensive Financial News Dataset in Time Series}, 
      author={Zihan Dong and Xinyu Fan and Zhiyuan Peng},
      year={2024},
      eprint={2402.06698},
      archivePrefix={arXiv},
      primaryClass={q-fin.ST}
}
