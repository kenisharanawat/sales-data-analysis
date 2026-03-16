# Sales Data Analysis – Superstore Dataset

A data analysis project exploring sales trends, regional performance, and customer behaviour using the Superstore retail dataset (9,800 orders across the US, 2015–2018).

Done as part of my self-learning in data science — this was my first end-to-end EDA project where I worked with a real-world messy dataset and tried to answer actual business questions rather than just plotting things randomly.

---

## What I was trying to find out

- Which regions and states drive the most revenue?
- Does Q4 really spike sales, or is that a myth for this dataset?
- Which product categories and sub-categories are most valuable?
- Are there differences in how Consumer, Corporate, and Home Office customers buy?
- How long does shipping actually take across different shipping modes?

---

## Dataset

**Source:** [Superstore Sales Dataset – Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)  
**File:** `data/train.csv`  
**Size:** 9,800 rows × 18 columns  
**Period:** January 2015 – December 2018

Columns used: `Order Date`, `Ship Date`, `Ship Mode`, `Segment`, `Region`, `State`, `Category`, `Sub-Category`, `Product Name`, `Sales`

---

## Project structure

```
sales-analysis/
│
├── data/
│   └── train.csv
│
├── notebooks/
│   └── sales_analysis.ipynb
│
├── outputs/
│   └── (charts saved here)
│
├── requirements.txt
└── README.md
```

---

## Key findings

1. **California and New York together account for ~33% of total revenue** — the top 3 states (CA, NY, TX) alone represent nearly half of all sales.

2. **Q4 consistently drives ~38–39% of annual revenue** across all four years, confirming strong end-of-year seasonality.

3. **Technology is the highest-revenue category** ($827K total), but Furniture and Office Supplies are close behind — no single category dominates overwhelmingly.

4. **Phones and Chairs are the top two sub-categories** by revenue (~$327K and ~$322K respectively), both significantly ahead of the rest.

5. **Consumer segment contributes 46% of revenue**, more than Corporate (28%) and Home Office (17%) combined.

6. **Revenue grew 57% from 2015 to 2018** ($479K → $722K), with the biggest jump happening between 2016 and 2017.

7. **Standard Class is the most used shipping mode** (60% of orders) but averages 5 days. Same Day is rarely used (5.5% of orders).

---

## How to run

```bash
git clone https://github.com/kenisha-ranawat/sales-analysis
cd sales-analysis
pip install -r requirements.txt
jupyter notebook notebooks/sales_analysis.ipynb
```

---

## Requirements

```
pandas
matplotlib
seaborn
jupyter
```

---

## What I'd do next

- Add a profit column analysis (this dataset only has sales, not profit)
- Try forecasting 2019 sales using a simple linear regression
- Look at customer-level repeat purchase behaviour

---

*This is a learning project. Feedback welcome.*
