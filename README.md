# Strategic Product Placement Analysis

A Tableau dashboard project investigating how **product positioning** (front-of-store, aisle, end-cap), **promotions**, and **consumer demographics** influence sales performance and shopper behavior in a retail environment.

![Tableau](https://img.shields.io/badge/Tableau-Public-E97627?logo=tableau&logoColor=white)
![Status](https://img.shields.io/badge/status-complete-brightgreen)

---

## 📌 Project Overview

Retailers constantly face the question: *where and how should a product be placed to sell the most?* This project analyzes sales, placement, promotion, and demographic data to answer exactly that — and to translate the findings into concrete merchandising recommendations.

**Business problem:** A retail company wants to understand the impact of product positioning on sales and consumer behavior. They have data on sales figures, product placement, and consumer demographics, and want to know which positioning strategies drive the most sales — and how to tailor marketing efforts accordingly.

**Goal:** Use Tableau to visualize the data and deliver actionable insights that optimize product positioning and drive revenue growth.

---

## 🎯 Objectives

- Quantify the effect of **product position** (Front of Store, Aisle, End-cap) on average sales volume, by category
- Measure how **promotions** move price and sales volume differently across categories
- Compare **internal pricing vs. competitor pricing** by category
- Understand which **consumer demographic segments** drive the most volume
- Explore the relationship between **foot traffic levels** and sales volume by position
- Convert all of the above into positioning and marketing recommendations

---

## 🗂️ Dataset

The dataset combines sales transactions with placement and shopper attributes:

| Field | Description |
|---|---|
| Product Category | Clothing / Electronics / Food |
| Product Position | Front of Store / Aisle / End-cap |
| Promotion (Seasonal) | Yes / No |
| Price / Competitor Price | Unit price vs. nearest competitor |
| Avg. Sales Volume | Average units sold |
| Foot Traffic | Low / Medium / High |
| Consumer Demographic | Young Adults / College Students / Families / Seniors |

---

## 🛠️ Tools & Skills

- **Tableau (Desktop / Public)** — data visualization & dashboard design
- **Dashboard actions & filters** — Seasonal (promotion), Product Category, Consumer Demographics, Avg. Price
- Chart types used: grouped bar charts, pie/donut charts, packed-bubble charts, cross-tab heat tiles

---

## 📊 Dashboard Views

The dashboard (`Dashboard 1`) combines six worksheets into a single interactive view:

1. **Promotion of Product Category on Price and Sales Volume** — cross-tab comparing avg. price and avg. sales volume with promotion **On vs Off**, per category
2. **Avg Sales Volume by Product Category by Season** — bar chart of seasonal effect per category
3. **Product Category vs Price** — pie chart of average price share by category
4. **Competitor Price vs Price** — grouped bars comparing internal price to competitor price per category
5. **Avg Sales Volume by Product Category by Product Position** — heat-tile matrix of category × position (Front of Store / Aisle / End-cap)
6. **Average Sales Volume by Product Category** — horizontal bar ranking of categories by volume
7. **Consumer Demographics vs Sales Volume** — donut chart of total volume (17,69,311 units) split across Young Adults, College Students, Families, Seniors
8. **Foot Traffic by Avg Sales Volume** — packed-bubble chart sizing sales volume by foot-traffic level and position

All views are cross-filtered by global **Seasonal**, **Product Category**, **Avg. Price**, and **Consumer Demographics** filters.

---

## 🔑 Key Insights

- **Promotions don't move every category the same way.** Clothing's average sales volume actually *drops* when promoted (1,869 → 1,781), while Electronics (1,726 → 1,773) and Food (1,677 → 1,782) both *gain* volume under promotion — suggesting promotion budgets are better spent on Electronics and Food than Clothing.
- **Position beats category** for Clothing: Front-of-Store placement (≈1,924 units) clearly outperforms Aisle placement (≈1,833 units) for Clothing — a ~5% lift from position alone.
- **Clothing leads overall average sales volume** (1,830 units), ahead of Electronics (1,749) and Food (1,728), even though Food carries the highest average price (28.47 vs ~27.8 for the others).
- **Pricing is competitive, not aggressive** — internal price tracks closely with competitor price across all three categories, implying volume differences come from placement and promotion rather than price undercutting.
- **College Students are the single largest demographic segment** by sales volume (4,50,063 units of 17,69,311 total), narrowly ahead of Seniors (4,44,089) and Families (4,43,276), with Young Adults trailing (4,31,883).
- **High foot-traffic zones consistently carry the largest sales-volume bubbles**, confirming that traffic exposure — not just shelf category — is a strong secondary driver of volume, with End-cap and Aisle spots showing the widest spread between Low and High traffic outcomes.

---

## ✅ Recommendations

1. **Reserve Front-of-Store placement for Clothing** — this is the category proven to benefit most from prime positioning.
2. **Redirect promotional spend toward Electronics and Food**, where promotions reliably increase sales volume; reconsider blanket promotions on Clothing.
3. **Target College Students and Seniors** in marketing campaigns, as they generate the highest sales volumes.
4. **Prioritize high-foot-traffic zones** (End-cap and Aisle) for categories that are under-indexed on volume, to capture more impulse-driven purchases.
5. **Maintain price parity** with competitors rather than competing on price — the data shows placement and promotion are the real levers, not discounting.

---

## 📁 Repository Structure

```
├── Strategic_Product_Placement_Analysis.twbx   # Packaged Tableau workbook
├── data/                                       # Source data (sales, placement, demographics)
├── README.md                                   # Project documentation (this file)
└── presentation/                               # Summary slide deck
```

---

## 🚀 How to View

1. Download [Tableau Public/Desktop](https://www.tableau.com/products/public) (free)
2. Open `Strategic_Product_Placement_Analysis.twbx`
3. Use the **Seasonal**, **Product Category**, and **Consumer Demographics** filters on the right panel to explore the data interactively

---

## 👤 Author

Prepared as part of a data analytics/BI portfolio project focused on retail sales and product positioning analysis.
