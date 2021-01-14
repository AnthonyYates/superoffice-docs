---
title: Void setValue(String colName, String value)
path: /EJScript/Classes/Ticket/Member functions/Void setValue(String colName, String value)
intellisense: 1
classref: 1
sortOrder: 9193
keywords: setValue(String,String)
---


Sets column colName to the given value.
Obs: For this to actually affect the ticket, you will have to use the function `save()` after you have set all the values you want.




###Parameter:###


 - colName
 - value: A String representation of the value to set




###Possible values are the extrafields on the ticket and the following:###


 - title
 - category: the category id
 - ownedBy: (owned\_by), the id of the user who owns the ticket
 - slevel: the security level of the ticket, 1 is internal, 2 is external
 - priority: the id
 - status: 1 = active, 2 = closed, 3 = postponed, 4 = deleted, 5 = composed
 - ticketStatus: (ticket\_status), the id of the custom status field
 - custId: the id of the primary customer
 - customers: comma separated list of customer ids
 - createdBy: the id of the user who posted the ticket, 1 if the ticket is posted into the system
 - author: a string containing the name of the ticket author
 - activate: the datetime when the ticket was activated
 - createdAt: (created\_at), the datetime when the ticket was created
 - repliedAt: (replied\_at), the datetime when the ticket first was replied at
 - stopEscalation
 - readStatus (read\_status)
 - deadline
 - filterAddress
 - timeToClose
 - realTimeToClose
 - dbiAgentId
 - dbiKey
 - dbiLastModified
 - dbiLastSyncronized


