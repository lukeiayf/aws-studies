• An ELB (Elastic Load Balancer) is a managed load balancer
• AWS guarantees that it will be working
• AWS takes care of upgrades, maintenance, high availability
• AWS provides only a few configuration knobs
• It costs less to setup your own load balancer but it will be a lot more
effort on your end (maintenance, integrations)

- ELBs can also work in Hybrid mode on on premises if needed

	- ELBs are not considered a single point of failure.

 **Kinds of load balancers offered by AWS:**

• [[ALB - Application load balancer]] (HTTP / HTTPS only) – Layer 7
• [[NLB - Network Load Balancer]] (ultra-high performance, allows for TCP) – Layer 4
• [[GWLB - Gateway Load Balancer]] – Layer 3
• Classic Load Balancer (retired in 2023) – Layer 4 & 7

![[ELBs.png]]