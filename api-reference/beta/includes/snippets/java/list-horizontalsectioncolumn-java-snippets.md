---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content columns = graphClient.sites("{sitesId}").pages("{sitePageId}").canvasLayout().horizontalSections().{horizontalSectionId}().columns()
	.buildRequest()
	.get();

```