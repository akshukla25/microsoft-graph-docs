---
title: "Update partnerInformation"
description: "Update the properties of a partnerInformation object."
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
ms.localizationpriority: medium
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://aka.ms/msgo?pagePath=Document-APIs/Guidelines/Metadata)**"
doc_type: apiPageType
---

# Update partnerInformation
Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Update the properties of a [partnerInformation](../resources/partnerinformation.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
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
PATCH /organization/{organizationId}/partnerInformation
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|
|Content-Type|application/json. Required.|

## Request body
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]


**TODO: Remove properties that don't apply**
|Property|Type|Description|
|:---|:---|:---|
|partnerTenantId|String|**TODO: Add Description** Required.|
|companyType|partnerTenantType|**TODO: Add Description**. The possible values are: `microsoftSupport`, `syndicatePartner`, `breadthPartner`, `breadthPartnerDelegatedAdmin`, `resellerPartnerDelegatedAdmin`, `valueAddedResellerPartnerDelegatedAdmin`, `unknownFutureValue`. Optional.|
|companyName|String|**TODO: Add Description** Optional.|
|supportTelephones|String collection|**TODO: Add Description** Optional.|
|supportEmails|String collection|**TODO: Add Description** Optional.|
|commerceUrl|String|**TODO: Add Description** Optional.|
|supportUrl|String|**TODO: Add Description** Optional.|
|helpUrl|String|**TODO: Add Description** Optional.|



## Response

If successful, this method returns a `200 OK` response code and an updated [partnerInformation](../resources/partnerinformation.md) object in the response body.

## Examples

### Request
The following is an example of a request.
<!-- {
  "blockType": "request",
  "name": "update_partnerinformation"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/partnerInformation
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.partnerInformation",
  "partnerTenantId": "d8b48888-ac07-af9b-fdbd-9862949545dd",
  "companyType": "String",
  "companyName": "String",
  "supportTelephones": [
    "String"
  ],
  "supportEmails": [
    "String"
  ],
  "commerceUrl": "String",
  "supportUrl": "String",
  "helpUrl": "String"
}
```


### Response
The following is an example of the response
>**Note:** The response object shown here might be shortened for readability.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.partnerInformation",
  "partnerTenantId": "d8b48888-ac07-af9b-fdbd-9862949545dd",
  "companyType": "String",
  "companyName": "String",
  "supportTelephones": [
    "String"
  ],
  "supportEmails": [
    "String"
  ],
  "commerceUrl": "String",
  "supportUrl": "String",
  "helpUrl": "String"
}
```

