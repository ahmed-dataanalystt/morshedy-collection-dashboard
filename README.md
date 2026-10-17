# Real Estate Collection Dashboard — Power BI

**Route Academy Data Analysis Diploma · Graduation Project**

An interactive 35-page Power BI report that tracks installment collections for a real estate developer (Morshedy Group) across **8 residential projects**: what has been collected, what is still outstanding, and how collection splits by date, payment method and bank.

![Home page](Home%20Page.png)

---

## Business problem

The developer sells units on installment plans. Collection data lived in **8 separate project workbooks**, each with its own summary rows mixed into the data. Management had no single view of:

- How much has been collected vs. what remains outstanding, per project and overall
- How collection changes between periods
- How payments split between cash and bank, and across banks

## What I built

| Area | Details |
|---|---|
| **ETL (Power Query)** | Combined the 8 project workbooks (21 columns each) into one table, removed the embedded control rows (*Summary Total*, *Paid Installments*, *Remaining Installments*), and linked a reference table of adopted total units per project |
| **DAX** | Measures for collected vs. outstanding amounts, paid vs. remaining installments, and collection over time with old-vs-new period comparison |
| **Report design** | 35 pages: Home → 2 global pages → 4 pages per project (Overall, Cash, Bank, Bank-wise) × 8 projects, with button navigation from a central Home page |

## Report pages

**Global Summary**: a portfolio table for all 8 projects showing total units, units sold, unit price, invoice amount, amount collected, bank and cash outstanding, and outstanding balance.

![Global Summary](Global%20Summary.png)

**Collection By Date**: a period-driven table comparing collected and outstanding amounts between an old and a new period, per project.

![Collection by date](Collection%20by%20Date.png)

**Per project (×8)**: Overall, Cash, Bank and Bank-wise pages for One Kattameya, Skyline Katamya, Degla Landmark, Degla Palms 6th October, Lake Front 6, Crystal Plaza Maadi, Rihana and Zahra North Coast.

## Key insights

- About **94% of the invoiced amount has been collected** (13.09B of 13.88B), leaving **791M outstanding**.
- **Skyline Katamya** is the largest project, at about **40% of total collections** (5.19B).
- **Skyline Katamya, Degla Landmark and One Kattameya** hold about 60% of the outstanding balance (476M of 791M), which is where collection follow-up matters most.
- Outstanding amounts are mostly bank-financed (522M bank vs. 269M cash).

## Tools

`Power BI` · `Power Query (M)` · `DAX` · `Data Modeling` · `Excel`

## Files

| File | Description |
|---|---|
| `El Morshedy Collection Dashboard.pbix` | The Power BI report (open with Power BI Desktop) |
| `*.png` | Report screenshots |

---

**Ahmed Khaled** · Data Analyst · [LinkedIn](https://linkedin.com/in/ahmed-khaled-347711287) · [GitHub](https://github.com/ahmed-dataanalystt)
