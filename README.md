# Revenue-Data-and-Building-a-Dashboard

## Overview

This project analyzes historical stock price data and revenue data for companies using Python. The project demonstrates how to collect financial data using the **yfinance library** and web scraping techniques with **Requests** and **BeautifulSoup**.

The analysis focuses on extracting, cleaning, and visualizing stock market data for:

- Tesla (TSLA)
- GameStop (GME)
- Amazon (AMZN)

The project was completed as part of the IBM Data Analyst / Python for Data Science coursework.

---

## Objectives

The main objectives of this project are:

- Extract historical stock data using the `yfinance` Python library.
- Create ticker objects for different companies.
- Retrieve maximum historical stock price data.
- Perform web scraping to collect quarterly revenue data.
- Clean and process financial datasets.
- Visualize stock prices and revenue trends.
- Compare stock performance with company revenue.

---

## Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas** – Data manipulation and analysis
- **yfinance** – Stock market data extraction
- **Requests** – Web page downloading
- **BeautifulSoup** – HTML parsing and web scraping
- **Matplotlib** – Data visualization

---

## Project Workflow

### 1. Stock Data Extraction

Using the `yfinance` library:

```python
import yfinance as yf

tesla = yf.Ticker("TSLA")
tesla_data = tesla.history(period="max")
