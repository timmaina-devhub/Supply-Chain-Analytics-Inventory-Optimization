# Supply Chain Analytics & Inventory Optimization

## 1. Project Overview

This project presents an end-to-end supply chain analytics solution designed to improve demand forecasting, reduce stockouts, and optimize inventory management across multiple warehouses.

The solution combines time series forecasting with operational analytics and inventory optimization techniques to enhance supply chain efficiency and support data-driven decision-making.

---

## 2. Business Problem

Supply chain operations face multiple inefficiencies, including frequent stockouts, excess inventory, poor demand forecasting accuracy, and unreliable supplier performance.

Approximately 12% of SKU-days result in stockouts, leading to significant lost sales, while large amounts of capital remain tied up in slow-moving inventory across warehouses. Existing Excel-based demand planning achieves low forecast accuracy and fails to capture seasonal demand patterns.

Additionally, supplier delays and bulk purchase anomalies distort demand signals, triggering reactive and costly inventory decisions.

---

## 3. Objectives

* Improve demand forecasting accuracy using time series models
* Identify and reduce stockout occurrences
* Detect overstock and low-velocity inventory
* Evaluate supplier reliability and delivery performance
* Design an inventory optimization framework (SS, ROP, EOQ)
* Enable data-driven supply chain decision-making

---

## 4. Dataset Description

The dataset consists of:

* SKU-level inventory data (stock levels, movements)
* Sales and demand data across time
* Supplier and shipment records (lead times, delays)
* Warehouse-level inventory distribution

These datasets were cleaned and transformed into structured formats for forecasting, inventory analysis, and supplier evaluation.

---

## 5. Methodology

### 5.1 Data Preparation

* Cleaned and standardized inventory and demand data
* Handled missing values and inconsistencies
* Engineered time-based features for forecasting
* Recalculated key metrics (e.g., stockout flags, stock levels)

---

### 5.2 Demand Forecasting

Models developed and compared:

* ARIMA (baseline statistical model)
* Prophet ✅ (best performer)

* Captured trend and seasonality patterns
* Generated monthly demand forecasts
* Improved forecast accuracy significantly over Excel baseline

---

### 5.3 Inventory Analysis

* Identified stockout events using recalculated inventory logic
* Analyzed stock distribution across SKUs and warehouses
* Detected imbalance between overstock and understock
* Evaluated inventory movement and availability trends

---

### 5.4 Supplier Performance Analysis

* Calculated delivery delays (`delay_days`)
* Identified extreme delays and unreliable suppliers
* Segmented supplier performance based on consistency
* Highlighted operational risks in logistics

---

### 5.5 Inventory Optimization Framework

Designed key inventory control models:

* Safety Stock (SS) for service level protection
* Reorder Point (ROP) for proactive replenishment
* Economic Order Quantity (EOQ) to balance holding and ordering costs

---

## 6. Model Performance

| Model   | MAPE (Error) | Accuracy | Notes                          |
|---------|-------------|----------|--------------------------------|
| Excel   | ~42%        | ~58%     | Baseline manual forecasting    |
| Prophet | ~23%        | ~77%     | Captures trend & seasonality ✅ |

* Significant improvement in demand prediction accuracy
* Reduced forecasting error by nearly half

---

## 7. Key Insights

* Forecast accuracy improved significantly using Prophet
* High frequency of stockouts indicates major availability gaps
* Overstock and understock imbalance exists across warehouses
* Supplier delays are a key driver of operational inefficiencies
* Seasonal demand patterns were previously unaccounted for
* Bulk order anomalies distort demand signals and forecasts

---

## 8. Challenges

* Handling inconsistent inventory and stock data
* Reconstructing accurate stockout indicators
* Managing demand volatility and anomalies
* Capturing seasonality using traditional models
* Aligning forecasting outputs with operational decisions

---

## 9. Conclusion

This project demonstrates how combining time series forecasting with supply chain analytics can significantly improve operational efficiency.

It highlights the importance of accurate demand forecasting, reliable supplier performance, and structured inventory policies in reducing costs and improving service levels.

---

## Project Structure

```
/marketing-attribution-roi-optimization
│
├── README.md
├── /data
├── /notebooks
└── /dashboard
```

## Future Work

* Budget optimization simulator

---
## Dashboard Preview

![Dashboard Preview](./x.png)

---
![Dashboard Preview](./y.png)

---
![Dashboard Preview](./z.png)
