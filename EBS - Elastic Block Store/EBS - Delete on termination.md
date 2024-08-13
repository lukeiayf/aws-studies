• Controls the EBS behaviour when an EC2 instance terminates
• By default, the root EBS volume is deleted (attribute enabled)
• By default, any other attached EBS volume is not deleted (attribute disabled)
• This can be controlled by the AWS console / AWS CLI
• Use case: preserve root volume when instance is terminated