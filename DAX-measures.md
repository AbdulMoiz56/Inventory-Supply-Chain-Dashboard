# DAX Measures & Calculated Columns

Documentation for custom DAX measures used in the **Inventory & Supply Chain Management Dashboard**.

---

## Warehouse Utilization

Measures how much of total warehouse capacity is currently being used by inventory.

```dax
Warehouse Utilization =
DIVIDE(
    SUM('Inventory_SupplyChain_Dataset'[Inventory Level]),
    SUM('Inventory_SupplyChain_Dataset'[Warehouse Capacity])
) * 100
```

**Result:** 34.08%

---

## Day Sales of Inventory (DSI)

Estimates the average number of days it takes to sell through current inventory, based on annual Cost of Goods Sold (COGS).

```dax
Day Sales of Inventory =
DIVIDE(
    SUM('Inventory_SupplyChain_Dataset'[Inventory Level]),
    SUM('Inventory_SupplyChain_Dataset'[Cost of Goods Sold])
) * 365
```

**Result:** 15.56 days

---

## Inventory Turnover Ratio

Measures how many times inventory is sold and replaced over a given period — a higher ratio indicates more efficient inventory management.

```dax
Inventory Turnover Ratio =
DIVIDE(
    SUM('Inventory_SupplyChain_Dataset'[Cost of Goods Sold]),
    SUM('Inventory_SupplyChain_Dataset'[Average Inventory])
)
```

**Result:** 23.47

---

## Summary Table

| Measure | DAX Function | Result |
|---|---|---|
| Warehouse Utilization | `DIVIDE`, `SUM` | 34.08% |
| Day Sales of Inventory | `DIVIDE`, `SUM` | 15.56 days |
| Inventory Turnover Ratio | `DIVIDE`, `SUM` | 23.47 |
