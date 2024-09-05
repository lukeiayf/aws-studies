• IPv4 – Internet Protocol version 4 (4.3 Billion Addresses)
	• Public IPv4 – can be used on the Internet
	• EC2 instance gets a new a public IP address every time you stop then start it (default)
	• Private IPv4 – can be used on private networks (LAN) such as internal AWS networking (e.g., 192.168.1.1)
• Private IPv4 is fixed for EC2 Instances even if you start/stop them

• Elastic IP – allows you to attach a fixed public IPv4 address to EC2 instance
• Note: all public IPv4 on AWS will be charged $0.005 per hour (including EIP)
	• Free Tier: 750 hours usage per month

• IPv6 – Internet Protocol version 6 (3.4 × 10!" Addresses)
	• Every IP address is public in AWS (no private range)
	• Example: 2001:db8:3333:4444:cccc:dddd:eeee:ffff
	• Free