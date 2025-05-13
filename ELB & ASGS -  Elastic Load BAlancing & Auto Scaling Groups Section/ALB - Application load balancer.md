
Work in the application layer
Allows you to load balance to multiple applications in the same [[EC2 instance]]  using [[ECS - Elastic Container Service]]

Components:

- Listener -> where data is coming from
- Target group -> where data is going to (made of EC2 instances for example)
	- Can be EC2 (managed by [[ASG - Auto Scaling Group]])
	- ECS tasks
	- [[AWS Lambda]] functions
	- IP addresses (private)
- Rules -> coordinate listeners and target groups to direct flow if necessary

**Good to know**
- You get a fixed hostname (xxx.region.elb.amazonaws.com)
- The application servers don't see the IP of the client directly
	- The true IP is inserted in the HTTP header: **X-Fowarded-For**
	- We also get **X-Fowarded-Port** and **X-Fowarded-Proto**