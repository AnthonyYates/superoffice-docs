---
title: Void toParser(Parser parser)
path: /EJScript/Classes/Message/Member functions/Void toParser(Parser parser)
intellisense: 1
classref: 1
sortOrder: 559
keywords: toParser(Parser)
---


This function loads many fields of the message to the input parser.




###Parameter:###


 - Parser parser. The parser that the message values is loaded into.


The fields will be loaded as: message.value


###The fields loaded are:###


 - message.id, The id of the message
 - message.slevelInteger, The security level of the message Internal = 1, External = 2
 - message.slevel, The security level of the message as a String, according to the active user's language.
 - message.createdAt, The datetime when the message is created in format 12. jan 1998, kl. 11:23.
 - message.createdAtRaw, The datetime when the message is created in format 1998-01-12 11:23:15
 - message.author,  The author of the message
 - message.bodyHtml, The html body of the message
 - message.messageCategory, The messageCategory, can be:  Message = 0, Bounce = 1, OutboxFailed = 2
 - message.body, The body of the message, if this is a plaintext message, this text will be returned with activated links
 - message.bodyPlain, The body of the message exactly as saved in database.
 - message.header, The message header
 - message.mailSorter, If this message is a recieved mail, the this is the name of the mail filter that took it.
 - message.x\_myextrafield, The value of the extrafield


