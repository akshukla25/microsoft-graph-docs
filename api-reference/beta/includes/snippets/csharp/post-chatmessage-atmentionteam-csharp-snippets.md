---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
	Body = new ItemBody
	{
		ContentType = BodyType.Html,
		Content = "<div><div><at id=\"0\">GraphTesting</at>&nbsp;Hello team</div></div>"
	},
	Mentions = new List<ChatMessageMention>()
	{
		new ChatMessageMention
		{
			Id = 0,
			MentionText = "GraphTesting",
			Mentioned = new ChatMessageMentionedIdentitySet
			{
				Conversation = new TeamworkConversationIdentity
				{
					Id = "68a3e365-f7d9-4a56-b499-24332a9cc572",
					DisplayName = "GraphTesting",
					ConversationIdentityType = TeamworkConversationIdentityType.Team
				}
			}
		}
	},
	Reactions = new List<ChatMessageReaction>()
	{
	},
	MessageHistory = new List<ChatMessageHistoryItem>()
	{
	}
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Messages
	.Request()
	.AddAsync(chatMessage);

```