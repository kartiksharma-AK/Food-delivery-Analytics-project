# Food Delivery Operations Analytics

**Project 8 | FoodTech / Logistics | Python Data Analytics**

## Objective
Analyse delivery orders to assess delivery performance, order outcomes, restaurant revenue, city-level operations, peak ordering hours, and payment-mode revenue.

## Dataset
`08_food_delivery.csv` contains 500 orders and these columns: Order_ID, City, Restaurant, Order_Value, Distance_km, Delivery_Time_Min, Order_Status, Payment_Mode, Order_Hour.

## Tools
- Python
- Pandas
- NumPy
- Matplotlib

## Tasks covered
109–123: dataset inspection, missing values, duplicate IDs, status shares, city delivery times, restaurant ranking and average order value, peak ordering hours, delivery time by status, city cancellation/delay rates, NumPy median and standard deviation, IQR outliers, delivery-time bands, revenue pivot by city/payment mode, and recommendations.

## Cleaning choices
- 7 delivery-time values are missing. These rows remain included in total-order, status and revenue analysis, but are excluded from delivery-time statistics rather than assigned invented times.
- There are no duplicate Order_ID values.
- Delivery-time bands use project-defined thresholds: Fast <= 30 min; Standard 31–45 min; Delayed > 45 min. These are analytical labels, not external service standards.
- IQR outlier flags are not automatically deleted; they are preserved for investigation.

## Run
1. Place the CSV and `food_delivery_analysis.py` in the same folder.
2. Install packages: `pip install pandas numpy matplotlib`
3. Run: `python food_delivery_analysis.py`

The script creates `outputs/` and `charts/`.

## Deliverables
- `food_delivery_analysis.py`: commented code for Tasks 109–123
- `outputs/`: analysis tables and text summaries
- `charts/`: six visualizations
- `SRS.docx`: requirements specification
