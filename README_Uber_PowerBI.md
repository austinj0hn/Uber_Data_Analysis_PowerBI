# Uber Data Analysis Dashboard | Power BI

## Project Overview

This project analyzes Uber ride-booking data for **2025** using Microsoft Power BI. The interactive dashboard explores booking performance, revenue trends, vehicle-category performance, rider behavior, cancellations, and location-based demand.

The goal is to turn ride data into actionable insights that can help stakeholders understand business performance, identify operational challenges, and make data-informed decisions.

## Dashboard Pages

The report contains five analytical pages:

### 1. Overview
- Summarizes completed, lost, and total bookings.
- Tracks revenue and average trip distance.
- Shows monthly booking and revenue trends.
- Highlights top pickup and drop-off locations and customer/driver ratings.

### 2. Vehicle Analysis
- Compares vehicle categories by revenue, customer count, and bookings.
- Examines completed and lost bookings by vehicle type.
- Shows monthly revenue trends across vehicle categories.
- Highlights each category's contribution to total revenue.

### 3. Revenue Analysis
- Examines monthly revenue and average revenue per month.
- Compares revenue across time slots and payment methods.
- Identifies the top 10 locations by revenue.
- Includes a ranking control for exploring location performance.

### 4. Rider Analysis
- Reviews booking status and customer counts.
- Segments riders into first-time, return, and regular riders.
- Tracks cancellations over time.
- Examines customer- and driver-related cancellation patterns.

### 5. Location Analysis
- Tracks total distance by month and vehicle type.
- Compares booking demand by day of week and time slot.
- Supports switching between pickup and drop-off location views.
- Highlights locations with higher booking counts.

## Key Metrics

The dashboard reports the following headline metrics:

| Metric | Reported value |
|---|---:|
| Total bookings | 148.8K |
| Completed bookings | 92.6K |
| Lost bookings | 56.8K |
| Revenue | 51.8M |
| Total distance | 2.51M |
| Average distance | 24.64 km |
| Total customers | 104.1K |
| Successful customers | 64.6K |

*Values are displayed as reported in the dashboard; revenue currency and distance-unit definitions follow the underlying project dataset.*

## Key Findings

- Approximately **62% of bookings were completed**, while a substantial number were lost or cancelled.
- Revenue remained broadly consistent across the months, at roughly **4.0M–4.6M**.
- The **6 PM–9 PM** time slot showed the highest revenue and strong booking demand.
- **UPI** was the largest revenue-generating payment method in the dashboard.
- Driver cancellations were higher than customer cancellations.
- Auto and Bike categories contributed the largest shares of revenue among the vehicle categories.
- Some locations consistently appeared among the higher-revenue or higher-booking areas.

## Business Recommendations

Based on the dashboard findings, the report recommends:

- Improve driver availability during peak evening hours.
- Investigate driver cancellation patterns and consider appropriate incentive programs.
- Focus promotions on high-performing locations.
- Strengthen retention strategies for first-time riders.
- Align vehicle allocation with observed demand patterns.

## Data Model

The project report describes a simple star-schema-style model consisting of:

- **`uber_data`** — central table containing booking, revenue, distance, and status data.
- **`Date_tbl`** — date table supporting month- and quarter-based analysis.
- **`veh_image`** — table used for vehicle categorization and dashboard visuals.

This structure supports time-based analysis, KPI calculations, and relationships between the main booking data and supporting tables.

## Tools & Skills Demonstrated

- **Microsoft Power BI** — interactive dashboard development and visual analytics
- **DAX** — KPI and analytical measure development
- **Data Modeling** — relationships and date-table-based analysis
- **Data Visualization** — KPI cards, trend charts, comparisons, and breakdowns
- **Business Analysis** — interpreting trends and developing data-driven recommendations

## Repository Contents

Suggested repository structure:

```text
Uber-Data-Analysis-Power-BI/
├── README.md
├── Uber_PBI_Project.pdf
├── Uber_Dashboard.pbix
└── screenshots/
    ├── overview.png
    ├── vehicle.png
    ├── revenue.png
    ├── rider.png
    └── location.png
```

Update the filenames above to match the files you actually upload. Add dashboard screenshots to the `screenshots/` folder if you want the report previews to appear in this README.

## How to Explore the Project

1. Download the `.pbix` file from this repository.
2. Open it in **Microsoft Power BI Desktop**.
3. Navigate through the Overview, Vehicle, Revenue, Rider, and Location pages.
4. Use the available month/quarter, booking-status, vehicle, payment, cancellation, and location controls to explore the report.

> **Note:** The Power BI report may require its original data source to be available or reconnected before all visuals and interactions work correctly.

## Conclusion

This project demonstrates how Power BI can be used to analyze ride-booking performance across revenue, vehicles, riders, cancellations, and locations. It combines KPI reporting, time-based analysis, interactive visuals, and business recommendations in a multi-page dashboard.

---

**Author:** Austin John  
**Project:** Uber Data Analysis Dashboard  
**Tools:** Power BI · DAX · Data Modeling · Data Visualization
