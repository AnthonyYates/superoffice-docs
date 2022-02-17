---
title: POST Agents/List/SaveHeadingsFromName
id: v1ListAgent_SaveHeadingsFromName
---

# POST Agents/List/SaveHeadingsFromName

```http
POST /api/v1/Agents/List/SaveHeadingsFromName
```

Save headings for list resolved by the provided name.







## Query String Parameters

| Parameter Name | Type |  Description |
|----------------|------|--------------|
| $select | string |  Optional comma separated list of properties to include in the result. Other fields are then nulled out to reduce payload size: "Name,department,category". Default = show all fields. |

```http
POST /api/v1/Agents/List/SaveHeadingsFromName?$select=name,department,category/id
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

Name, Entities 

| Property Name | Type |  Description |
|----------------|------|--------------|
| Name | string |  |
| Entities | array |  |


## Response: array



| Response | Description |
|----------------|-------------|
| 200 | OK |

Response body: array

| Property Name | Type |  Description |
|----------------|------|--------------|
| HeadingId | int32 | Primary key |
| Name | string | The visible heading |
| Tooltip | string | Tooltip or other description |
| Deleted | bool | True if the heading is marked as deleted |
| Rank | int32 | Rank order |
| UdListDefinitionId | int32 | The id of the list which this heading belongs to |
| TableRight |  |  |
| FieldProperties | object |  |

## Sample Request

```http!
POST /api/v1/Agents/List/SaveHeadingsFromName
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: fr,de,ru,zh
Content-Type: application/json; charset=utf-8

{
  "Name": "Spencer, Brekke and Herzog",
  "Entities": [
    {
      "HeadingId": 487,
      "Name": "Gibson Group",
      "Tooltip": "culpa",
      "Deleted": false,
      "Rank": 109,
      "UdListDefinitionId": 279
    },
    {
      "HeadingId": 487,
      "Name": "Gibson Group",
      "Tooltip": "culpa",
      "Deleted": false,
      "Rank": 109,
      "UdListDefinitionId": 279
    }
  ]
}
```

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

[
  {
    "HeadingId": 605,
    "Name": "Heathcote-Cummings",
    "Tooltip": "doloremque",
    "Deleted": false,
    "Rank": 201,
    "UdListDefinitionId": 269,
    "TableRight": {
      "Mask": "Delete",
      "Reason": ""
    },
    "FieldProperties": {
      "fieldName": {
        "FieldRight": {
          "Mask": "FULL",
          "Reason": ""
        },
        "FieldType": "System.String",
        "FieldLength": 66
      }
    }
  }
]
```