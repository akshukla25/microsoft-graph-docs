---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
	Reason = "none"
}

Invoke-MgRejectCommunicationCall -CallId $callId -BodyParameter $params

```