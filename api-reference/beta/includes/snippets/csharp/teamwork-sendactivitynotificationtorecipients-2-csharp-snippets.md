---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
	Source = TeamworkActivityTopicSource.Text,
	Value = "Deployment Approvals Channel",
	WebUrl = "https://teams.microsoft.com/l/message/19:448cfd2ac2a7490a9084a9ed14cttr78c@thread.skype/1605223780000?tenantId=c8b1bf45-3834-4ecf-971a-b4c755ee677d&groupId=d4c2a937-f097-435a-bc91-5c1683ca7245&parentMessageId=1605223771864&teamName=Approvals&channelName=Azure%20DevOps&createdTime=1605223780000"
};

var activityType = "deploymentApprovalRequired";

var previewText = new ItemBody
{
	Content = "New deployment requires your approval"
};

var templateParameters = new List<KeyValuePair>()
{
	new KeyValuePair
	{
		Name = "deploymentId",
		Value = "6788662"
	}
};

var recipients = new List<TeamworkNotificationRecipient>()
{
	new AadUserNotificationRecipient
	{
		UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
	},
	new AadUserNotificationRecipient
	{
		UserId = "ab88234e-0874-477c-9638-d144296ed04f"
	},
	new AadUserNotificationRecipient
	{
		UserId = "01c64f53-69aa-42c7-9b7f-9f75195d6bfc"
	}
};

await graphClient.Teamwork
	.SendActivityNotificationToRecipients(topic,activityType,null,previewText,null,templateParameters,recipients)
	.Request()
	.PostAsync();

```