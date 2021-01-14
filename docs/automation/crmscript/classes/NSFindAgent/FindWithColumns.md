---
title: NSFindResults FindWithColumns(String storageType, String providerName, String storageKey, String[] desiredColumns, Integer pageSize, Integer pageNumber, NSArchiveOrderByInfo[] orderBy)
path: /EJScript/Classes/NSFindAgent/Member functions/NSFindResults FindWithColumns(String p_0, String p_1, String p_2, String[] p_3, Integer p_4, Integer p_5, NSArchiveOrderByInfo[] p_6)
intellisense: 1
classref: 1
sortOrder: 3678
keywords: FindWithColumns(String,String,String,String[],Integer,Integer,NSArchiveOrderByInfo[])
---


Execute a Find operation and return a page of results. The criteria for the Find are fetched from the restriction storage provider according to the given parameters.



* **storageType:** Restriction storage type specification, either 'Criteria' or 'Reporter' (or possible extensions)
* **providerName:** Name of archive provider that is to execute the search and return the result columns/rows
* **storageKey:** Storage key to be interpreted by the restriction storage provider, when it fetches criteria for the search
* **desiredColumns:** Array of column names desired for the result. Each name must match a column offered by the given archive provider.
* **pageSize:** Size of result set pages
* **pageNumber:** Result set page to return, 0 is the first page. When a call returns no rows, no further pages are available. Negative page numbers are interpreted as number of rows to skip.
* **orderBy:** Array of order by specifications. If it is null or empty, the row order is unspecified, database dependent, and might not be the same from call to call, depending on query execution plans. The unspecified order willgenerally not vary within pages of the same query.
* **Returns:** Results from search, containing column information and result rows.


