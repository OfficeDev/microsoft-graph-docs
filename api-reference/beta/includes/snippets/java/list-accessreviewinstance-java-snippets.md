---
description: "Automatically generated file. DO NOT MODIFY"
---

```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AccessReviewInstanceCollectionPage instances = graphClient.identityGovernance().accessReviews().definitions("60860cdd-fb4d-4054-91ba-f75e04f34444").instances()
	.buildRequest()
	.skip(0)
	.top(100)
	.get();

```