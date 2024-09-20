• Anytime you hear “encryption” for an AWS service, it’s most likely KMS
• KMS = AWS manages the encryption keys for us

• Encryption Opt-in:
	• EBS volumes: encrypt volumes
	• S3 buckets: Server-side encryption of objects
	• Redshift database: encryption of data
	• RDS database: encryption of data
	• EFS drives: encryption of data

• Encryption Automatically enabled:
	• CloudTrail Logs
	• S3 Glacier
	• Storage Gateway

**Types of KMS Keys:**

• Customer Managed Key:
	• Create, manage and used by the customer, can enable or disable
	• Possibility of rotation policy (new key generated every year, old key preserved)
	• Possibility to bring-your-own-key

• AWS Managed Key:
	• Created, managed and used on the customer’s behalf by AWS
	• Used by AWS services (aws/s3, aws/ebs, aws/redshift)

• AWS Owned Key:
	• Collection of CMKs that an AWS service owns and manages to use in multiple accounts
	• AWS can use those to protect resources in your account (but you can’t view the keys)
	
• CloudHSM Keys (custom keystore):
	• Keys generated from your own CloudHSM hardware device
	• Cryptographic operations are performed within the CloudHSM cluster