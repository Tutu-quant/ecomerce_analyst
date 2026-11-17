# Business Insights

**Project:** Olist Brazilian E-Commerce Analytics  
**Dataset:** `olist_order_items_dataset.csv`  
**Analysis Period:** Initial Data Exploration  
**Status:** In Progress
**Total record:** 112,650

## 1.1 Product Price Analysis

- Average product price: 120.65
- Median product price: 74.99
- Minimum product price: 0.85
- Maximum product price: 6,735.00

Initial observation:

- Mean is considerably higher than median, suggesting a right-skewed price distribution.

- A small number of high priced products may influence the average product price.

Hypothesis to investigate:
- High-priced products may have disproportionate impact on total revenue.

## 1.2. Freight Value Analysis
- Avg freight value: 19.99
- Median freight value: 16.26
- Minimum freight value: 0.00
- Maximum freight value: 409.68

Initial observation:
- Mean is considerably higher than median, suggesting a right-skewed price distribution.

- Some records have zero freight value.

- Maximum freight value is considerably higher than the median.

Hypotheses to investigate:
- High freight values may be associated with product weight,dimensions, or delivery distance.

- Zero freight values may represent valid business cases or potential data quality issues.

## 1.3 Data Quality Investigation

The following items require further investigation:

1. Identify the products with the highest prices.
2. Count and inspect records with zero freight value.
3. Investigate unusually high freight values.

### Status: Preliminary findings. No data has been modified or removed.

## 1.4 Freight Value - Preliminary Observation
- 383 records (approximately 0.34% of all order items) have zero freight value.

- These records still contain positive product prices.

- Further investigation is required to determine whether zero freight values are associated with specific products or business policies.

## 1.5 Zero Freight Analysis by Product
Key findings:
- 383 order_item records (0.34% of all records) have zero freight value.

- Zero freight records are concentrated in a small number of products.

- Product 53b36df67ebb7c41585e8d54d6772e08 has 187 zero-freight records out of 323 occurrences, representing 57.89%.

- Product aca2eb7d00ea1a7b8ebd4e68314663af has 98 zero-freight records out of 527 occurrences, representing 18.60%.

- Product 422879e10f46682990de24d770e7f83d has 56 zero-freight records out of 484 occurrences, representing 11.57%.

### Business interpretation:

Zero freight values may be associated with specific products or business conditions. However, further investigation is needed before
atttributing them to free-shipping policies.

### Next investigation:

- Join product data to identify product categories
- Compare zero-freight and non-zero-freight records.
- Investigate whether these patterns are related to product
  characteristics or sell behavior.

### Status: Preliminary finding - requires validation.