# Financial Data Extraction and Analysis (Estimize.com)

This project demonstrates the complete pipeline of extracting structured financial data from [Estimize.com](https://www.estimize.com), storing it into a MySQL database, and querying it for analyst insights, earnings estimates, and industry-level metrics. Regression analysis is also performed to predict EPS values based on extracted features.

---

## Project Overview

### Problem Statement
- Extract EPS data, company info, and analyst insights for 29 tickers over 3 years (2020–2022).
- Clean, structure, and store scraped data into a MySQL database.
- Perform exploratory queries to answer investment-related business questions.
- Build a regression model to predict EPS outcomes.

---

##  Contents
```code
Financial-Data-Extraction-and-Analysis/
├── sql queries.sql         # All analytical SQL queries
├── webscraping.ipynb       # Selenium-based data extraction scripts
├── Regression.ipynb        # Linear regression model and results
└── README.md               # This file
```

---

## Tools Used

- **Scraping:** Python, Selenium, BeautifulSoup
- **Storage:** MySQL, SQLAlchemy
- **Analysis:** Jupyter Notebooks (Pandas, scikit-learn)
- **Reporting:** PDF + PowerPoint

---

## Data Source

- Website: [https://www.estimize.com](https://www.estimize.com)
- Data extracted includes:
  - EPS estimates (Wall Street, Estimize, Reported)
  - Company metadata (sector, industry, followers)
  - Analyst profiles (confidence score, accuracy, roles)

> *Note: Authentication is required for scraping (user login used with Selenium).*

---

##  Key Business Queries Answered

- Top analysts per stock by confidence and accuracy
- Analyst count per ticker and industry
- Most followed companies
- Bias between reported vs. estimated earnings
- Industry-wide analyst average estimates

---

##  Regression Model

- Performed linear regression to predict EPS
- Achieved ~79.7% accuracy
- Key predictors: Ticker, Company metadata, Estimize estimates


