---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var lists = await graphClient.Me.Tasks.Lists
	.Request()
	.GetAsync();

```