---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OAuth2PermissionGrant oAuth2PermissionGrant = new OAuth2PermissionGrant();
oAuth2PermissionGrant.clientId = "b0d9b9e3-0ecf-4bfd-8dab-9273dd055a94";
oAuth2PermissionGrant.consentType = "AllPrincipal";
oAuth2PermissionGrant.resourceId = "7ea9e944-71ce-443d-811c-71e8047b557a";
oAuth2PermissionGrant.scope = "User.Read.All Group.Read.All";

graphClient.oauth2PermissionGrants()
	.buildRequest()
	.post(oAuth2PermissionGrant);

```