# battery-fleet-availability-analysis
Python (Pandas) analysis of availability and operating behaviour of grid-scale Scottish batteries
**Work in progress** — analysis and full write-up being added.

## Question
How available and reliable are grid-scale batteries in practice? This project analyses real metered data from five ~50 MW Scottish battery storage sites to measure availability, downtime, mean time between failures (MTBF) and abnormal behaviour.

## Data
Public half-hourly metered data from Elexon (GB electricity balancing mechanism).

## Progress so far
- Identified battery units from Elexon's register of 3,128 BM units (fuel type blank for 81%, so filtered by name and validated results)
- Pulled six months of half-hourly data (43,925 rows) for five batteries and checked completeness against 48 readings per day
- Resolved sign conventions (charging is negative) and UTC vs settlement-period timing

## Next
- Availability and downtime analysis
- MTBF across the fleet
- Automated anomaly detection

**Tools:** Python, Pandas, Jupyter
