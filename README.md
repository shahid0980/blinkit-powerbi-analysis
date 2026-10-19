# Blinkit Sales Analysis (Power BI)

An interactive Power BI dashboard analysing orders, products, payments and delivery performance for a Blinkit-style quick-commerce dataset.

![Dataset cover](docs/assets/dataset-cover.png)

## Dashboard overview

The report (`report/blinkit.pbix`) has a main dashboard page with:

| Visual | What it shows |
|---|---|
| KPI cards | Total order amount, total number of orders, total quantity sold, product profit-margin count |
| Order Amount by Month (line) | Revenue trend over time |
| Quantity Sold by Month (column) | Units sold per month |
| Top 10 Selling Products (bar) | Best sellers by quantity |
| Order Amount by Payment Method (donut) | Revenue split across payment methods |
| Delivery Status (pie) | Share of orders by delivery outcome |

## Data model

Five tables in a star-style model:

- `blinkit_orders` – order header (date, payment method, delivery status)
- `blinkit_order_items` – line items (quantity, order amount)
- `blinkit_products` – product catalogue (name, profit margin)
- `blinkit_customers` – customer details
- `blinkit_inventory` – stock data

## Repository structure

```
.
├── report/
│   └── blinkit.pbix        # Power BI report (open in Power BI Desktop)
├── docs/
│   └── assets/             # Images used in this README
├── .gitignore
├── .gitattributes
├── LICENSE
└── README.md
```

## How to use

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Windows).
2. Clone this repo and open `report/blinkit.pbix`.
3. Use the slicers and cross-filtering to explore.

## Key insights

_Add your findings here, for example:_

- Which months drove the highest revenue?
- Which payment method contributes the most?
- What share of orders were delayed or cancelled?
- Which products dominate sales?

## Tools

Power BI Desktop, DAX, Power Query

## Add dashboard screenshots

Export each page from Power BI (File → Export → PDF, or screenshot) into `docs/assets/` and embed with `![Dashboard](docs/assets/dashboard.png)`.
