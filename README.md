# Marketing Analytics Case Study

## Project Overview

This project presents an end-to-end marketing analytics solution for **ShopEasy**, an online retail company experiencing declining customer engagement and conversion rates despite increasing marketing investments.

The objective was to analyze customer interactions, engagement metrics, and customer feedback to uncover actionable business insights and recommend strategies for improving marketing performance. The business case focused on improving conversion rates, increasing customer engagement, and understanding customer sentiment from product reviews. :contentReference[oaicite:0]{index=0}

---

## Business Objectives

- Improve website conversion rates
- Analyze customer engagement across marketing channels
- Perform sentiment analysis on customer reviews
- Build an interactive dashboard for decision making

---

## Tech Stack

- SQL Server
- SQL
- Python
- Pandas
- NLTK (VADER Sentiment Analysis)
- Power BI

---

## Project Workflow

### 1. Data Cleaning using SQL

The raw marketing datasets were cleaned using SQL.

Cleaning included:

- Removing duplicate records
- Standardizing text fields
- Handling NULL values
- Formatting customer review text
- Preparing dimensional and fact tables for analysis

SQL files:

- dim_customers.sql
- dim_products.sql
- fact_customer_journey.sql
- fact_customer_review.sql
- fact_engagement_data.sql

---

### 2. Customer Sentiment Analysis using Python

Customer reviews were extracted from SQL Server using **pyodbc** and analyzed using the **VADER Sentiment Analyzer** from NLTK.

The script:

- connects to SQL Server
- loads customer reviews
- computes sentiment scores
- classifies reviews into sentiment categories
- creates sentiment buckets
- exports an enriched CSV for visualization

Python libraries:

- pandas
- nltk
- pyodbc

Output:

```
fact_customer_review_with_sentiment.csv
```

---

### 3. Interactive Dashboard in Power BI

The cleaned SQL data and enriched customer review dataset were imported into Power BI to build an executive dashboard.

Dashboard includes:

- Conversion Rate
- Customer Engagement Trends
- Monthly Views
- Click-through Analysis
- Customer Rating Distribution
- Sentiment Analysis
- Product Performance

---

## Key Insights

### Conversion Rate

- Conversion rates fluctuated significantly throughout the year.
- January achieved the highest conversion rate, while May recorded the lowest.
- Seasonal product categories such as Ski Boots and Kayaks showed particularly strong performance. :contentReference[oaicite:1]{index=1}

### Customer Engagement

- Website views declined during the second half of the year.
- Blog content consistently generated the highest engagement.
- Click-through rates remained healthy despite declining overall traffic. :contentReference[oaicite:2]{index=2}

### Customer Feedback

- Most reviews were rated 4 or 5 stars.
- Positive sentiment dominated customer feedback.
- Mixed and negative reviews highlighted opportunities for product and service improvements. :contentReference[oaicite:3]{index=3}

---

## Business Recommendations

- Focus marketing efforts on high-converting product categories.
- Improve engagement through richer and more interactive content.
- Address recurring customer complaints identified through sentiment analysis to improve satisfaction and increase conversions. :contentReference[oaicite:4]{index=4}

---

## Repository Structure

```
marketing-analytics-case-study
│
├── sql/
├── python/
├── powerbi/
├── data/
├── csv/
├── images/
└── README.md
```

---

## Skills Demonstrated

- SQL Data Cleaning
- Data Transformation
- Natural Language Processing (NLP)
- Sentiment Analysis
- Data Visualization
- Power BI Dashboard Development
- Business Analytics
- Marketing Analytics


---

## Author

**Anandini Kashyap**
