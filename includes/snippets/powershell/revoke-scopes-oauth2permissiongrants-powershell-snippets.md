---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	Scope = "User.Read.All"
}

Update-MgOauth2PermissionGrant -OAuth2PermissionGrantId $oAuth2PermissionGrantId -BodyParameter $params

```