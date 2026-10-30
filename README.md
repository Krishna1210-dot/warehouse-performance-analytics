# Warehouse Performance Analytics

A warehouse and supply chain analytics project using Python, SQL, SQLite, Pandas and Excel to analyse warehouse operations, inventory performance, order fulfilment and delivery costs.

This project uses synthetic warehouse data to demonstrate how data analytics can support operational decision-making and performance monitoring.

## Project Overview

The project analyses warehouse operations across four major areas:

* **Warehouse Productivity:** Evaluating picker productivity, fulfilment time and operational efficiency.
* **Inventory Management:** Analysing SKU movement, stock levels and replenishment requirements.
* **Demand Analysis:** Identifying peak ordering hours, daily trends and demand patterns.
* **Logistics Performance:** Analysing delivery costs, delivery outcomes and fulfilment performance.

## Tech Stack

| Technology | Application                      |
| ---------- | -------------------------------- |
| Python     | Data generation and processing   |
| SQL        | Warehouse operations analysis    |
| SQLite     | Relational database              |
| Pandas     | Data manipulation and analysis   |
| Excel      | Interactive analytical dashboard |
| OpenPyXL   | Excel dashboard generation       |

## Project Structure

```text
Warehouse-Performance-Analytics/
│
├── Data Files/
│   ├── orders.csv
│   ├── skus.csv
│   ├── pickers.csv
│   ├── deliveries.csv
│   └── [10 analytical output CSV files]
│
├── generate_data.py
├── analysis.py
├── dashboard.py
│
├── warehouse_ops.db
├── Warehouse_Dashboard.xlsx
├── requirements.txt
└── README.md
```

## Key Analytical Areas

The project performs 10 SQL-based analyses:

1. Picker Productivity (Units Per Hour)
2. SKU Velocity Analysis
3. Peak Hour Analysis
4. Daily Order Trends
5. Inventory Replenishment Alerts
6. Delivery Cost Analysis
7. Category-wise Fulfilment Time
8. Delivery Status Analysis
9. Day-wise Performance
10. Overall Warehouse KPI Summary

## Excel Dashboard

The project generates an Excel dashboard containing six analytical sheets:

| Dashboard Sheet        | Analysis                                     |
| ---------------------- | -------------------------------------------- |
| KPI Summary            | Overall warehouse performance indicators     |
| Picker Productivity    | Employee productivity and fulfilment metrics |
| SKU Performance        | Product movement and inventory performance   |
| Demand Patterns        | Hourly and daily order trends                |
| Delivery Cost Analysis | Delivery costs and logistics performance     |
| Replenishment Alerts   | Inventory stock monitoring                   |

## Sample Business Insights

The synthetic dataset contains 5,000 orders across 30 days.

Some observations from the analysis include:

* Peak ordering hours experience higher fulfilment times.
* Evening delivery slots have higher average delivery costs.
* A relatively small proportion of SKUs contributes a significant share of sales value.
* Picker productivity is relatively consistent across the eight pickers.
* Inventory analysis identifies products approaching their reorder levels.
* Delivery analysis provides a breakdown of delivered, delayed and returned orders.

**Note:** These observations are based on simulated data and should not be interpreted as actual warehouse performance findings.

## Installation

Install the required dependencies:

```bash
pip install pandas numpy openpyxl
```

## How to Run

Run the scripts in the following order:

**1. Generate datasets and SQLite database**

```bash
python generate_data.py
```

**2. Execute SQL analyses**

```bash
python analysis.py
```

**3. Generate Excel dashboard**

```bash
python dashboard.py
```

The final Excel dashboard will be saved as:

`Warehouse_Dashboard.xlsx`

## Dataset Information

The project uses synthetic datasets generated through Python.

| Dataset    | Records |
| ---------- | ------: |
| Orders     |   5,000 |
| SKUs       |      36 |
| Pickers    |       8 |
| Deliveries |   5,000 |

The data is intended for learning and analytical demonstration purposes.
