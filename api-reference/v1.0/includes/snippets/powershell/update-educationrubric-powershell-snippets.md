---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Education

$params = @{
	DisplayName = "Example Credit Rubric after display name patch"
}

Update-MgEducationMeRubric -EducationRubricId $educationRubricId -BodyParameter $params

```