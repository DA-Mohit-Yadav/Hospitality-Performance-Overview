# Hospitality Performance Overview

![Hospitality Dashboard Preview](./Images/dashboard.png)

This project is a Power BI dashboard built to analyze hospitality business performance across revenue, bookings, occupancy, realization, ADR, and RevPAR. The report is designed for quick executive review with KPI cards, trend visuals, city and category comparisons, weekday revenue patterns, and weekly operational breakdowns.

## Dashboard Highlights

- Tracks core business KPIs including `Realized Revenue`, `Gross Booked Revenue`, `ADR`, `RevPAR`, `Total Bookings`, `Occupancy`, and `Realization`.
- Supports interactive slicing by `city`, `property_name`, `room_class`, and `Month`.
- Compares realized and booked revenue over time.
- Breaks revenue down by city, day name, category, and room class.
- Includes weekly operational performance metrics such as `DBRN`, `DURN`, `BRN`, and `RevPAR`.

## Data Model

### Dimension Tables

- `DimDate`: date, month label (`mmm yy`), week number, and day type
- `DimHotels`: property, category, and city
- `DimRooms`: room class reference

### Fact Tables

- `FactBookings`: booking-level operational and revenue data
- `Fact_AggregatedBookings`: aggregated capacity support table

## Key Measures In The Model

- `Realized Revenue`
- `Gross Booked Revenue`
- `ADR`
- `RevPAR`
- `Total Bookings`
- `occupancy`
- `Realization`
- `Revenue PM`
- `Revenue PW`
- `Revenue LY`
- `Rev MOM %`
- `MoM Display`
- `MoM Color`
- `ADR WoW %`
- `Occupancy WoW %`

## MoM Card Logic

The dashboard includes measure logic for Month-over-Month performance indicators on card visuals:

- `Rev MOM %`: calculates percentage change in realized revenue versus previous month
- `MoM Display`: shows an up arrow for growth and a down arrow for decline
- `MoM Color`: applies green for positive movement and red for negative movement

This pattern is useful for KPI cards where users need a quick visual signal beyond the numeric value.

## Business Questions Answered

- How much realized revenue and booked revenue did the business generate?
- Which cities contribute the highest realized revenue?
- Which day of the week drives the strongest revenue?
- How do room classes and property categories contribute to revenue mix?
- How are occupancy, ADR, RevPAR, and realization trending over time?
- How do weekly operational metrics compare across selected filters?

## Report Experience

The dashboard is built for fast scanning:

- a top filter bar for quick segmentation
- high-visibility KPI cards for headline metrics
- supporting trend and composition visuals for diagnosis
- a weekly detail table for operational drilldown

## Contact

<p align="left">
  <a href="https://github.com/DA-Mohit-Yadav" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-DA--Mohit--Yadav-181717?style=for-the-badge&logo=github" />
  </a>
  <a href="https://www.linkedin.com/in/mohit-yadav-0394b224a/" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-Mohit%20Yadav-0A66C2?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="mailto:mohitkaninwal12@gmail.com">
    <img src="https://img.shields.io/badge/Email-mohitkaninwal12%40gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</p>

If you'd like to collaborate, discuss machine learning projects, or connect professionally, feel free to reach out.
