---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = true;

graphClient.servicePrincipals("{id}")
	.getMemberGroups(securityEnabledOnly)
	.buildRequest()
	.post();

```