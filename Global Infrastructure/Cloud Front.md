• Content Delivery Network (CDN)
**• Improves read performance, content is cached at the edge**
• Improves users experience
• 216 Point of Presence globally (edge locations)
• DDoS protection (because worldwide), integration with Shield,
AWS Web Application Firewall
- You can use AWS WAF(Web Application FIrewall) web access control lists (web ACLs) to help minimize the effects of a distributed denial of service (DDoS) attack. For additional protection against DDoS attacks, AWS also provides AWS Shield Standard and AWS Shield Advanced.

**Origins**

• S3 bucket
	• For distributing files and caching them at the edge
	• Enhanced security with CloudFront Origin Access Control (OAC)
	• OAC is replacing Origin Access Identity (OAI)
	• CloudFront can be used as an ingress (to upload files to S3)
	
• Custom Origin (HTTP)
	• Application Load Balancer
	• EC2 instance
	• S3 website (must first enable the bucket as a static S3 website)
	• Any HTTP backend you want