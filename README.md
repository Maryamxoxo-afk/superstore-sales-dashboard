# Superstore Sales & Profit Dashboard

Interactive Excel dashboard analyzing retail sales, profit, and discounts from the Superstore dataset, built with PivotTables, charts, KPI cards, and slicers.

![Dashboard screenshot](dashboard.png)

## Problem
Where does this retail business make money, and where does it lose it? I set out to answer:
1. Which region and category earn the most profit?
2. Which sub-categories lose money?
3. Does a higher discount reduce profit?
4. Which states and cities bring the most sales, and which lose money?
5. Which customer segment and ship mode are the most profitable?

## Dataset
- Superstore sample dataset (Kaggle): 9,994 rows and 13 columns, 9,977 after cleaning
- Fields: ship mode, segment, location, region, category, sub-category, sales, quantity, discount, profit
- **Limitations:** no order date, order ID, or customer ID, so trends over time, customer counts, and average order value are not included. Averages are per order line.

## Process
1. **Explored** the data and wrote a data dictionary
2. **Cleaned** it: removed 17 duplicate rows, formatted postal codes as ZIP codes, added a Profit Margin column, and converted the data to an Excel Table
3. **Analyzed** each question with PivotTables
4. **Visualized** results with charts and KPI cards (total sales, total profit, profit margin, average discount)
5. **Added interactivity** with slicers connected to every pivot
6. **Summarized** findings and recommendations

## Key insights
- **Overall:** $2.30M in sales and $286K in profit, a **12.5% margin**.
- **Regions:** West ($108K) and East ($92K) earn the most profit. Central has $501K in sales but only $40K profit (about 8% margin).
- **Categories:** Technology ($145K) and Office Supplies ($122K) drive profit. Furniture brings $741K in sales but only $18K profit (about 2.5% margin).
- **Loss-making sub-categories:** Tables (-$17.7K), Bookcases (-$3.5K), and Supplies (-$1.2K).
- **Discounts:** Average profit per line is positive up to a 20% discount and negative from 30% upward. Lines discounted 20% or more lost $45K combined, while lines below 20% earned $331K.
- **States:** Texas (-$25.8K), Ohio (-$17.0K), and Pennsylvania (-$15.6K) lose money. California ($76K) and New York ($74K) are the most profitable.
- **Segments and shipping:** Consumer is the largest segment by sales but has the lowest margin (11.5%) vs Home Office (14.0%). Ship mode has little effect on margin.

## Recommendations
- Cap discounts at 20%, especially on Furniture, where deep discounts drive losses.
- Review pricing and costs on Tables and Bookcases before continuing to sell them at current terms.
- Investigate why Texas, Ohio, and Pennsylvania lose money (discounting, product mix, or shipping costs).
- Focus growth on Technology and Office Supplies in the West and East regions.

## Tools used
Excel, PivotTables, PivotCharts, calculated fields, slicers

## Files
- `superstore-sales-dashboard.xlsx`: the dashboard
- `SampleSuperstore.csv`: original data
- `dashboard.png`: screenshot
