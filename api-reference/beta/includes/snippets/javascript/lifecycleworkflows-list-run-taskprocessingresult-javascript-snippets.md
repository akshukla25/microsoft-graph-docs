---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let taskProcessingResults = await client.api('/IdentityGovernance/lifecycleWorkflows/workflows/14879e66-9ea9-48d0-804d-8fea672d0341/runs/72885f91-2cf0-44b1-b3ed-bd145af0192c/userProcessingResults/78b83505-6967-4168-a7ea-4921c0543ce9/taskProcessingResults')
	.version('beta')
	.get();

```