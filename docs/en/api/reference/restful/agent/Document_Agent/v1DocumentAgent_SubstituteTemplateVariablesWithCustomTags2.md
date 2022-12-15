---
title: POST Agents/Document/SubstituteTemplateVariablesWithCustomTags2
uid: v1DocumentAgent_SubstituteTemplateVariablesWithCustomTags2
---

# POST Agents/Document/SubstituteTemplateVariablesWithCustomTags2

```http
POST /api/v1/Agents/Document/SubstituteTemplateVariablesWithCustomTags2
```

Parse the source string, and replace any template variable tags with their values, based on the ID's given in the other parameters.


&lt;p/&gt;This method also takes a pair of arrays specifying custom tags and their values; these tags will be available during substitution in addition to all the existing tags. Custom values will override values otherwise set.






## Query String Parameters

| Parameter Name | Type |  Description |
|----------------|------|--------------|
| $select | string |  Optional comma separated list of properties to include in the result. Other fields are then nulled out to reduce payload size: "Name,department,category". Default = show all fields. |

```http
POST /api/v1/Agents/Document/SubstituteTemplateVariablesWithCustomTags2?$select=name,department,category/id
```


## Request Headers

| Parameter Name | Description |
|----------------|-------------|
| Authorization  | Supports 'Basic', 'SoTicket' and 'Bearer' schemes, depending on installation type. |
| X-XSRF-TOKEN   | If not using Authorization header, you must provide XSRF value from cookie or hidden input field |
| Content-Type | Content-type of the request body: `application/json`, `text/json`, `application/xml`, `text/xml`, `application/x-www-form-urlencoded`, `application/json-patch+json`, `application/merge-patch+json` |
| Accept         | Content-type(s) you would like the response in: `application/json`, `text/json`, `application/xml`, `text/xml`, `application/json-patch+json`, `application/merge-patch+json` |
| Accept-Language | Convert string references and multi-language values into a specified language (iso2) code. |
| SO-Language | Convert string references and multi-language values into a specified language (iso2) code. Overrides Accept-Language value. |
| SO-Culture | Number, date formatting in a specified culture (iso2 language) code. Partially overrides SO-Language/Accept-Language value. Ignored if no Language set. |
| SO-TimeZone | Specify the timezone code that you would like date/time responses converted to. |
| SO-AppToken | The application token that identifies the partner app. Used when calling Online WebAPI from a server. |

## Request Body: request  

Source, GeneratorEncoding, CustomTags, ContactId, PersonId, AppointmentId, DocumentId, SaleId, SelectionId, ProjectId, CultureName 

| Property Name | Type |  Description |
|----------------|------|--------------|
| Source | string |  |
| GeneratorEncoding | string |  |
| CustomTags | object |  |
| ContactId | int32 |  |
| PersonId | int32 |  |
| AppointmentId | int32 |  |
| DocumentId | int32 |  |
| SaleId | int32 |  |
| SelectionId | int32 |  |
| ProjectId | int32 |  |
| CultureName | string |  |


## Response: string

OK

| Response | Description |
|----------------|-------------|
| 200 | OK |

Response body: string


## Sample request

```http!
POST /api/v1/Agents/Document/SubstituteTemplateVariablesWithCustomTags2
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: en
Content-Type: application/json; charset=utf-8

{
  "Source": "ratione",
  "GeneratorEncoding": "Html",
  "CustomTags": {
    "CustomTags1": "sint",
    "CustomTags2": "omnis"
  },
  "ContactId": 137,
  "PersonId": 749,
  "AppointmentId": 770,
  "DocumentId": 599,
  "SaleId": 321,
  "SelectionId": 465,
  "ProjectId": 796,
  "CultureName": "sv"
}
```

## Sample response

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

"ex"
```