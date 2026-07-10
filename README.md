# Inventory & Supply Chain Management Dashboard

An interactive Power BI dashboard analyzing inventory levels, order fulfillment, and logistics performance across regions, warehouses, and suppliers.

## Overview

This project analyzes 1,200+ orders (2022–2024) to surface key supply chain KPIs — order accuracy, backorder rate, lead time, and transportation cost — enabling data-driven decisions on warehouse and supplier performance.

## Dashboard Preview

![Dashboard Overview](Dashboard_Overview.png)

## Key Metrics

| KPI | Value |
|---|---|
| Total Orders | 1,200+ |
| Order Accuracy | 91.3% |
| Backorder Rate | 9.7% |
| Avg Lead Time | 15.7 days |
| Avg Transportation Cost | $7,700+ |
| Regions Covered | 4 |
| Warehouses | 3 |
| Suppliers | 4 |

## Features

- Cross-filtering slicers for Region, Category, Supplier, and Warehouse
- DAX measures (`SUM`, `DIVIDE`) for order accuracy %, backorder %, and average lead time
- Drill-down analysis on 3 years of transactional data
- Visual breakdown of transportation cost by region and supplier to flag optimization opportunities

## Dataset

`data/Inventory_SupplyChain_Dataset.csv` — 1,200 rows, 15 columns:

| Column | Description |
|---|---|
| Date | Order date |
| Region | North / South / East / West |
| Category | Product category |
| Supplier | Supplier A–D |
| Warehouse | Warehouse 1–3 |
| Order Status | Fulfilled / Pending / Canceled |
| Units Sold | Quantity sold |
| Inventory Level | Stock on hand |
| Transportation Cost | Shipping cost (USD) |
| Order Accuracy | TRUE/FALSE |
| Lead Time (Days) | Days from order to fulfillment |
| Backorder | TRUE/FALSE |
| Cost of Goods Sold (COGS) | USD |
| Average Inventory | Average stock level |
| Warehouse Capacity | Max warehouse capacity |

## Tools

- **Power BI Desktop** — data modeling, DAX measures, visuals
- **DAX** — SUM, DIVIDE for KPI calculations

## Repository Structure
