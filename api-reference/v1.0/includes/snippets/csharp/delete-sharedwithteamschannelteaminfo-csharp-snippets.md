---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].SharedWithTeams["{sharedWithChannelTeamInfo-id}"]
	.Request()
	.DeleteAsync();

```