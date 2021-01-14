---
title: String SubstituteTemplateVariablesWithCustomTags2(String source, Integer generatorEncoding, StringDictionary customTags, Integer contactId, Integer personId, Integer appointmentId, Integer documentId, Integer saleId, Integer selectionId, Integer projectId, String cultureName)
path: /EJScript/Classes/NSDocumentAgent/Member functions/String SubstituteTemplateVariablesWithCustomTags2(String p_0, Integer p_1, StringDictionary p_2, Integer p_3, Integer p_4, Integer p_5, Integer p_6, Integer p_7, Integer p_8, Integer p_9, String p_10)
intellisense: 1
classref: 1
sortOrder: 2539
keywords: SubstituteTemplateVariablesWithCustomTags2(String,Integer,StringDictionary,Integer,Integer,Integer,Integer,Integer,Integer,Integer,String)
---


Parse the source string, and replace any template variable tags with their values, based on the ID's given in the other parameters.\<p/>This method also takes a pair of arrays specifying custom tags and their values; these tags will be available during substitution in addition to all the existing tags. Custom values will override values otherwise set.



* **source:** Source string to parse for template variables. Such variables must have delimiters corresponding to the standard for the given generator encoding.\<p/>Non-text source data (such as the binary content of a .doc file) should be passed in as Base64.
* **generatorEncoding:** Encoding of source string. Non-text formats such as MsWord or Excel should be Base64 encoded in the source string.
* **customTags:** Dictionary of custom tag names and values. Each name should have exactly four characters. There should be exactly one value for each tag.
* **contactId:** Identifier for a contact
* **personId:** Identifier for a person
* **appointmentId:** Identifier for an appointment
* **documentId:** Identifier for a document
* **saleId:** Identifier for a sale
* **selectionId:** Identifier for a selection
* **projectId:** Identifier for a project
* **cultureName:** Name of culture to be used for culture-sensitive data, such as dates or multi-language texts. Use a blank string to accept whatever current culture is set on the server (possibly not a good choice in multinational organizations with a single server).
* **Returns:** Source string with templates substituted, using the same encoding as for the source (binary data will be returned in Base64).


