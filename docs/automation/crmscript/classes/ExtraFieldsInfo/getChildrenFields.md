---
title: Void getChildrenFields(Integer type, Integer extraTableTarget)
path: /EJScript/Classes/ExtraFieldsInfo/Member functions/Void getChildrenFields(Integer type, Integer extraTableTarget)
intellisense: 1
classref: 1
sortOrder: 310
keywords: getChildrenFields(Integer,Integer)
---

This function loads extra fields of the type given in the first parameter. If the type is an extra table relation, the second pointer is the id of the extra table it points to.

Unless type is 20 (extratable) the second parameter won't do anything.

If you want all extra fields pointing to the extra table with id 5, you'd call getChildrenFields(20, 5)

If you want all extra fields of type Dat you'd call getChildrenFields(3, 0)




###Types can be:###

Integer                   =  1
Text (long)              =  2
Date                       =  3
DateTime                =  4
Time                       =  5
Bool                        =  6
TimeSpan                =  7
Text (short)              = 10
Customer relation     = 16
Company relation     = 17
Ticket relation          = 18
User relation            = 19
Extra table relation   = 20
Attachment relation  = 22
Link                        = 23
Category relation     = 24
Priority relation        = 25
FAQ relation             = 26


