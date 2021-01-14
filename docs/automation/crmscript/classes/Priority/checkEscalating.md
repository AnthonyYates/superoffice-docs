---
title: Void checkEscalating(Integer ticketId, Integer action)
path: /EJScript/Classes/Priority/Member functions/Void checkEscalating(Integer ticketId, Integer action)
intellisense: 1
classref: 1
sortOrder: 8966
keywords: checkEscalating(Integer,Integer)
---


This method will check if the ticket should change its alert level based on the priority and action. If it is to change, the alert level and alert timeout for the ticket will be updated.
This method is usefull if you want to change the state of a ticket that is monitored by the its priority. It will take care of all the escalation routines so you do not have to do this manually.



* **ticketId:** The id of the ticket to check
* **action:** The action that triggered this escalation. Possible values are:
Ticket changed owner = 0
Ticket change owner = 1
Ticket recieved new information = 2
Ticket closed = 3
Ticket changed priority = 4
New ticket = 5


