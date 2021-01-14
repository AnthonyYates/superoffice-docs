---
title: NSAppointment[] GetMyDiary(DateTime startTime, DateTime endTime, Integer count)
path: /EJScript/Classes/NSAppointmentAgent/Member functions/NSAppointment[] GetMyDiary(DateTime p_0, DateTime p_1, Integer p_2)
intellisense: 1
classref: 1
sortOrder: 849
keywords: GetMyDiary(DateTime,DateTime,Integer)
---


Method that returns a specified number of appointments within a time range. It only returns appointments that would be displayed in the user's diary. The appointments belong to the currently logged on user.



* **startTime:** The start of the time interval we want appointments from. This will usually be the current time.
* **endTime:** The end of the time interval.
* **count:** The maximum number of appointments that should be returned. -1 means no count restrictions.
* **Returns:** Array of Appointments.


