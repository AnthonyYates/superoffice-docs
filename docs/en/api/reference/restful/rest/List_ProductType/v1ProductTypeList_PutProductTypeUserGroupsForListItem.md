---
title: PUT List/ProductType/Items/{id}/UserGroups
uid: v1ProductTypeList_PutProductTypeUserGroupsForListItem
---

# PUT List/ProductType/Items/{id}/UserGroups

```http
PUT /api/v1/List/ProductType/Items/{itemId}/UserGroups
```

Saves user groups visible for the ProductType list's item.


Calls the List agent service SaveHeadingsForListItemFromListDefinition.





| Path Part | Type | Description |
|-----------|------|-------------|
| itemId | int32 | The ID of the item to save. **Required** |



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

## Request Body: entities  

The headings to be saved. 

| Property Name | Type |  Description |
|----------------|------|--------------|
| Id | int32 | The Id of the ListItem |
| Name | string | The name of the ListItem |
| ToolTip | string | The tooltip of the ListItem |
| Deleted | bool | The deleted status of the ListItem |
| Rank | int32 | The rank of the ListItem |
| Type | string | The type of the ListItem. Custom field. |
| ColorBlock | int32 | The color indicator of the ListItem color block |
| IconHint | string | The Icon hint of the ListItem. Custom field. |
| Selected | bool | True if the ListItem is selected |
| LastChanged | date-time | Time of last change. |
| ChildItems | array | The child items of the SelectableMDOListItem |
| ExtraInfo | string | Extra information added to the ListItem. Could be information such as sort order etc or other meta data. Custom field. |
| StyleHint | string | Style hint indicating, information such as background color etc. Custom field. |
| Hidden | bool | True if the ListItem is hidden |
| FullName | string | The name of the ListItem in its context |


## Response: array

OK

| Response | Description |
|----------------|-------------|
| 200 | OK |

Response body: array

| Property Name | Type |  Description |
|----------------|------|--------------|
| Id | int32 | The Id of the ListItem |
| Name | string | The name of the ListItem |
| ToolTip | string | The tooltip of the ListItem |
| Deleted | bool | The deleted status of the ListItem |
| Rank | int32 | The rank of the ListItem |
| Type | string | The type of the ListItem. Custom field. |
| ColorBlock | int32 | The color indicator of the ListItem color block |
| IconHint | string | The Icon hint of the ListItem. Custom field. |
| Selected | bool | True if the ListItem is selected |
| LastChanged | date-time | Time of last change. |
| ChildItems | array | The child items of the SelectableMDOListItem |
| ExtraInfo | string | Extra information added to the ListItem. Could be information such as sort order etc or other meta data. Custom field. |
| StyleHint | string | Style hint indicating, information such as background color etc. Custom field. |
| Hidden | bool | True if the ListItem is hidden |
| FullName | string | The name of the ListItem in its context |
| TableRight |  |  |
| FieldProperties | object |  |

## Sample request

```http!
PUT /api/v1/List/ProductType/Items/{itemId}/UserGroups
Authorization: Basic dGplMDpUamUw
Accept: application/json; charset=utf-8
Accept-Language: sv
Content-Type: application/json; charset=utf-8

[
  {
    "Id": 272,
    "Name": "Hills-Kohler",
    "ToolTip": "Fugit deserunt occaecati veniam.",
    "Deleted": false,
    "Rank": 435,
    "Type": "quo",
    "ColorBlock": 198,
    "IconHint": "harum",
    "Selected": true,
    "LastChanged": "2008-08-03T02:49:52.3753234+02:00",
    "ChildItems": [
      {
        "Id": 973,
        "Name": "Torphy, Prosacco and Kovacek",
        "ToolTip": "Soluta et minus doloribus veritatis.",
        "Deleted": false,
        "Rank": 934,
        "Type": "rem",
        "ColorBlock": 335,
        "IconHint": "error",
        "Selected": true,
        "LastChanged": "2000-05-27T02:49:52.3753234+02:00",
        "ChildItems": [
          {},
          {}
        ],
        "ExtraInfo": "voluptatibus",
        "StyleHint": "aliquam",
        "Hidden": false,
        "FullName": "Ignatius Mann PhD"
      }
    ],
    "ExtraInfo": "esse",
    "StyleHint": "laudantium",
    "Hidden": false,
    "FullName": "Mose Murazik Jr."
  }
]
```

## Sample response

```http_
HTTP/1.1 200 OK
Content-Type: application/json; charset=utf-8

[
  {
    "Id": 670,
    "Name": "Metz-Lindgren",
    "ToolTip": "In quasi sit.",
    "Deleted": false,
    "Rank": 626,
    "Type": "pariatur",
    "ColorBlock": 27,
    "IconHint": "eum",
    "Selected": false,
    "LastChanged": "2003-03-02T02:49:52.3753234+01:00",
    "ChildItems": [
      {
        "Id": 572,
        "Name": "Hodkiewicz-Spinka",
        "ToolTip": "Dolorem molestiae non aut est sunt eos esse.",
        "Deleted": false,
        "Rank": 288,
        "Type": "ut",
        "ColorBlock": 86,
        "IconHint": "harum",
        "Selected": true,
        "LastChanged": "1997-05-29T02:49:52.3753234+02:00",
        "ChildItems": [
          {},
          {}
        ],
        "ExtraInfo": "optio",
        "StyleHint": "nesciunt",
        "Hidden": false,
        "FullName": "Prof. Franco Harris",
        "TableRight": null,
        "FieldProperties": {
          "fieldName": {
            "FieldRight": null,
            "FieldType": "System.Int32",
            "FieldLength": 927
          }
        }
      }
    ],
    "ExtraInfo": "et",
    "StyleHint": "nostrum",
    "Hidden": false,
    "FullName": "Winifred Mohr",
    "TableRight": null,
    "FieldProperties": {
      "fieldName": {
        "FieldRight": null,
        "FieldType": "System.String",
        "FieldLength": 267
      }
    }
  }
]
```