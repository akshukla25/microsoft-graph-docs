---
title: "longRunningOperation resource type"
description: "The status of a long-running operation."
ms.localizationpriority: medium
author: "zhvolosh"
ms.prod: teamwork
doc_type: resourcePageType
---

# longRunningOperation resource type

Namespace: microsoft.graph

The status of a long-running operation.

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|The start time of the operation.|
|id|String|The unique identifier of the operation |
|lastActionDateTime|DateTimeOffset|The time of the last action in the operation.|
|resourceLocation|String| URI of the resource that the operation is performed on. |
|status|longRunningOperationStatus|The status of the operation. The possible values are: `notStarted`, `running`, `succeeded`, `failed`, `unknownFutureValue`.|
|statusDetail|String|Details about the status of the operation.|


## JSON representation

Here is a JSON representation of the resource.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.longRunningOperation",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.longRunningOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "resourceLocation": "String",
  "status": "String",
  "statusDetail": "String"
}
```

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

