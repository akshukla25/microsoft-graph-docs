---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.DeviceManagement.Actions

$params = @{
	Filter = "CloudPcId eq '40f9315c-5b63-4126-9f89-b7dcb14fffff' and SignInDateTime gt datetime'2022-09-09T01:22:51.849Z'"
	Select = @(
		"SignInDateTime"
		"SignOutDateTime"
		"UsageInHour"
		"RoundTripTimeInMsP50"
		"AvailableBandwidthInMBpsP50"
		"RemoteSignInTimeInSec"
	)
	Top = 25
	Skip = 0
}

Get-MgDeviceManagementVirtualEndpointReportRemoteConnectionHistoricalReport -BodyParameter $params

```