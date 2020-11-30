---
title: "Create policy"
description: "Create a new policy object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: apiPageType
---

# Create policy
Namespace: microsoft.graph

Create a new policy object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Provide applicable permissions.**|
|Delegated (personal Microsoft account)|**TODO: Provide applicable permissions.**|
|Application|**TODO: Provide applicable permissions.**|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /legacy/policies
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
In the request body, supply a JSON representation of the [policy](../resources/policy.md) object.

The following table shows the properties that are required when you create the [policy](../resources/policy.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|deletedDateTime|DateTimeOffset|**TODO: Add Description** Inherited from [directoryObject](../resources/directoryobject.md)|
|alternativeIdentifier|String|**TODO: Add Description**|
|definition|String collection|**TODO: Add Description**|
|displayName|String|**TODO: Add Description**|
|isOrganizationDefault|Boolean|**TODO: Add Description**|
|keyCredentials|[keyCredential](../resources/keycredential.md) collection|**TODO: Add Description**|
|type|String|**TODO: Add Description**|



## Response

If successful, this method returns a `201 Created` response code and a [policy](../resources/policy.md) object in the response body.

## Examples

### Request
<!-- {
  "blockType": "request",
  "name": "create_policy_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/legacy/policies
Content-Type: application/json
Content-length: 366

{
  "@odata.type": "#Microsoft.DirectoryServices.policy",
  "deletedDateTime": "String (timestamp)",
  "alternativeIdentifier": "String",
  "definition": [
    "String"
  ],
  "displayName": "String",
  "isOrganizationDefault": "Boolean",
  "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredential"
    }
  ],
  "type": "String"
}
```


### Response
**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Microsoft.DirectoryServices.policy"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.type": "#Microsoft.DirectoryServices.policy",
  "id": "9fb5d030-d030-9fb5-30d0-b59f30d0b59f",
  "deletedDateTime": "String (timestamp)",
  "alternativeIdentifier": "String",
  "definition": [
    "String"
  ],
  "displayName": "String",
  "isOrganizationDefault": "Boolean",
  "keyCredentials": [
    {
      "@odata.type": "microsoft.graph.keyCredential"
    }
  ],
  "type": "String"
}
```
