---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
	DisplayName = "My application"
};

await graphClient.Applications
	.Request()
	.AddAsync(application);

```