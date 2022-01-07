---
uid: ISaintAgent-SetRankOnStatusMonitors
title: ISaintAgent.SetRankOnStatusMonitors event method
description: Scripting events called on the SetRankOnStatusMonitors method on the ISaintAgent service agent.
so.generated: true
keywords:
  - "netserver"
  - "scripting"
so.date: 03.19.2021
so.topic: reference
so.envir:
  - "onsite"
---
# ISaintAgent.SetRankOnStatusMonitors

Scripting events called on the <see cref='M:SuperOffice.CRM.Services.ISaintAgent.SetRankOnStatusMonitors'>SetRankOnStatusMonitors</see> method on the <see cref='ISaintAgent'>ISaintAgent</see>  service agent.

## BeforeSetRankOnStatusMonitors
```cs
    static void BeforeSetRankOnStatusMonitors(
       String  type,
       Int32[]  itemsIds,
       ref object  eventState
      );
```
Executes before the service method is invoked.
It can store some state in the *eventState* parameter, that is passed to the **After** and **AfterAsync** methods in this service call.
Event state is not preserved between different service calls. It is set to null at the start of each service call.
## AfterSetRankOnStatusMonitors
```cs
    static void AfterSetRankOnStatusMonitors(
       String  type,
       Int32[]  itemsIds,
       ref object  eventState
      );
```
Executes after the service method has been invoked. The service waits for this method to complete before returning the result to the caller.
This service call has no return value, so there is no **returnValue** parameter
Any state you set in the **Before** method is passed in through the *eventState* parameter.
## AfterSetRankOnStatusMonitorsAsync
```cs
    static void AfterSetRankOnStatusMonitorsAsync(
       String  type,
       Int32[]  itemsIds,
       ref object  eventState
      );
```
Executes after the service method is invoked, without waiting for the call to return.
The service call is not blocked waiting for this method to complete.
Any state you set in the **Before** method is passed in through the *eventState* parameter.
