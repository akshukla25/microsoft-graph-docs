---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
	.Request()
	.DeleteAsync();

```