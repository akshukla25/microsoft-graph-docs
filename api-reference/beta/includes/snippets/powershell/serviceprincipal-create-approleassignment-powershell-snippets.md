---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
	PrincipalId = "9028d19c-26a9-4809-8e3f-20ff73e2d75e"
	ResourceId = "8fce32da-1246-437b-99cd-76d1d4677bd5"
	AppRoleId = "498476ce-e0fe-48b0-b801-37ba7e2685c6"
}

New-MgServicePrincipalAppRoleAssignment -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```