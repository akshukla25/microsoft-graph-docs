---
title: "riskyServicePrincipal: confirmCompromised"
description: "Confirm one or more riskyServicePrincipal objects as compromised."
author: "ebasseri"
ms.localizationpriority: medium
ms.prod: "identity-and-sign-in"
doc_type: apiPageType
---

# riskyServicePrincipal: confirmCompromised
Namespace: microsoft.graph

Confirm one or more [riskyServicePrincipal](../resources/riskyserviceprincipal.md) objects as compromised. This action sets the targeted service principal account's risk level to `high`.

>**Note:** Using the riskyServicePrincipal API requires an Entra Workload Identity Premium license.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

|Permission type|Permissions (from least to most privileged)|
|:---|:---|
|Delegated (work or school account)|IdentityRiskyServicePrincipal.ReadWrite.All|
|Delegated (personal Microsoft account)|Not supported.|
|Application|IdentityRiskyServicePrincipal.ReadWrite.All|

## HTTP request

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /identityProtection/riskyServicePrincipals/confirmCompromised
```

## Request headers
|Name|Description|
|:---|:---|
|Authorization|Bearer {token}. Required.|

## Request body
In the request body, specify the collection of ids of the risky service principals in a **servicePrincipalIds** property. 

## Response

If successful, this action returns a `204 No Content` response code. It does not return anything in the response body.

## Example

### Request

<!-- {
  "blockType": "request",
  "name": "riskyserviceprincipal_confirmcompromised"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/identityProtection/riskyServicePrincipals/confirmCompromised
Content-Type: application/json

{
  "servicePrincipalIds": [
    "9089a539-a539-9089-39a5-899039a58990"
  ]
}
```

### Response
The following is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

