---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
	.Request()
	.Select("ext55gb1l09_msLearnCourses")
	.GetAsync();

```