---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
	DisplayName = "New display name"
}

Update-MgApplication -ApplicationId $applicationId -BodyParameter $params

```