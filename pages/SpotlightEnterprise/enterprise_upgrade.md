---
title: Upgrade Spotlight Enterprise
tags: [setup]
keywords: setup, install
summary: "Upgrade Spotlight Enterprise using the Spotlight Enterprise installer."
sidebar: p_enterprise_sidebar
permalink: enterprise_upgrade.html
folder: SpotlightEnterprise
---


## Upgrade from versions
To upgrade from an earlier version of Spotlight on SQL Server than 10.0, upgrade to at least version 10.0 before upgrading to 11.6.

To upgrade from Spotlight on SQL Server 10.5.0, first upgrade to 10.5.2 and then upgrade to 11.6.

## Backup first
Backup all Spotlight configuration and saved collection data before you run the Spotlight on SQL Server executable.

## Run the Spotlight on SQL Server executable on each Spotlight Client
If your enterprise has multiple Spotlight Clients then ensure all Spotlight Clients are included in the upgrade process. If the Spotlight Client and Spotlight Diagnostic Server are running different versions of Spotlight on SQL Server, the client will be unable to connect to the Spotlight Diagnostic Server.

## Upgrade the Playback Database and Spotlight Statistics Repository
Following upgrade of the Spotlight Diagnostic Server, the Playback Database and Spotlight Statistics Repository are automatically upgraded the next time they are accessed by the Spotlight Diagnostic Server. If in your environment the Playback Database / Spotlight Statistics Repository are replicated as per a Microsoft Replication database the upgrade can fail if schema changes are required that can only be made when replication is turned off. To successfully upgrade, the steps are to: turn replication off, upgrade the Spotlight Diagnostic Server, then reenable replication.

## What configuration information is preserved on upgrade?
The following information on the Spotlight Diagnostic Server is preserved when you upgrade:

*  Connection properties for all monitored servers (including changes to scheduling and alarms)
*  Enterprise views
*  Collection properties
*  Alarm Actions (These include running a program and sending an email.)
*  Planned Outages
*  Global options such as user-created Error Log rules
*  Configuration information for the Spotlight Statistics Repository (this applies only if you installed the Spotlight Statistics Repository from an earlier version of Spotlight on SQL Server) and the Playback Database.

## Upgrade from Spotlight on SQL Server Enterprise 11.2 and alarms requiring acknowledgment
The Spotlight factory settings for alarms requiring acknowledgment changes on upgrade from Spotlight 11.2. Only Connection Failure alarms are now factory set to require acknowledgment.

The alarms that were factory set to require acknowledgment in Spotlight 11.2 and earlier are as follows. They are included here so you can choose to manually enable them to require acknowledgment again post upgrade if required.

*  Availability Group - Failed Over
*  Clusters - Failed over
*  Diagnostic Server - Auto Update Success
*  Error Log - Error Count
*  LiteSpeed Backup Failed
*  LiteSpeed Backup Warning
*  Locks - Blocked Processes
*  Locks - Deadlocks
*  Mirroring Failedover
*  SQL Agent - Jobs Failed

## Upgrade from Spotlight on SQL Server Enterprise 11.1.x or earlier and Spotlight Mobile
If you used Spotlight 11.1.x or earlier to monitor your Spotlight on SQL Server connections on a mobile device and intend to continue monitoring your connections on a mobile device then the following additional upgrade instructions are required.

1. Uninstall the **Spotlight Web Publisher** via **Windows \| Control Panel \| Programs and Features**. The Spotlight Web Publisher was required in the past to monitor SQL Server connections on a mobile device. It is now important that you uninstall it. By default the Spotlight Web Publisher was installed on the same computer as the Spotlight Diagnostic Server.

2. From the Spotlight Client, click **Configure \| Spotlight Cloud**. Select **Upload data to Spotlight Cloud**. Ensure your Spotlight Cloud (Spotlight Essentials) account details are correct.

{% include links.html %}
