---
title: NSArchiveConfiguration GetArchiveConfigurationWithContext(String guiName, String providerName, String context)
path: /EJScript/Classes/NSArchiveAgent/Member functions/NSArchiveConfiguration GetArchiveConfigurationWithContext(String p_0, String p_1, String p_2)
intellisense: 1
classref: 1
sortOrder: 1104
keywords: GetArchiveConfigurationWithContext(String,String,String)
---


Get the configuration for one archive, with context parameter. The configuration is keyed by a combination of archive provider name and gui name. The archive provider name must match an archive provider plugin; the gui name is an arbitrary string used to distinguish multiple occurrences of the same underlying provider in a gui.



* **guiName:** String that identifies the archive in the GUI, must be the same when fetching and storing configurations, but does not otherwise have to match anything.
* **providerName:** Name of archive provider, must match one of the plugins known to the ArchiveProviderFactory.
* **context:** Context parameter, url-encoded string context parameter for ArchiveProvider constructor
* **Returns:** Archive configuration consisting of column information, orderby information and entities


