---
title: ﻿Monitored Server - SQL Server Alarm Evaluation Failure Alarm
last_updated: July 29, 2016
summary: "Raised when a (specified alarm) failed to evaluate."
sidebar: c_sqlserver_sidebar
permalink: sqlserver_alarm_monitoredserver_alarmevaluationfailure.html
id: ruleevaluationfailure.alarm
folder: ConnectSQLServer
---



The specified alarm failed to evaluate.

To clear this alarm, go to the Alarms dialog for this connection and disable this alarm. Alternatively, you can add a disabled severity to the 'Monitored Server - Alarm Evaluation Failure' key for the particular alarm that is failing.

To do either of these:


1. Click **Configure \| Alarms**.
2. Select the connection where the alarm failed.
3. Select the alarm **Monitored Server - Alarm Evaluation Failure** for the connection type.
4. Select **Override default setting for alarm 'Monitored Server - Alarm Evaluation Failure'**.
5. Do one of the following:
        * To disable the alarm, select **Disable this alarm**.
        * To add a disabled severity:
            1. Click **Add**.
            2. From the Key value list, select the key that the alarm was raised for.
            3. With the key selected, click the Severity list and select **Disabled**.

{% include links.html %}
