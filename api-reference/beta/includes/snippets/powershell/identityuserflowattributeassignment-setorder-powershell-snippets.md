---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
	NewAssignmentOrder = @{
		Order = @(
			"City"
			"extension_GUID_ShoeSize"
		)
	}
}

Set-MgIdentityB2CUserFlowUserAttributeAssignmentOrder -B2cIdentityUserFlowId $b2cIdentityUserFlowId -BodyParameter $params

```