---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
	RequestType = "AdminRemove"
	AccessPackageAssignment = @{
		Id = "a6bb6942-3ae1-4259-9908-0133aaee9377"
	}
}

New-MgEntitlementManagementAccessPackageAssignmentRequest -BodyParameter $params

```