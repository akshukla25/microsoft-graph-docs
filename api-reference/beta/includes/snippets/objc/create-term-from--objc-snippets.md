---
description: "Automatically generated file. DO NOT MODIFY"
---

```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/termStore/sets/{setId}/children"]]];
[urlRequest setHTTPMethod:@"POST"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphTermStoreTerm *term = [[MSGraphTermStoreTerm alloc] init];
NSMutableArray *labelsList = [[NSMutableArray alloc] init];
MSGraphTermStoreLocalizedLabel *labels = [[MSGraphTermStoreLocalizedLabel alloc] init];
[labels setLanguageTag:@"en-US"];
[labels setName:@"Car"];
[labels setIsDefault: true];
[labelsList addObject: labels];
[term setLabels:labelsList];

NSError *error;
NSData *termData = [term getSerializedDataWithError:&error];
[urlRequest setHTTPBody:termData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
	completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

		//Request Completed

}];

[meDataTask execute];

```