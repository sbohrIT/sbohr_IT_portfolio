# Loaner Stock Alert Automation

Overview
==================
The Loaner Stock Alert Automation project is designed to address the issue of stockout situations with loaner devices at Meta Helpdesks. This system proactively sends alerts to the proper point of contact whenever the stock of any loaner device at any site falls below the desired threshold, allowing our team to request more loaner devices from supply chain before a complete stockout event occurs.

Problem Statement
==================
At Meta Helpdesks, we were experiencing issues with stockout situations with loaner devices, leaving Meta employees unable to request the loaner device that they need while they wait for their replacement. The issue was stemming from the combination of:
Lack of visibility of loaner stock count, as devices are kept in an IT storage closet or dedicated room at each helpdesk.
Lack of accountability of the loaner re-fill request process, as Enterprise Support Techs are often rotated between helpdesks on a bi-weekly basis.

Solution
==================
Our solution consists of the following components:
- *SQL Queries*: Individual SQL queries retrieve the count of how many loaner devices are stocked at each office's helpdesk from the hourly supply chain hive table.
- *Metric Catalog*: The query is then converted into a metric through an internal metric catalog used to create, manage, and share metrics across the company.
- *Detector:* A detector is created from that metric which monitors time series data and triggers alerts when predefined conditions are met. Detectors are part of the monitoring infrastructure, enabling teams to detect anomalies, track metric violations, and ensure system reliability.
- *Oncall System*:
The detector fires an alert whenever any loaner device count falls below our desired threshold.
This alert automatically sends the desired message to the associated members in the oncall group, allowing proactive actions to be taken to prevent stockouts.

![Image description](https://github.com/sbohrIT/sbohr_IT_portfolio/blob/main/Meta-Projects/Landed%20Projects/Loaner_Stock_Automation_Flow.png)

Outcomes
==================
This solution was launched for all helpdesks in Meta's Menlo Park Headquarters Campus along with New York City offices, providing real-time visibility into loaner stock levels and enabling proactive management of loaner device inventory.
