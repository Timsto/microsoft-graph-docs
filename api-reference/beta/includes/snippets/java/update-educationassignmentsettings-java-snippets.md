---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

EducationAssignmentSettings educationAssignmentSettings = new EducationAssignmentSettings();
educationAssignmentSettings.submissionAnimationDisabled = true;

graphClient.education().classes("{id}").assignmentSettings()
	.buildRequest()
	.patch(educationAssignmentSettings);

```