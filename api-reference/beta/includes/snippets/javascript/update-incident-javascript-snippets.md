---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

const incident = {
    classification: 'TruePositive',
    determination: 'MultiStagedAttack',
    tags: [
      'Demo'
    ]
};

await client.api('/security/incidents/2972395')
	.version('beta')
	.update(incident);

```