---
title: InvoiceEntry
path: /EJScript/Classes/InvoiceEntry
intellisense: 1
classref: 1
sortOrder: 430
---

This class represent invoice entries. You will be able to create new or modify existing invoice entries with this class.



###Example code:###


    InvoiceEntry i;
    
    i.setValue("description", "test");
    i.setValue("quantity", "1");
    i.setValue("pricePrUnit", "700");
    i.setValue("discount", "0.2");
    Date d; // Default value for date is today
    i.setValue("date", d.toString());
    i.save();




1. autolist

