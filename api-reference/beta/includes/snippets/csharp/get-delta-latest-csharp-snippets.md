---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
	new QueryOption("token", "latest")
};

var delta = await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
	.Delta()
	.Request( queryOptions )
	.GetAsync();

```