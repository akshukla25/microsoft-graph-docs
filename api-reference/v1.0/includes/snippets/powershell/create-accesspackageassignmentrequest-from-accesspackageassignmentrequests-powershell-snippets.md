---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	RequestType = "userAdd"
	Assignment = @{
		AccessPackageId = "d7be3253-b9c6-4fab-adef-30d30de8da2b"
	}
}

New-MgEntitlementManagementAssignmentRequest -BodyParameter $params

```