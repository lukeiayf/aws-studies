**• Amazon S3 Standard - General Purpose**
	• 99.99% Availability
	• Used for frequently accessed data
	• Low latency and high throughput
	• Sustain 2 concurrent facility failures
	• Use Cases: Big Data analytics, mobile & gaming applications,content distribution…

For data that is less frequently accessed, but requires rapid access when needed, it is also cheaper than standard S3

• **Amazon S3 Standard-Infrequent Access (IA)**
	• 99.9% Availability
	• Use cases: Disaster Recovery, backups
• **Amazon S3 One Zone-Infrequent Access**
	• High durability (99.999999999%) in a single AZ; data lost when AZ is destroyed
	• 99.5% Availability
	• Use Cases: Storing secondary backup copies of on-premise data, or data you can recreate

Low-cost object storage meant for archiving / backup

• A**mazon S3 Glacier Instant Retrieval**
	• Millisecond retrieval, great for data accessed once a quarter
	• Minimum storage duration of 90 days
• **Amazon S3 Glacier Flexible Retrieval**
	• Expedited (1 to 5 minutes), Standard (3 to 5 hours), Bulk (5 to 12 hours) – free
	• Minimum storage duration of 90 days
• **Amazon S3 Glacier Deep Archive**
	• Standard (12 hours), Bulk (48 hours)
	• Minimum storage duration of 180 days
• **Amazon S3 Intelligent Tiering**
	• Moves objects automatically between Access Tiers based on usage
	• There are no retrieval charges in S3 Intelligent-Tiering
• Amazon S3 Express One Zone

• Can move between classes manually or using S3 Lifecycle configurations