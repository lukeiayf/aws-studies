• At rest: data stored or archived on a device
• On a hard disk, on a RDS instance, in S3 Glacier Deep Archive, etc.
• In transit (in motion): data being moved from one location to another
• Transfer from on-premises to AWS, EC2 to DynamoDB, etc.
• Means data transferred on the network
• We want to encrypt data in both states to protect it!
• For this we leverage **encryption keys**