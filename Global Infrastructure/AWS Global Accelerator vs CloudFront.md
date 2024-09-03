• They both use the AWS global network and its edge locations around the world
• Both services integrate with AWS Shield for DDoS protection.

• CloudFront – Content Delivery Network
	• Improves performance for your cacheable content (such as images and videos)
	• Content is served at the edge
	
• Global Accelerator
	• No caching, proxying packets at the edge to applications running in one or more AWS Regions.
	• Improves performance for a wide range of applications over TCP or UDP
	• Good for HTTP use cases that require static IP addresses
	• Good for HTTP use cases that required deterministic, fast regional failover