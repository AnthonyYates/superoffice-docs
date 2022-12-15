---
uid: crmscriptagent-savetriggerscriptbyuniqueid
title: CRMScriptAgent.SaveTriggerScriptByUniqueId event method
description: Scripting events called on the SaveTriggerScriptByUniqueId method on the CRMScriptAgent service agent.
so.generated: true
keywords:
  - "netserver"
  - "scripting"
so.date: 11.29.2022
so.topic: reference
so.envir:
  - "onsite"
---
# CRMScriptAgent.SaveTriggerScriptByUniqueId

Scripting events called on the <see cref='M:SuperOffice.CRM.Services.ICRMScriptAgent.SaveTriggerScriptByUniqueId'>SaveTriggerScriptByUniqueId</see> method on the <see cref='ICRMScriptAgent'>ICRMScriptAgent</see>  service agent.

## BeforeSaveTriggerScriptByUniqueId
```cs
    static void BeforeSaveTriggerScriptByUniqueId(
       String  triggerScriptUniqueId,
       TriggerScriptEntity  entity,
       ref object  eventState
      );
```
Executes before the service method is invoked.
The return value is not calculated yet, so this method can't affect the result.
It can store some state in the *eventState* parameter, that is passed to the **After** and **AfterAsync** methods in this service call.
Event state is not preserved between different service calls. It is set to null at the start of each service call.
## AfterSaveTriggerScriptByUniqueId
```cs
    static void AfterSaveTriggerScriptByUniqueId(
       String  triggerScriptUniqueId,
       TriggerScriptEntity  entity,
       ref TriggerScriptEntity  returnValue,
       ref object  eventState
      );
```
Executes after the service method has been invoked. The service waits for this method to complete before returning the result to the caller.
The return value has been set. The script may modify the return value by altering the **returnValue** parameter.
Any state you set in the **Before** method is passed in through the *eventState* parameter.
## AfterSaveTriggerScriptByUniqueIdAsync
```cs
    static void AfterSaveTriggerScriptByUniqueIdAsync(
       String  triggerScriptUniqueId,
       TriggerScriptEntity  entity,
       ref TriggerScriptEntity  returnValue,
       ref object  eventState
      );
```
Executes after the service method is invoked, without waiting for the call to return.
The service call is not blocked waiting for this method to complete.
The async event handler cannot modify the return value of the service call.
Any state you set in the **Before** method is passed in through the *eventState* parameter.
