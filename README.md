# 📊 RFM Customer Segmentation Analysis with Python

## 🎯 Project Overview

This project applies **RFM (Recency, Frequency, Monetary)** analysis to an e-commerce dataset to segment customers and provide strategic marketing recommendations. 

The project reflects practical skills in **data cleaning, RFM scoring, segmentation logic, and business interpretation**—commonly used in customer analytics and CRM applications.

---

## 📁 Dataset

- **Source**: Ecommerce Retail CSV

---

## 📐 Methodology

### 🔹 Step 1: Data Preview & Cleaning
- Loaded data with `pandas`
- Cleaned missing or invalid entries
- Formatted columns for analysis

### 🔹 Step 2: Feature Engineering
- Created `TotalRevenue` column
- Converted `InvoiceDate` to datetime
- Prepared relevant columns for RFM analysis

### 🔹 Step 3: RFM Scoring
- Calculated:
  - **Recency** = Days since last purchase
  - **Frequency** = Number of transactions
  - **Monetary** = Total revenue
- Assigned quantile-based RFM scores (1–5)
- Created a composite `RFMScore` (e.g., 555)

### 🔹 Step 4: Segmentation & Visualization
- Mapped RFM scores to labeled customer segments
- Visualized distribution of R, F, M scores
- Created **treemap** of customer segments using `squarify`

---

## 📊 Key Customer Segments & Recommendations

| Segment | Description | Action |
|---------|-------------|--------|
| 🏆 Champions | Recent, frequent, and high-spending | Reward, upsell, exclusive offers |
| 🔄 Potential Loyalists | Moderate scores in all 3 | Convert to champions with incentives |
| 💤 Hibernating | Old, inactive, low-spending | Reactivate with re-engagement campaigns |
| 🆕 New Customers | New, low frequency | Nurture and guide onboarding |
| ⚠️ At Risk | High-value but disengaging | Prevent churn with personalized offers |

> Full strategy table included in notebook.

---

## 📈 Visualizations

- Histogram plots of Recency, Frequency, Monetary distribution
- Treemap of customer segments by percentage share
- Clean layout using `matplotlib`, `seaborn`, and `squarify`

---

## 🛠️ Tools & Libraries

- Python 3
- Google Colab
- `pandas`, `numpy`, `seaborn`, `matplotlib`, `squarify`
- Excel integration via `pandas.read_excel`

---

## 🚀 How to Run

1. Open the notebook in [Google Colab](https://colab.research.google.com/)
2. Upload the `ecommerce-retail.csv` in the zip file 
3. Run all code cells in sequence
