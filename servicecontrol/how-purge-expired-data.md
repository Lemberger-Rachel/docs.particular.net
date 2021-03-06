---
title: Automatic Expiration of Data
summary: Configuring ServiceControl's data retention policy
related:
 - nservicebus/recoverability
 - nservicebus/operations/auditing
reviewed: 2018-10-05
---

ServiceControl stores audit and error data. Any audit and error data that is older than the specified thresholds is deleted from the embedded RavenDB. The expiration thresholds for both faulted and audited messages must be set during installation. These values can be modified later by launching ServiceControl Management and editing the configuration settings for the instance.

Note: The expiration process curates only the data in the embedded RavenDB. Audit and error forwarding queues are not curated or managed by ServiceControl. To turn these settings off, launch ServiceControl Management and edit the configuration settings for the instance.