---
title: Tags
summary: "Tags are a free form organizational tool that may be optionally applied to Spotlight Connections. Tag names represent a project, geographic region or other indicator of interest to you and your organization. Multiple tags can be assigned to one connection."
sidebar: p_enterprise_sidebar
permalink: enterprise_connect_tags.html
folder: SpotlightEnterprise
---





## Possible applications for tags

Tags are a way for you to group your connections in a way that is meaningful to you, independent of the connection name and connection type. Here are some possible applications for tags in Spotlight Enterprise.


### Select Connections dialog

Search for Spotlight Connections by tag name.

### Alarm Action dialog

Configure an Alarm Action for Spotlight to make when an alarm is raised. The Alarm Actions can be conditional on the tag name.  

### Send an Email dialog

Configure an Alarm Action to send an email when an alarm is raised. The tag name for the affected Spotlight Connection can be included in the email subject or message.


### Run a Program dialog

Configure an Alarm Action to run a program when an alarm is raised. The tag name for the affected Spotlight Connection can be included in the program output.



## How to list all the tags assigned to a Spotlight Connection

From the Spotlight Client

1. Click **Configure \| Connections**.
2. Right-click on the connection and select **Properties \| Tags**.

## Example tag names and notes on tag names

Example tag names are:

```
   #Country.USA
   #APP.Finance
   #APP.HR
```

*  Use the drop down menu to select from tags currently assigned to connections on the Spotlight Diagnostic Server.
*  A tag can be made up of alphanumeric and special characters. It can include spaces within the name and value. It is not case sensitive.
*  Duplicate tags are not allowed.
*  Tag names are prefixed with the # character. A tag name cannot begin with the # character as in ##owner.bob.

## How to Replace a tag assigned to the Spotlight Connection

Use to modify a tag in the list of tags.

1. Click **Configure \| Connections**.
2. Right-click on the connection and select **Properties \| Tags**.
3. Select the tag in the list of tags.
4. The tag appears in the **Value** field. Edit as required.
5. Click **Replace**.

## How to Add a tag to the Spotlight Connection

1. Click **Configure \| Connections**.
2. Right-click on the connection and select **Properties \| Tags**.
3. Create a tag in the **Value** field.
4. Click **Add**.

## How to Delete a tag from the Spotlight Connection

1. Click **Configure \| Connections**.
2. Right-click on the connection and select **Properties \| Tags**.
3. Select the tag in the list of tags.
4. The tag appears in the **Value** field.
5. Click **Delete**.

{% include note.html content="Read-only users cannot Add, Replace and Delete tags. For more information, see Spotlight diagnostic user groups." %}

{% include tip.html content="The Connection Discovery Wizard imports details to SQL Server instances or Windows Servers from file. If you re-import the same file with updated tags, Spotlight will skip the connection creation step but update the tags." %}


{% include links.html %}
