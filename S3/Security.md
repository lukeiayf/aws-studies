• User-Based
	• **IAM Policies** – which API calls should be allowed for a specific user from IAM
• Resource-Based
	• **Bucket Policies** – bucket wide rules from the S3 console - allows cross account
	• **Object Access Control List (ACL)** – finer grain (can be disabled)
	• **Bucket Access Control List (ACL)** – less common (can be disabled)
• Note: an IAM principal can access an S3 object if
	• The user IAM permissions ALLOW it OR the resource policy ALLOWS it
	• AND there’s no explicit DENY
• Encryption: encrypt objects in Amazon S3 using encryption keys