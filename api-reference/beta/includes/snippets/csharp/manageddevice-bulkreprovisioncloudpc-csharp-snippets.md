---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var managedDeviceIds = new List<String>()
{
	"30d0e128-de93-41dc-89ec-33d84bb662a0",
	"7c82a3e3-9459-44e4-94d9-b92f93bf78dd"
};

await graphClient.DeviceManagement.ManagedDevices
	.BulkReprovisionCloudPc(managedDeviceIds)
	.Request()
	.PostAsync();

```