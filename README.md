# Automated Trends Collection & Interactive Analysis of Greek Shoe Models

Interactive analysis of Google Trends search volume for the Greek athletic
footwear market — **19 brands, 96 shoe models and 22 sock terms**, collected
automatically and placed on one comparable scale.

### 📊 [Open the interactive report →](https://step-sport-search-analysis.netlify.app)

---

## What it does

**Automated collection (Python)** — pulls weekly Google Trends series for 90+
shoe models using a shared anchor term. This is the core problem: Trends
normalises every request to 0–100 *within that request*, so two separate
exports cannot be compared. The anchor makes them comparable.

**Analysis (R)** — seasonality indices, correlation structure between models,
volume-vs-momentum positioning, and rising-query ranking on a common scale.

**Interactive report** — per-chart search and filtering, published as a single
self-contained HTML page.

## About the code

The analysis was built during a data analysis internship, so the source is not
published here. The report is a lightly adapted version of the internal one and
uses public Google Trends data only.

## Practical note

Collection runs noticeably faster in the early morning (06:00–10:00) — Google
Trends throttles requests less at those hours.

---

Python · R (tidyverse, plotly, crosstalk) · Data: Google Trends, subject to Google's Terms of Service
© 2026 Charalampos Sarakatsanis
