• Must enable Versioning in source and destination buckets
**• Cross-Region Replication (CRR)**
**• Same-Region Replication (SRR)**
• Buckets can be in different AWS accounts
• Copying is asynchronous
• Must give proper IAM permissions to S3
• Use cases:
	• CRR – compliance, lower latency access, replication across
	accounts
	• SRR – log aggregation, live replication between production and test
	accounts