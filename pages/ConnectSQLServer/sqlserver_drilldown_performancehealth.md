---
title: Performance Health drilldown
last_updated: July 29, 2016
summary: "Show information relating to the performance health of the SQL Server. The Performance Health drilldown is designed to provide a high level view of potential bottlenecks. "
sidebar: c_sqlserver_sidebar
permalink: sqlserver_drilldown_performancehealth.html
folder: ConnectSQLServer
---


The Performance Health drilldown assesses data from server level wait statistics (sys.dm_os_wait_stats).

## rating

### Healthy
 Database time is being spent productively on CPU and IO.

A performance-health rating of 80% or more is considered healthy.

If no performance-health rating is provided then the load being placed on the database is too low to assess its health. The database performance health is still considered to be healthy.

### Unhealthy
 Too much database time is spent waiting for bottlenecks such as locks and latches.

The Poor Performance Health Alarm is raised.


## Current Wait Rate
The current wait rate and this as a percentage of total available CPU time.


## Instance Wait Time
This bar chart provides a visual overview of where most of the wait time is being spent.

Color | Description
------|------------
Green | Bars colored green represent healthy wait time (CPU and I/O).
Yellow | If I/O is colored yellow then I/O latency is high.
Blue | Bars colored blue represent unhealthy wait time. Categories of unhealthy wait are: Latch, Lock, CLR, OTHER, DBM, DTC, Backup, Memory, Network, ServiceBroker, SOS and MISC.

Note:
* The bar chart shows only the categories currently contributing to wait time. The bar chart adjusts itself dynamically in real time.
* Hover the mouse over each bar in turn to see a statistical summary.
* Click on a bar to open the SQL Server \| Wait Events Drilldown specific to the represented category of wait.


## I/O Latency

Use this chart to check the responsiveness of the I/O subsystem by measuring the single-block-read latency. I/O latency is low in a healthy system to indicate that the time being spent on I/O is productive.

The position of the pin on the chart indicates the current I/O latency.


{% include links.html %}
