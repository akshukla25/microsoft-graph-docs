---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentScheduleRequests = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
	.Request()
	.Expand("roleDefinitionId")
	.Select("principalId,action,roleDefinitionId")
	.GetAsync();

```