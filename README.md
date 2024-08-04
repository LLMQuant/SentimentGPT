
<div align="center">
<img align="center" width="30%" alt="image" src="[[https://chatgpt.com/api/content/file-FL7lS65iQnrqPG5BwWYIITh3]](https://github.com/LLMQuant/SentimentGPT/blob/main/sentimentGPT.png)">
</div>

# SentimentGPT: Enhancing Trading with Sentiment Analysis using Large Language Models
[![Downloads](https://static.pepy.tech/badge/sentimentgpt)]([https://pepy.tech/project/sentimentgpt](https://pepy.tech/project/sentimentgpt))
[![Downloads](https://static.pepy.tech/badge/sentimentgpt/week)](https://pepy.tech/project/sentimentgpt)
[![Python 3.8](https://img.shields.io/badge/python-3.6-blue.svg)](https://www.python.org/downloads/release/python-360/)
[![PyPI](https://img.shields.io/pypi/v/sentimentgpt.svg)](https://pypi.org/project/sentimentgpt/)
![License](https://img.shields.io/github/license/LLMQuant/sentimentgpt.svg?color=brightgreen)
![](https://img.shields.io/github/issues-raw/LLMQuant/sentimentgpt?label=Issues)
![](https://img.shields.io/github/issues-closed-raw/LLMQuant/sentimentgpt?label=Closed+Issues)
![](https://img.shields.io/github/issues-pr-raw/LLMQuant/sentimentgpt?label=Open+PRs)
![](https://img.shields.io/github/issues-pr-closed-raw/LLMQuant/sentimentgpt?label=Closed+PRs)

<div align="center">
<img align="center" src="figs/logo_white_background.jpg" width="40%"/>
</div>
**SentimentGPT** is a cutting-edge platform designed to leverage sentiment analysis in trading. Sentiment analysis involves analyzing and interpreting emotions, opinions, and attitudes expressed in text data. Market sentiment refers to market participants' overall attitude and emotions towards a particular financial instrument or market, which can influence buying and selling decisions.

## Table of Contents
- [SentimentGPT Overview](#sentimentgpt-overview)
- [Components](#components)
  - [Data Collection](#data-collection)
  - [Data Preprocessing](#data-preprocessing)
  - [Sentiment Analysis](#sentiment-analysis)
  - [Trading Strategy Integration](#trading-strategy-integration)
- [Installation](#installation)
- [Usage](#usage)
  - [Data Collection](#data-collection-usage)
  - [Data Preprocessing](#data-preprocessing-usage)
  - [Sentiment Analysis](#sentiment-analysis-usage)
  - [Trading Strategy Integration](#trading-strategy-integration-usage)
- [File Structure](#file-structure)
- [License](#license)

## SentimentGPT Overview

SentimentGPT utilizes natural language processing and machine learning techniques to determine the sentiment behind text data, whether positive, negative, or neutral. It provides valuable insights into how traders and investors feel about certain assets, which can influence their decision-making process.

## Components

### Data Collection

Collect relevant text data from various sources, such as news articles, social media, and financial reports, to understand market sentiment.

### Data Preprocessing

Prepare the collected data for analysis by cleaning, tokenizing, and transforming it into a suitable format for sentiment analysis.

### Sentiment Analysis

Apply natural language processing and machine learning techniques to determine the sentiment behind the preprocessed text data.

### Trading Strategy Integration

Integrate the sentiment analysis results into trading strategies to gauge market sentiment, identify trends, and make informed trading decisions.

## Installation

**1. (Recommended) Create a new virtual environment**
```shell
conda create --name sentimentgpt python=3.10
conda activate sentimentgpt
```

**2. Download the SentimentGPT repository**
```shell
git clone https://github.com/YourUsername/SentimentGPT.git
cd SentimentGPT
```

**3. Install SentimentGPT & dependencies from source or PyPI**
```bash
pip install -U sentimentgpt
```
or
```bash
pip install -e .
```

**4. Configure API keys**
```shell
1. Rename `OAI_CONFIG_LIST_sample` to `OAI_CONFIG_LIST` and add your OpenAI API key.
2. Rename `config_api_keys_sample` to `config_api_keys` and add your financial data API keys.
```

## Usage

### Data Collection Usage
To collect relevant text data:
```python
from sentimentgpt.data_collection import DataCollector

collector = DataCollector(config)
data = collector.collect()
```

### Data Preprocessing Usage
To preprocess the collected data:
```python
from sentimentgpt.data_preprocessing import DataPreprocessor

preprocessor = DataPreprocessor(config)
processed_data = preprocessor.preprocess(data)
```

### Sentiment Analysis Usage
To perform sentiment analysis:
```python
from sentimentgpt.sentiment_analysis import SentimentAnalyzer

analyzer = SentimentAnalyzer(config)
sentiment = analyzer.analyze(processed_data)
```

### Trading Strategy Integration Usage
To integrate sentiment analysis into trading strategies:
```python
from sentimentgpt.trading_strategy import StrategyIntegrator

integrator = StrategyIntegrator(config)
integrated_strategy = integrator.integrate(sentiment)
```

## File Structure

The main folder **sentimentgpt** has four subfolders **data_collection, data_preprocessing, sentiment_analysis, trading_strategy**. 

```
SentimentGPT
├── sentimentgpt (main folder)
│   ├── data_collection
│   	├── data_collector.py
│   ├── data_preprocessing
│   	├── data_preprocessor.py
│   ├── sentiment_analysis
│   	├── sentiment_analyzer.py
│   ├── trading_strategy
│   	├── strategy_integrator.py
│   ├── utils.py
│
├── configs
├── experiments
├── tutorials (hands-on tutorial)
│   ├── data_collection_tutorial.ipynb
│   ├── data_preprocessing_tutorial.ipynb 
│   └── sentiment_analysis_tutorial.ipynb
├── setup.py
├── config_api_keys_sample
├── requirements.txt
└── README.md
```

## License

This project is licensed under the Apache-2.0 License. See the LICENSE file for more details.

---

**Disclaimer**: The information provided in this repository is for educational purposes only and should not be construed as financial advice. Always consult with a qualified financial advisor before making any investment decisions.
