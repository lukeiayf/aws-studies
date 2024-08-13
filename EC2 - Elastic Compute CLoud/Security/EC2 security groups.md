Security groups for EC2 instances have inbound and outbound rules for data access, take the diagram as example: 
![[EC2 security groups.png]]

- Can be attached to multiple instances;
- Locked down to a region;
- They live outside the EC2 -  if traffic is blocked the EC2 instance won't see;
- It's good to maintain one separate security group for SSH access;
- If application timed out it is a security group issue;
- If application gives 'connection refused', it's an application error or the instance is not launched;
- All inbound traffic is blocked by default;
- All outbound traffic is authorized by default;
- You can reference another security group to the one already attached to the instance through [[Security group referencing]];