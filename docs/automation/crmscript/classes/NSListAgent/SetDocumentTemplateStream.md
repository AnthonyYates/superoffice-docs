---
title: NSDocumentTemplateEntity SetDocumentTemplateStream(NSDocumentTemplateEntity documentTemplateEntity, NSStream stream, String languageCode, Integer pluginId)
path: /EJScript/Classes/NSListAgent/Member functions/NSDocumentTemplateEntity SetDocumentTemplateStream(NSDocumentTemplateEntity p_0, NSStream p_1, String p_2, Integer p_3)
intellisense: 1
classref: 1
sortOrder: 4186
keywords: SetDocumentTemplateStream(NSDocumentTemplateEntity,NSStream,String,Integer)
---


Store a document template from its stream. Since there is a potential for a name conflict (the file name stored by the document entity earlier may prove to be invalid), the (possibly amended) document entity is returned. The client should not assume that any earlier, cached entity information is valid.



* **documentTemplateEntity:** The document entity object that the binary data (document) should be stored to. Its file name may be amended by this call, see the return value
* **stream:** The document as a stream.
* **languageCode:** The language code ('en-US', 'nb-NO', etc). Use empty string if not supported or used.
* **pluginId:** The plugin id to store the template with. 0 for SOArc
* **Returns:** Since there is a potential for a name conflict (the file name stored by the document entity earlier may prove to be invalid), the (possibly amended) document entity is returned. The client should not assume that any earlier, cached entity information is valid.


