---
description: "Automatically generated file. DO NOT MODIFY"
---

```javascript

const options = {
	authProvider,
};

const client = Client.init(options);

let provisioning = await client.api('/auditLogs/provisioning')
	.version('beta')
	.get();

```