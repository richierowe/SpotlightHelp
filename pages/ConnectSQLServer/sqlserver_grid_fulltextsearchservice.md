---
title: Full Text Search Service Grid
last_updated: July 29, 2016
summary: ""
sidebar: c_sqlserver_sidebar
permalink: sqlserver_grid_fulltextsearchservice.html
id: supportservices2_fts.ftsgrid
folder: ConnectSQLServer
---

<note type="note">In full-text indexing, a separate catalog is maintained that indexes each word in a database field as a separate index entry. The Full Text Search Service grid displays performance details for all full-text indexes on the server.</note>


The Full Text Search Service grid contains the following columns:

## Database Name

The name of the database where the tables in the Full Text Catalog reside.

## ID

The Full Text Catalogue ID.

## FTC Name

The Full Text Catalog Name.

## Status

The status of the full-text catalog (for example, Idle, Building Index, Paused).

## Index Size MB

The size of the full-text index, rounded to the nearest megabyte.

## Item Count

The number of items in the full-text catalog.

## Path

The location on disk of the full-text catalog.

## Last Populated

When the full-text catalog was last populated.

## Table Count

The number of tables in the full text catalog.



<note type="note">If some of the details are incomplete for all of the rows, the Full Text Search Service may not be running.
Check the Services Status grid on the Service Status page to confirm this.</note>


{% include links.html %}
