---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let learningContent = await client.api('/employeeExperience/learningProviders/13727311-e7bb-470d-8b20-6a23d9030d70/learningContents(externalId='LP4471')')
	.version('beta')
	.get();

```