---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestConfiguration = new TemplatesRequestBuilderGetRequestConfiguration();

$queryParameters = new TemplatesRequestBuilderGetQueryParameters();
$queryParameters->select = ["name","description","id","scenarios"];
$queryParameters->filter = "scenarios has 'secureFoundation'";

$requestConfiguration->queryParameters = $queryParameters;


$requestResult = $graphServiceClient->identity()->conditionalAccess()->templates()->get($requestConfiguration);


```