---
title: String getValue(String colName)
path: /EJScript/Classes/Customer/Member functions/String getValue(String colName)
intellisense: 1
classref: 1
sortOrder: 184
keywords: getValue(String)
---

Returns the value of the given field of the customer.



###The following fields are available:###


 - id
 - name The name of the customer.
 - firstname
 - lastname
 - phone
 - cellphone
 - note
 - username: This is the usedname used for the external web.
 - password: This is the password used for the external web.
 - email: A list of all email addresses.
 - mainEmail: The main email address.
 - language: The name, languagecode or id of the customers language.
 - deleted
 - company: The id of the related company
 - display\_company: The value showing the name of the related company.
 - dbi\_agent_id
 - dbi\_key
 - dbi\_last_modified
 - dbi\_last_syncronized These values are for database integration
 - priority: The id or name of the customers priority.
 - our\_contact: The username, loginname or id of the related contact (user).
 - x_*: The extrafield with the given database field name.
[extra field] The extrafield with the given name (e.g. "Country").




###Example code:###


    Customer c;
    
    c.load(3);
    Bool b = c.checkTableRights("select");
    print(b.toString());
    
    c.setValue("name", "Test");
    print(c.getValue("name"));


