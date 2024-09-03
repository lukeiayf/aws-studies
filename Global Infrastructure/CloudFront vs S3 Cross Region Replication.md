
• CloudFront:
	• Global Edge network
	• Files are cached for a TTL (maybe a day)
	• Great for static content that must be available everywhere

• S3 Cross Region Replication:
	• Must be setup for each region you want replication to happen
	• Files are updated in near real-time
	• Read only
	• Great for dynamic content that needs to be available at low-latency in few regions