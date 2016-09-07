---
layout: post
title:  "E-book Lending System"
date:   2016-05-20 18:24:25
description: My research proposal assignment
categories:
- project
---

## Purpose of System
The purpose of the system is to build a system that will contain information about current electronic books (including audio books).

## System
The eBooks system should contain the following major subsystems:

1. GUI - the system will include a Web user interface in which users (readers, library members, eBook publishers (e.g., Penguin Books, and other user groups involved with books) interact with the system. A GUI can be used to enter some associated data (e.g., movies) and provide information concerning current use of the system. At a minimum, the system will include the provisions for site administrators to update and correct information in the database.
2. Reporting Module - the system includes reports that summarize the data. Reports will provide administrators with information concerning the electronic book inventory and purchasing patterns. At a minimum, the reports contain enough information to allow administrators to manage their inventory. For example, reports showing patterns in the number of requests are essential.
3. Interfaces - The system includes interfaces to external systems (e.g., e-book delivery systems, etc.) and a skeleton implementation of these systems to allow for adequate testing.
4. Database - Data used by the system is contained in a database. At a minimum, this data includes information on content and users.
5. Database batch update - The system includes the ability to update the database both manually (through a GUI) and through an automatic database update module whenever you identify an electronic data source for information in the DB.

## System Issues
1. The user interface for all users is a Web interface.
2. The system runs on a hardware server that supports a Java EE Web Container ( Java 8.0 and above and JSP 2.0 and above).
3. The system works for current releases of Safari, Chrome, Firefox, and IE browsers.
4. You can assume that browsers will support CSS 1, but not necessarily all of CSS 2.
5. User monitors is a minimum screen resolution of 800 x 600 and a maximum of 1920 x 1200.
6. The system uses a relational database (MySQL recommended).
7. All interface screens have the same look and feel, although differing look and feels can be provided for different types of users (e.g., faculty and staff).
8. The system is able to accommodate the number of accesses consistent with a small number of simultaneous users.

### Related Document
* [Requirement Document]({{site.baseurl}}/cse308/RequiremetDocument.pdf)
* [User case]({{site.baseurl}}/cse308/Usercase.pdf)
* [Link to Github](https://github.com/BobZcao/CSE308SB)
