---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	SelfServiceSignUp = @{
		IsEnabled = $true
	}
}

Update-MgPolicyAuthenticationFlowPolicy -BodyParameter $params

```