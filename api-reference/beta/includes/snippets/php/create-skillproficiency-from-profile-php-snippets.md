---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new SkillProficiency();
$requestBody->setCategories(['Professional', ]);

$requestBody->setAllowedAudiences(new AllowedAudiences('organization'));

$requestBody->setDisplayName('API Design');

$requestBody->setProficiency(new SkillProficiencyLevel('generalprofessional'));

$requestBody->setCollaborationTags(['ableToMentor', ]);



$requestResult = $graphServiceClient->me()->profile()->skills()->post($requestBody);


```