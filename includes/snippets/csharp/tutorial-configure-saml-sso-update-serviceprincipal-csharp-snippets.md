---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var servicePrincipal = new ServicePrincipal
{
	PreferredSingleSignOnMode = "saml"
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"]
	.Request()
	.UpdateAsync(servicePrincipal);

```