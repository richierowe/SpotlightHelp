---
title: SQL Agent - Long Running Jobs (Percent) Alarm
last_updated: July 29, 2016
summary: "The SQL Agent - Long Running Jobs (Percent) alarm is raised when a SQL Agent job has been running for considerably longer than the average run time for SQL Agent jobs of its type."
sidebar: c_sqlserver_sidebar
permalink: sqlserver_alarm_sqlagent_longrunningjobs_percent.html
id: longrunningjobs.alarm
folder: ConnectSQLServer
---




The default threshold for this alarm is 200% of average run time.

When this alarm is raised, open the Support Services drilldown \| SQL Agent Jobs page to investigate the long running SQL Agent Job.

You can customize the threshold to a value more suitable for your environment. You can customize a severity table for a SQL Agent job - see "Configure Keyed Alarms" in the online help for more information.


{% include links.html %}
