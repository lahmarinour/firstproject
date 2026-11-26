# StockTwits Sentiment Analysis & Market Performance

## Overview
This project explores the relationship between social-media sentiment expressed on StockTwits and stock-market performance. StockTwits messages are collected, cleaned, analyzed with two sentiment-analysis approaches, and compared with historical stock prices.

The project uses **VADER** as a lexicon-based baseline and **FinBERT**, a transformer model trained for financial text, to compare sentiment predictions.

## Objectives
- Collect StockTwits messages for a selection of stock tickers.
- Clean and prepare text data for sentiment analysis.
- Analyze messages using VADER and FinBERT.
- Aggregate sentiment scores by ticker and date.
- Compare sentiment indicators with stock-price movements.
- Explore the differences between the two sentiment models.

## Workflow
1. **Data collection:** retrieve StockTwits messages for selected tickers.
2. **Data cleaning:** handle missing text, duplicates, and prepare text for analysis.
3. **VADER analysis:** calculate positive, negative, neutral, and compound sentiment scores.
4. **FinBERT analysis:** estimate positive, negative, and neutral probabilities; calculate a sentiment score as positive probability minus negative probability.
5. **Aggregation:** summarize sentiment by ticker and, where applicable, by date.
6. **Market comparison:** retrieve price data with `yfinance` and compare sentiment with price changes.
7. **Visualization:** plot model results and market-performance comparisons.

## Sentiment models
- **VADER:** a rule- and lexicon-based model used as a baseline.
- **FinBERT:** a transformer-based model designed for financial-language sentiment classification.

The two approaches are compared rather than assuming one is automatically better.

## Technologies
- Python
- pandas
- matplotlib
- seaborn
- yfinance
- NLTK / VADER
- Transformers
- PyTorch
- Jupyter Notebook

## Project files
Notebook names and data files may evolve as the project is improved. The notebooks follow the analysis workflow from collection and cleaning to sentiment analysis, aggregation, and visualization.

## Limitations
- Social-media messages may be noisy, informal, sarcastic, or ambiguous.
- The available sample and time period may be limited.
- Stock-price changes can be affected by many factors unrelated to social-media sentiment.
- A correlation does not demonstrate causation or predictive ability.
- FinBERT and VADER scores are not directly equivalent because they use different scoring methods.

## Disclaimer
This project is for educational and exploratory purposes only. It is not financial advice and should not be used as the sole basis for investment decisions.