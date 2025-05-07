
EC2 Hibernate is a feature in Amazon Web Services (AWS) that allows you to pause and resume your [[EC2 instance]], preserving their in-memory state in [[EBS Volume]].

- This enables rapid startup on instances since it preserves the RAM state
- To enable HIbernate the EC2 Instance Root volume must be an EBS Volume and it must be encrypted.