---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	ServicePrincipalIds = @(
		"9089a539-a539-9089-39a5-899039a58990"
	)
}

Invoke-MgDismissRiskyServicePrincipal -BodyParameter $params

```