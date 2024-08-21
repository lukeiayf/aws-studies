• JSON based policies
	• Resources: buckets and objects
	• Effect: Allow / Deny
	• Actions: Set of API to Allow or Deny
	• Principal: The account or user to apply the policy to
• Use S3 bucket for policy to:
	• Grant public access to the bucket
	• Force objects to be encrypted at upload
	• Grant access to another account (Cross Account)

YOU CAN USE THE AWS POLICY GENERATOR TO CREATE POLICIES: https://awspolicygen.s3.amazonaws.com/policygen.html

- Before setting a bucket public you must unblock the settings on its permissions;

Example of a policy that makes the bucket public for reading
![[Public Bucket Policy example.png]]