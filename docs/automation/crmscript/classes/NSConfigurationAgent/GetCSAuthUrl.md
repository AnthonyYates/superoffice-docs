---
title: String GetCSAuthUrl(String language, String programName, String action, String extraParameters)
path: /EJScript/Classes/NSConfigurationAgent/Member functions/String GetCSAuthUrl(String p_0, String p_1, String p_2, String p_3)
intellisense: 1
classref: 1
sortOrder: 1607
keywords: GetCSAuthUrl(String,String,String,String)
---


Will generate an url to the emarketing module



* **language:** By setting this parameter, you can change the CS language for the current user.
* **programName:** In this parameter you must specify which CS program you want to create an URL for. Valid examples are "ticket", "rms", "spm" etc.
* **action:** Here you can optionally specify the action for the current program. This will enable you to go to a specific screen.
* **extraParameters:** If an action is specified, you can specify extra parameters here. This can be used to set specific behaviour for the chosen screen/action. If an empty action is supplied, this parameter will be ignored.
* **Returns:** Returns a valid CS URL composed of the give parameters.


