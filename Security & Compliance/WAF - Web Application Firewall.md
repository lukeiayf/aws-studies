• Protects your web applications from common web exploits (Layer 7)
• Layer 7 is HTTP (vs Layer 4 is TCP)
• Deploy on Application Load Balancer, API Gateway, CloudFront

• Define Web ACL (Web Access Control List):
• Rules can include IP addresses, HTTP headers, HTTP body, or URI strings
• Protects from common attack - SQL injection and Cross-Site Scripting (XSS)
• Size constraints, geo-match (block countries)
• Rate-based rules (to count occurrences of events) – for DDoS protection