---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = await graphClient.Users["{user-id}"].Extensions["{extension-id}"]
	.Request()
	.GetAsync();

```