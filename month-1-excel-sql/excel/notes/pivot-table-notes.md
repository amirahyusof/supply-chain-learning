# Pivot Table Notes

**Resource:** https://www.freecodecamp.org/news/how-to-create-a-pivot-table-in-excel/
**Dataset:** shopee_dataset.csv (40 orders, 14 columns)
**Date started:** 2/6/2026

---

## How to Create a Pivot Table (Steps)

1. Select your data → Insert → PivotTable → New Worksheet
2. Drag fields into ROWS, COLUMNS, VALUES, or FILTERS
3. In VALUES, click dropdown → Value Field Settings to change
   calculation (SUM, COUNT, AVERAGE, MAX, MIN)

---

## Pivot Tables I Built

### PT1 — Sales by Category

- Rows: Category
- Values: Sum of NetSales, Sum of Quantity
- Key finding: [write what you found, e.g. "Electronics had highest NetSales"]

### PT2 — Seller Performance

- Rows: Seller
- Values: Sum of NetSales, Average of Rating, Count of OrderID
- Calculated Field: Avg Order Value = NetSales / Quantity
- Key finding: [e.g. "TopStore had most orders but SellerA had higher avg order value"]

### PT3 — Sales by Region

- Rows: Region
- Values: Sum of NetSales, Count of OrderID
- Key finding: [fill in]

### PT4 — Payment Method Breakdown

- Rows: PaymentMethod
- Values: Count of OrderID, Sum of NetSales
- Key finding: [fill in]

### PT5 — Discount Impact

- Rows: Category
- Values: Sum of GrossSales, Sum of NetSales, Average of Discount
- Calculated Field: Revenue Retained = NetSales / GrossSales
- Key finding: [e.g. "Bags had the highest discount rate"]

---

## Calculated Fields (New Rows)

- Where to find: Analyze tab → Fields, Items & Sets → Calculated Field
- What it does: creates a brand new column using a formula based
  on existing fields — Excel calculates it per row automatically
- When to use: when you need a ratio, percentage, or derived metric
  that doesn't exist in your raw data
- Supply chain use case: calculating fill rate, margin %,
  supplier discount rate

---

## PivotCharts (Visualization)

- Where to find: Analyze tab → PivotChart
- Chart updates automatically when pivot table filter changes
- Best chart types:
  - Bar/Column → comparing categories or sellers
  - Pie → showing share of total (e.g. region % of sales)
  - Line → showing trends over time (useful when data has dates)

---

## What I Struggled With

- understanding the meaning of each table data
- calculated field formula for PT 5 which I get error until I realize the field name must be same
- I misundertood when add Category as a column filter which I get error display on pivot table so I fix it when I just drop the category on Rows

## What I Want to Practice More

- I would like to do more practicing in different dataset to get more understanding

## Supply Chain Connection

Pivot tables answer questions like:

- Which product category drives the most revenue? (PT1)
- Which seller is most reliable/valuable? (PT2)
- Where are our strongest markets? (PT3)
- How are discounts affecting our margins? (PT5)

These are the same questions a supply chain analyst asks about
real supplier and inventory data.
