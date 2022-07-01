---
uid: help-en-specifying-search-criteria
title: Specifying search criteria
description: Specifying search criteria
author: SuperOffice RnD
so.date: 06.29.2022
keywords: Settings and maintenance
so.topic: help
language: en
---

# Specify search criteria

You can specify search criteria for both individual words (for example *Peter*) and phrases consisting of several words (for example *Oliver Peter Nielsen*).

To specify the search criteria for a freetext search:

1. Click the **Options** button in the Navigator (![icon](../media/Knapp-Systemvalg-liten.bmp)).

2. Select the **Free text search** tab.

3. Check that freetext search is enabled for SuperOffice CRM (see [Enable freetext search](Enabling-freetext-search.md)).

4. Choose one of the following for **Single-word search operator**:

    * **Starts with**: a search for *pet* returns *Peter* and *Peterson* as hits.
    * **Contains**: a search for *eter* returns *Peter* and *Peterson* as hits.
    * **Exact match**: a search for *Peter* only returns *Peter* as a hit.

    > [!NOTE]
    > The **Exact match** option is the least resource-intensive when searching, while the **Contains** option is the most resource-intensive.

5. Choose one of the following for **Multi-word search operator**:
    * **Starts with**: a search for *pet* returns *Peter Nielsen* as a hit.
    * **Contains**: a search for *pet* returns *Oliver Peter Nielsen* and *Alan Peterson* as hits.
    * **Exact match**: only a search for *Oliver Peter Nielsen* returns *Oliver Peter Nielsen* as a hit.

    > [!NOTE]
    > When searching for phrases consisting of several words, a search is made for all the words together.