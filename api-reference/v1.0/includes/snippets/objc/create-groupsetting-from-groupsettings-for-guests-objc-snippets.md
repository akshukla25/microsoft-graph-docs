---
description: "Automatically generated file. DO NOT MODIFY"
---

```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/v1.0/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/groups/055a5d18-a3a9-4338-b9c5-de92559b7ebf/settings"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphGroupSetting *groupSetting = [[MSGraphGroupSetting alloc] init];
[groupSetting setTemplateId:@"08d542b9-071f-4e16-94b0-74abb372e3d9"];
NSMutableArray *valuesList = [[NSMutableArray alloc] init];
MSGraphSettingValue *values = [[MSGraphSettingValue alloc] init];
[values setName:@"AllowToAddGuests"];
[values setValue:@"false"];
[valuesList addObject: values];
[groupSetting setValues:valuesList];

NSError *error;
NSData *groupSettingData = [groupSetting getSerializedDataWithError:&error];
[urlRequest setHTTPBody:groupSettingData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
	completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

		//Request Completed

}];

[meDataTask execute];

```