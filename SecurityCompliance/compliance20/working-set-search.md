---
title: "Query the data in a working set"
ms.author: markjjo
author: markjjo
manager: laurawi
ms.date: 
ms.audience: Admin
ms.topic: article
ms.service: O365-seccomp
localization_priority: Normal
ms.collection: M365-security-compliance 
search.appverid: 
- MOE150
- MET150
ms.assetid: 

description: ""
---

# Query the data in a working set

In most cases, it will be useful to be able to dig deeper into what is there in a working set and organize them to review more efficiently. Queries within a working set enables you to do so by letting you focus on a subset of documents that meet the criteria defined by you at once.

## Creating and running a query within a working set

In order to create and run a query within your working set, click on "New Query" in your working set. After you name your query and define the conditions, click "Save" to run the query. To run a query that has been previously saved, simply click on the saved query. Refer to [Document metadata fields](document-metadata-fields.md) for a list of metadata you can search by.

## Building your query

You can build your query using a combination of condition cards and query language in the Keywords condition card.

### Condition card

Every searchable field in a working set has a corresponding condition card that you can use to build your query.

There are multiple types of condition cards:
- Freetext: freetext condition card is used for text fields such as subject. You can list multiple search terms by separating them out with a comma.
- Date: date condition card is used for date fields such as last modified date.
- Search options: search options condition card will provide a list of possible values for the particular field in your working set. This is used for fields such as sender, where there is a finite number of possible values in your working set.
- Keyword: keyword condition card is a specific instance of freetext condition card that you can use to search for terms, or use KQL-like query language in. See below for more detail.

### Query language

In addition to condition cards, you can use a KQL-like query language in the Keywords card to craft your query. The query language supports standard KQL syntax like AND, OR, NOT, and NEAR(n). It also supports single-character wildcard (?) and multi-character wildcard (*).