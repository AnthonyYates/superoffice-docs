---
title: NSPreference[] GetPreferencesWithDisplayValues(NSPreferenceSpec[] specifications)
path: /EJScript/Classes/NSPreferenceAgent/Member functions/NSPreference[] GetPreferencesWithDisplayValues(NSPreferenceSpec[] p_0)
intellisense: 1
classref: 1
sortOrder: 5302
keywords: GetPreferencesWithDisplayValues(NSPreferenceSpec[])
---

Get one or more preferences based on a set of specifications\<br/>The PrefDisplayValue and PrefDisplaytooltip are populated, at some additional processing cost.


* **specifications:** Array of preference specifications. The key value may be * (asterisk), which means 'all keys within section'. 


    	/// 
    	/// Note that the semantics of this are more strictly 'all keys actually set at any accessible level for this associate'; you will NOT get entries for preferences that might exist, but have no set value anywhere.
    	/// 
    	/// You can also have askerisk as the section name. In that case the specification array must contain exactly one entry and the key must also be asterisk. This will return all known preferences in all sections for your associate. It might be a lot, tests have shown that a heavily used database can accumulate up to 500 preferences on a single associate. If the Sentry table/field right preferences have been used, the number could be a lot greater!



* **Returns:** Array of preference values for your given `specification(s)`. More strictly:


    	/// 'all keys actually set at any accessible level for this associate'; you will NOT get entries for preferences that might exist, but have no set value anywhere.<br/>The PrefDisplayValue and PrefDisplaytooltip are populated, at some additional processing cost.


