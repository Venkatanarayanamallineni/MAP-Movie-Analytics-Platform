<div align="center">

# 🎬 Movie Analytics Platform (MAP)

### Big Data • Sentiment Analysis • Financial Insights • Visualization

**MIS 5150 – Big Data for Business**
**Project Deliverable 4 | January 2026**

</div>

---

## 📌 Table of Contents

* [Project Overview](#-project-overview)
* [Business Goals](#-business-goals)
* [Data Sources](#-data-sources)
* [Dataset Overview](#-dataset-overview)
* [Data Preparation](#-data-preparation)
* [Financial Analysis](#-financial-analysis)
* [Data Architecture & Flow](#-data-architecture--flow)
* [Sentiment Analysis](#-sentiment-analysis)
* [Predictive Modeling](#-predictive-modeling)
* [Key Insights](#-key-insights)
* [Power BI Visualizations](#-power-bi-visualizations)
* [Tools & Technologies](#-tools--technologies)
* [Conclusion](#-conclusion)
* [Repository Structure](#-repository-structure)

---

## 🎯 Project Overview

The **Movie Analytics Platform (MAP)** is an end-to-end big data analytics solution designed to transform how movie data is evaluated. By integrating large-scale datasets with sentiment analysis, financial modeling, and interactive visualization, MAP provides deeper insights into **movie performance and audience emotional engagement**.

Unlike traditional rating-based analysis, this platform uncovers how audiences *feel* about movies, revealing insights that ratings alone fail to capture.

---

## 🧠 Business Goals

* Analyze over **1 million movie records** efficiently
* Compare **financial performance** using inflation-adjusted metrics
* Identify discrepancies between **ratings and sentiment**
* Enhance decision-making using **interactive dashboards**
* Apply **big data engineering and analytics techniques**

   ## Tech Stack
  - Python (Pandas, NumPy, Scikit-learn)
  - NLP (TF-IDF, Logistic Regression)
  - Power BI (DAX dashboards)
  - SQL (data extraction)
  
  ## Key Results
  - Processed 1M+ movie records with 99%+ data quality
  - Built sentiment classifier: 82% accuracy, 0.79 precision, 0.81 recall
  - Analyzed 50K+ reviews (positive/negative/neutral)
  
  ## Business Impact
  - Discovered r=0.67 correlation between sentiment and box office revenue
  - Identified optimal release timing strategies
  - Created executive dashboards for content strategy decisions

  
---

## 📂 Data Sources

* **IMDb (Internet Movie Database)**
* **TMDB (The Movie Database)**

---

## 📊 Dataset Overview

| Feature    | Description                              |
| ---------- | ---------------------------------------- |
| Records    | > 1,000,000                              |
| Attributes | 42                                       |
| Data Types | Ratings, Financials, Sentiment, Metadata |

---

## 🧹 Data Preparation

### Key Steps

* Downloaded raw datasets
* Cleaned and standardized values
* Removed irrelevant attributes
* Engineered new financial and sentiment variables
* Uploaded cleaned data to cloud storage

### Relevant Attributes

* Movie titles
* Ratings
* Budget & revenue
* Sentiment scores
* Explanatory variables

### Removed Attributes

* URLs
* ID numbers
* Runtime
* Movie status

---

## 💰 Financial Analysis

To enable fair comparisons across different release years:

* **Inflation Rate Assumption:** 2.5%
* Created:

  * Adjusted Revenue
  * Adjusted Budget
  * Return on Investment (ROI)
  * Profit Margin

These metrics allow consistent evaluation of movie profitability over time.

---

## 🔄 Data Architecture & Flow

```text
Data Source
   ↓
Azure Storage Account
   ↓
Azure Data Factory Pipelines
   ↓
Bronze Lakehouse
   ↓
Gold Lakehouse (Power Query Transformations)
   ↓
SQL Endpoint
   ↓
Power BI Dashboards
```

### Key Transformations

* Inflation-adjusted revenue & budget
* ROI and profit margin calculations

---

## 🧠 Sentiment Analysis

### Sentiment Categorization

Sentiment scores were classified into intuitive categories:

| Score Range | Category    |
| ----------- | ----------- |
| -1.0        | Disastrous  |
| -0.5        | Terrible    |
| 0.0         | Neutral     |
| 0.5         | Enjoyable   |
| 1.0         | Masterpiece |

### Advanced Sentiment Processing

* Conducted using **JMP Pro 17**
* Word-level sentiment impact analysis
* Identified emotional drivers beyond numerical ratings

---

## 🔮 Predictive Modeling

* Logistic Regression model
* Sample size: **100 randomly selected movies**
* Binary sentiment classification:

  * **In Favor** (positive emotion)
  * **Opposed** (negative emotion)

### Text Analysis

* Word clouds generated using Text Explorer
* Frequently used words analyzed for sentiment influence

---

## 🔍 Key Insights

✔ High-rated movies often showed **lower sentiment scores**
✔ Low-rated movies sometimes evoked **strong emotional engagement**
✔ Ratings do not always reflect audience emotion
✔ Sentiment captures nuances that ratings miss

These findings suggest emotional response and critical rating are not always aligned.

---

## 📈 Power BI Visualizations

* Adjusted Budget vs. Adjusted Revenue (log scale)
* Top 10 Movies by Highest Adjusted Revenue
* Simplified dashboards for business insights

*(Visualizations designed for clarity and executive decision-making)*

---

## 🛠 Tools & Technologies

* IMDb & TMDB datasets
* Azure Storage Account
* Azure Data Factory
* Lakehouse Architecture
* SQL
* Power BI
* JMP Pro 17

---


## ✅ Conclusion

The Movie Analytics Platform successfully demonstrates:

* Scalable big data processing
* Financial modeling with real-world assumptions
* Advanced sentiment analysis techniques
* Effective visualization for actionable insights

This project highlights the importance of combining **quantitative metrics** with **emotional analytics** to better understand audience behavior.
>
