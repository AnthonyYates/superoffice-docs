---
title: SuperOffice view of the world
uid: crmscript-domain
SortOrder: 15
---

SuperOffice has 5 important things:

* **Companies** in code and database references referred to as *contact*.
* **Associates** are SuperOffice users - employees of the company.
* **Projects** are a type of activity that usually involves several stakeholders and various types of other activities.
* **Activities** are things employees do with companies, contacts, projects, diary and sales.
  * appointments of various task types
  * documents
  * mailings and form submissions
  * chat sessions
* **Tickets** from Service are linked to persons who may or may not belong to a company.

You can [read more about the main tables](https://community.superoffice.com/documentation/SDK/SO.Database/html/TheMainTables.htm) in the developer documentation.

## Business rules

* Activities happen at a particular point in time.
* Sales are expected closed on a date in the future.
* Appointments are scheduled for a particular date and time.
* Documents are written on a specific day.
* Activities start on one day and finish on another.
* Time is important for activities.
* Companies and projects are not time-specific, but are linked to activities in time.

The appointment table contains foreign keys to all the other important tables, plus a date field (ActiveDate).

## Context-sensitive labels

| Real-world term | UI        | Database table  | CRMScript class |
|-----------------|-----------|-----------------|-----------------|
| company<br/>organization | company | contact  | Company         |
| person          | contact<br/>associate |     |                 |
| customer        | contact   | person          | Customer        |
| employee        | associate | associate       |                 |
| user account    | user      | ejuser          | User            |
| database owner  | tenant    | Company         |                 |
