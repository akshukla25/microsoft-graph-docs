---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let authenticationMethodModeDetail = await client.api('/identity/conditionalAccess/authenticationStrengths/authenticationMethodModes/windowsHelloForBusiness')
	.version('beta')
	.get();

```