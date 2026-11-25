<img width="1257" height="495" alt="Screenshot 2026-11-25 204916" src="https://github.com/user-attachments/assets/991a9309-2797-450c-8bb2-47abb5fd027d" /># Container Import & Port Clearance Performance

An end-to-end logistics analytics project analyzing container clearance turnaround times, demurrage exposure, and port charges across origin lanes and clearing agents.

## Overview
- *Dataset:* clean_container_shipments (320 cleaned shipment records sourced from MySQL)
- *Tools:* MySQL, Tableau Public
- *Interactive Dashboard:* [View Live Dashboard on Tableau Public]((https://public.tableau.com:9443/views/ContainerImportClearancePerformance/ContainerImportPortClearancePerformance?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link))

<img width="1257" height="495" alt="Screenshot 2026-11-25 204916" src="https://github.com/user-attachments/assets/918665e6-4b46-4018-bb1e-4b44d7ba3934" />


## Key Findings
- *Clearing Agent Bottleneck:* *Horizon Port Clearing* recorded a *16.3-day average turnaround* and *$80.6k in demurrage*, highlighting clearance delays as a major cost driver.
- *High-Cost Lanes:* *Body & Suspension Parts* shipped from *Dubai* and *Hamburg* stood out among high-charge lanes, warranting closer review of freight/port fees and clearance efficiency.
- *Executive Cost & Volume Metrics:* Built Total Port Charges ([Clearing Fee Usd] + ZN([Demurrage Cost Usd])) alongside views for agent performance, port/cargo charges, monthly turnaround trends, and distinct container counts (320).

## Dashboard Structure
- *KPI Summary:* High-level view of demurrage cost, total port charges, average turnaround days, and distinct container count.
- *Agent Turnaround & Demurrage:* Compares clearing agents on turnaround speed and demurrage exposure.
- *Charges by Port & Cargo:* Breaks down total port charges by origin port and cargo category.
- *Monthly Turnaround Trend:* Tracks average turnaround days across arrival months with global Clearing Agent filtering across all sheets.

## Repository Structure
- sql/ — MySQL data cleaning and query scripts
- data/ — Cleaned shipment dataset (clean_container_shipments)
- docs/DATA_CLEANING_LOG.md — Summary of data cleaning rules, null handling, and validation steps
- dashboard_preview.png — Screenshot of the published Tableau dashboard
